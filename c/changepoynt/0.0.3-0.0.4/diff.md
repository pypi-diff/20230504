# Comparing `tmp/changepoynt-0.0.3.tar.gz` & `tmp/changepoynt-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "changepoynt-0.0.3.tar", last modified: Mon Mar 27 12:36:46 2023, max compression
+gzip compressed data, was "changepoynt-0.0.4.tar", last modified: Thu May  4 09:54:03 2023, max compression
```

## Comparing `changepoynt-0.0.3.tar` & `changepoynt-0.0.4.tar`

### file list

```diff
@@ -1,44 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-03-27 12:36:46.427169 changepoynt-0.0.3/
--rw-rw-rw-   0        0        0     1339 2023-03-09 14:46:45.000000 changepoynt-0.0.3/LICENSE
--rw-rw-rw-   0        0        0       25 2023-03-17 16:14:28.000000 changepoynt-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      601 2023-03-27 12:36:46.427169 changepoynt-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       32 2023-03-09 14:59:23.000000 changepoynt-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-03-27 12:36:46.411542 changepoynt-0.0.3/changepoynt/
--rw-rw-rw-   0        0        0        0 2023-03-07 14:04:42.000000 changepoynt-0.0.3/changepoynt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-27 12:36:46.427169 changepoynt-0.0.3/changepoynt/algorithms/
--rw-rw-rw-   0        0        0        0 2023-03-07 13:36:15.000000 changepoynt-0.0.3/changepoynt/algorithms/__init__.py
--rw-rw-rw-   0        0        0      281 2023-03-17 13:02:18.000000 changepoynt-0.0.3/changepoynt/algorithms/base_algorithm.py
--rw-rw-rw-   0        0        0     5829 2023-03-27 11:06:08.000000 changepoynt-0.0.3/changepoynt/algorithms/floss.py
--rw-rw-rw-   0        0        0     2923 2023-03-27 09:53:53.000000 changepoynt-0.0.3/changepoynt/algorithms/fluss.py
--rw-rw-rw-   0        0        0     5919 2023-03-24 08:33:41.000000 changepoynt-0.0.3/changepoynt/algorithms/rulsif.py
--rw-rw-rw-   0        0        0    10764 2023-03-14 17:00:32.000000 changepoynt-0.0.3/changepoynt/algorithms/si.py
--rw-rw-rw-   0        0        0    22337 2023-03-17 13:02:18.000000 changepoynt-0.0.3/changepoynt/algorithms/sst.py
--rw-rw-rw-   0        0        0     2669 2023-03-17 14:53:55.000000 changepoynt-0.0.3/changepoynt/algorithms/ulsif.py
-drwxrwxrwx   0        0        0        0 2023-03-27 12:36:46.427169 changepoynt-0.0.3/changepoynt/utils/
--rw-rw-rw-   0        0        0        0 2023-03-06 13:15:58.000000 changepoynt-0.0.3/changepoynt/utils/__init__.py
--rw-rw-rw-   0        0        0    20061 2023-03-17 15:29:17.000000 changepoynt-0.0.3/changepoynt/utils/densityratioestimation.py
--rw-rw-rw-   0        0        0    11996 2023-03-14 17:36:01.000000 changepoynt-0.0.3/changepoynt/utils/linalg.py
--rw-rw-rw-   0        0        0     1569 2023-03-07 15:42:55.000000 changepoynt-0.0.3/changepoynt/utils/normalization.py
-drwxrwxrwx   0        0        0        0 2023-03-27 12:36:46.427169 changepoynt-0.0.3/changepoynt/visualization/
--rw-rw-rw-   0        0        0        0 2023-03-14 12:37:51.000000 changepoynt-0.0.3/changepoynt/visualization/__init__.py
--rw-rw-rw-   0        0        0      548 2023-03-24 14:48:11.000000 changepoynt-0.0.3/changepoynt/visualization/score_plotting.py
-drwxrwxrwx   0        0        0        0 2023-03-27 12:36:46.411542 changepoynt-0.0.3/changepoynt.egg-info/
--rw-rw-rw-   0        0        0      601 2023-03-27 12:36:46.000000 changepoynt-0.0.3/changepoynt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      956 2023-03-27 12:36:46.000000 changepoynt-0.0.3/changepoynt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-27 12:36:46.000000 changepoynt-0.0.3/changepoynt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-07 14:02:39.000000 changepoynt-0.0.3/changepoynt.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      176 2023-03-27 12:36:46.000000 changepoynt-0.0.3/changepoynt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-03-27 12:36:46.000000 changepoynt-0.0.3/changepoynt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       90 2023-03-24 13:56:32.000000 changepoynt-0.0.3/requirements.txt
--rw-rw-rw-   0        0        0      119 2023-03-24 13:56:32.000000 changepoynt-0.0.3/requirements_examples.txt
--rw-rw-rw-   0        0        0       86 2023-03-24 13:56:32.000000 changepoynt-0.0.3/requirements_tests.txt
--rw-rw-rw-   0        0        0       42 2023-03-27 12:36:46.427169 changepoynt-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1548 2023-03-27 12:12:52.000000 changepoynt-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-27 12:36:46.427169 changepoynt-0.0.3/tests/
--rw-rw-rw-   0        0        0      975 2023-03-27 11:07:21.000000 changepoynt-0.0.3/tests/test_floss.py
--rw-rw-rw-   0        0        0      921 2023-03-24 14:17:58.000000 changepoynt-0.0.3/tests/test_fluss.py
--rw-rw-rw-   0        0        0     3987 2023-03-09 12:44:11.000000 changepoynt-0.0.3/tests/test_linalg.py
--rw-rw-rw-   0        0        0      923 2023-03-17 13:07:07.000000 changepoynt-0.0.3/tests/test_rulsif.py
--rw-rw-rw-   0        0        0      983 2023-03-27 12:10:40.000000 changepoynt-0.0.3/tests/test_si.py
--rw-rw-rw-   0        0        0     1683 2023-03-14 16:21:57.000000 changepoynt-0.0.3/tests/test_sst.py
--rw-rw-rw-   0        0        0      919 2023-03-17 13:08:02.000000 changepoynt-0.0.3/tests/test_ulsif.py
+drwxrwxrwx   0        0        0        0 2023-05-04 09:54:03.550902 changepoynt-0.0.4/
+-rw-rw-rw-   0        0        0     1339 2023-03-09 14:46:45.000000 changepoynt-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0       44 2023-05-04 09:46:22.000000 changepoynt-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     4830 2023-05-04 09:54:03.550902 changepoynt-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4204 2023-05-04 09:38:34.000000 changepoynt-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 09:54:03.425039 changepoynt-0.0.4/changepoynt/
+-rw-rw-rw-   0        0        0      195 2023-03-31 08:44:08.000000 changepoynt-0.0.4/changepoynt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 09:54:03.487923 changepoynt-0.0.4/changepoynt/algorithms/
+-rw-rw-rw-   0        0        0        0 2023-03-07 13:36:15.000000 changepoynt-0.0.4/changepoynt/algorithms/__init__.py
+-rw-rw-rw-   0        0        0      281 2023-03-17 13:02:18.000000 changepoynt-0.0.4/changepoynt/algorithms/base_algorithm.py
+-rw-rw-rw-   0        0        0     3228 2023-04-12 09:41:05.000000 changepoynt-0.0.4/changepoynt/algorithms/clasp.py
+-rw-rw-rw-   0        0        0     7876 2023-04-12 09:20:49.000000 changepoynt-0.0.4/changepoynt/algorithms/esst.py
+-rw-rw-rw-   0        0        0     5970 2023-05-04 09:39:07.000000 changepoynt-0.0.4/changepoynt/algorithms/floss.py
+-rw-rw-rw-   0        0        0     2923 2023-04-13 21:46:01.000000 changepoynt-0.0.4/changepoynt/algorithms/fluss.py
+-rw-rw-rw-   0        0        0     5919 2023-03-24 08:33:41.000000 changepoynt-0.0.4/changepoynt/algorithms/rulsif.py
+-rw-rw-rw-   0        0        0    10764 2023-03-14 17:00:32.000000 changepoynt-0.0.4/changepoynt/algorithms/si.py
+-rw-rw-rw-   0        0        0    22746 2023-04-13 21:43:35.000000 changepoynt-0.0.4/changepoynt/algorithms/sst.py
+-rw-rw-rw-   0        0        0     7179 2023-04-20 16:10:34.000000 changepoynt-0.0.4/changepoynt/algorithms/torch_esst.py
+-rw-rw-rw-   0        0        0     2669 2023-03-17 14:53:55.000000 changepoynt-0.0.4/changepoynt/algorithms/ulsif.py
+drwxrwxrwx   0        0        0        0 2023-05-04 09:54:03.519191 changepoynt-0.0.4/changepoynt/utils/
+-rw-rw-rw-   0        0        0        0 2023-03-06 13:15:58.000000 changepoynt-0.0.4/changepoynt/utils/__init__.py
+-rw-rw-rw-   0        0        0    20061 2023-03-17 15:29:17.000000 changepoynt-0.0.4/changepoynt/utils/densityratioestimation.py
+-rw-rw-rw-   0        0        0    12092 2023-04-11 16:57:50.000000 changepoynt-0.0.4/changepoynt/utils/linalg.py
+-rw-rw-rw-   0        0        0     2756 2023-04-04 14:32:02.000000 changepoynt-0.0.4/changepoynt/utils/normalization.py
+drwxrwxrwx   0        0        0        0 2023-05-04 09:54:03.519191 changepoynt-0.0.4/changepoynt/visualization/
+-rw-rw-rw-   0        0        0        0 2023-03-14 12:37:51.000000 changepoynt-0.0.4/changepoynt/visualization/__init__.py
+-rw-rw-rw-   0        0        0      600 2023-04-11 16:20:18.000000 changepoynt-0.0.4/changepoynt/visualization/score_plotting.py
+drwxrwxrwx   0        0        0        0 2023-05-04 09:54:03.431548 changepoynt-0.0.4/changepoynt.egg-info/
+-rw-rw-rw-   0        0        0     4830 2023-05-04 09:54:03.000000 changepoynt-0.0.4/changepoynt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1076 2023-05-04 09:54:03.000000 changepoynt-0.0.4/changepoynt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 09:54:03.000000 changepoynt-0.0.4/changepoynt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-07 14:02:39.000000 changepoynt-0.0.4/changepoynt.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      204 2023-05-04 09:54:03.000000 changepoynt-0.0.4/changepoynt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-04 09:54:03.000000 changepoynt-0.0.4/changepoynt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      105 2023-04-11 12:57:47.000000 changepoynt-0.0.4/requirements.txt
+-rw-rw-rw-   0        0        0      134 2023-03-30 12:56:50.000000 changepoynt-0.0.4/requirements_examples.txt
+-rw-rw-rw-   0        0        0      101 2023-03-30 12:56:50.000000 changepoynt-0.0.4/requirements_tests.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 09:54:03.550902 changepoynt-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1638 2023-05-04 09:52:46.000000 changepoynt-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 09:54:03.550902 changepoynt-0.0.4/tests/
+-rw-rw-rw-   0        0        0      919 2023-04-11 12:54:42.000000 changepoynt-0.0.4/tests/test_clasp.py
+-rw-rw-rw-   0        0        0      975 2023-03-27 11:07:21.000000 changepoynt-0.0.4/tests/test_floss.py
+-rw-rw-rw-   0        0        0      921 2023-03-24 14:17:58.000000 changepoynt-0.0.4/tests/test_fluss.py
+-rw-rw-rw-   0        0        0     3987 2023-03-09 12:44:11.000000 changepoynt-0.0.4/tests/test_linalg.py
+-rw-rw-rw-   0        0        0      923 2023-03-17 13:07:07.000000 changepoynt-0.0.4/tests/test_rulsif.py
+-rw-rw-rw-   0        0        0      983 2023-03-27 12:10:40.000000 changepoynt-0.0.4/tests/test_si.py
+-rw-rw-rw-   0        0        0     1575 2023-04-11 13:13:08.000000 changepoynt-0.0.4/tests/test_sst.py
+-rw-rw-rw-   0        0        0      919 2023-03-17 13:08:02.000000 changepoynt-0.0.4/tests/test_ulsif.py
```

### Comparing `changepoynt-0.0.3/LICENSE` & `changepoynt-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `changepoynt-0.0.3/changepoynt/algorithms/floss.py` & `changepoynt-0.0.4/changepoynt/algorithms/floss.py`

 * *Files 10% similar despite different names*

```diff
@@ -53,20 +53,20 @@
         assert time_series.ndim == 1, "Time series needs to be an 1D array."
 
         # check that we have at least two windows
         assert time_series.shape[0] > self.initial_length, \
             'Time series needs to be longer than specified initial length.'
 
         # feed it through the online process
-        print(self.initial_length, self.window_length)
         score = _transform(time_series, self.initial_length, self.window_length)
         return score
 
 
 def save_animation(mp, windows, time_series):
+    import matplotlib.pyplot as plt
     from matplotlib import animation
     import os
 
     fig, axs = plt.subplots(2, sharex=True, gridspec_kw={'hspace': 0})
 
     axs[0].set_xlim((0, mp.shape[0]))
     axs[0].set_ylim((min(time_series), max(time_series)))
@@ -76,14 +76,17 @@
     lines = []
     for ax in axs:
         line, = ax.plot([], [], lw=2)
         lines.append(line)
     line, = axs[1].plot([], [], lw=2)
     lines.append(line)
 
+    # mark the window lengths
+    axs[1].plot([401, 401], (0, mp.shape[0]))
+
     def init():
         for line in lines:
             line.set_data([], [])
         return lines
 
     def animate(window):
         data_out, cac_out = window
@@ -113,40 +116,40 @@
     # create the initial matrix profile
     matrix_profile = stumpy.stump(init_signal, m=window_length)
 
     # initialize the floss object
     stream = stumpy.floss(matrix_profile, init_signal, m=window_length, L=window_length, excl_factor=1)
 
     # make the score vector
-    score = np.ones_like(time_series)
-    score[:start_idx] = 0
+    score = np.zeros_like(time_series)
+    score[:start_idx] = 1
 
     # iterate over all the values in the signal starting at start_idx computing the change point score
     windows = []
     for idx in range(start_idx, time_series.shape[0]):
 
         # update the floss streaming module
         stream.update(time_series[idx])
 
         # get the latest score (1-cac)
-        score[idx] -= stream.cac_1d_[-window_length+1]
+        score[idx] = stream.cac_1d_[-window_length-2]
 
-        if idx % 20 == 0:
-            windows.append((stream.T_, stream.cac_1d_))
+        if idx % 20 == 0: windows.append((stream.T_, stream.cac_1d_))
     save_animation(matrix_profile, windows, time_series)
-    return score
+    return 1-score
 
 
 def _main():
     """
     Internal quick testing function.
 
     :return:
     """
     from time import time
+    import matplotlib.pyplot as plt
     # make synthetic step function
     np.random.seed(123)
     # synthetic (frequency change)
     x0 = np.sin(2 * np.pi * 1 * np.linspace(0, 10, 1000))
     x1 = np.sin(2 * np.pi * 2 * np.linspace(0, 10, 1000))
     x2 = np.sin(2 * np.pi * 8 * np.linspace(0, 10, 1000))
     x3 = np.sin(2 * np.pi * 4 * np.linspace(0, 10, 1000))
@@ -155,12 +158,15 @@
 
     # create the method
     fluss_recognizer = FLOSS(50)
 
     # compute the score
     start = time()
     score = fluss_recognizer.transform(x)
+    plt.plot(x)
+    plt.plot(score)
+    plt.show()
     print(f'Computation for {len(x)} signal values took {time()-start} s.')
 
 
 if __name__ == '__main__':
     _main()
```

### Comparing `changepoynt-0.0.3/changepoynt/algorithms/fluss.py` & `changepoynt-0.0.4/changepoynt/algorithms/fluss.py`

 * *Files identical despite different names*

### Comparing `changepoynt-0.0.3/changepoynt/algorithms/rulsif.py` & `changepoynt-0.0.4/changepoynt/algorithms/rulsif.py`

 * *Files identical despite different names*

### Comparing `changepoynt-0.0.3/changepoynt/algorithms/si.py` & `changepoynt-0.0.4/changepoynt/algorithms/si.py`

 * *Files identical despite different names*

### Comparing `changepoynt-0.0.3/changepoynt/algorithms/sst.py` & `changepoynt-0.0.4/changepoynt/algorithms/sst.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import numpy as np
-from numba import jit
 from changepoynt.utils import linalg as lg
 from changepoynt.utils import normalization
 from typing import Callable
 from functools import partial
 from changepoynt.algorithms.base_algorithm import Algorithm
 
 
-class SingularSpectrumTransformation(Algorithm):
+class SST(Algorithm):
     """
     This class implements all the utility and functionality necessary to compute the SST change point detection
     algorithm as described in:
 
     [1]
     Idé, Tsuyoshi, and Keisuke Inoue.
     "Knowledge discovery from heterogeneous dynamic systems using change-point correlations."
@@ -43,15 +42,15 @@
 
     Also, we decided to do type hinting but not type checking as it requires too much boilerplate code. We recommend
     to input the specified types as the program will break in unforeseen ways otherwise.
     """
 
     def __init__(self, window_length: int, n_windows: int = None, lag: int = None, rank: int = 5, scale: bool = True,
                  method: str = 'ika', lanczos_rank: int = None, random_rank: int = None,
-                 feedback_noise_level: float = 1e-3) -> None:
+                 feedback_noise_level: float = 1e-3, scoring_step: int = 1) -> None:
         """
         Initializing the Singular Spectrum Transformation (SST) requires setting a lot of parameters. See the parameters
         explanation for some intuition into the right choices. Currently, there are two SST methods from [1] and [2]
         available for use.
 
         :param window_length: This specifies the length of the time series (in samples), which will be used to extract
         the representative "eigensignals" to be compared before and after the lag. The windows length should be big
@@ -88,26 +87,29 @@
         this value, the faster the computation but the higher the error (as the approximation gets worse).
 
         :param feedback_noise_level: This specifies the amplitude of additive white gaussian noise added to the dominant
         "eigensignal" of the future behavior when shifting forward. This idea is noted in [2] and initializes
         the seed of the power method for dominant eigenvector estimation with the precious dominant eigenvector
         plus the noise level specified here. The noise level should just be a small fraction of the value range
         of the signal.
+
+        :param scoring_step: the distance between scoring steps in samples.
         """
 
         # save the specified parameters into instance variables
         self.window_length = window_length
         self.n_windows = n_windows
         self.lag = lag
         self.rank = rank
         self.scale = scale
         self.method = method
         self.lanczos_rank = lanczos_rank
         self.random_rank = random_rank
         self.noise = feedback_noise_level
+        self.scoring_step = scoring_step
 
         # set some default values when they have not been specified
         if self.n_windows is None:
             self.n_windows = self.window_length
         if self.lag is None:
             # rule of thumb
             self.lag = max(self.n_windows//3, 1)
@@ -168,50 +170,57 @@
             time_series = time_series.copy()
 
         # get the changepoint scorer from the different methods
         scoring_function = self.methods[self.method]
 
         # start the scaling itself by calling the jit compiled staticmethod and return the result
         score = _transform(time_series=time_series, start_idx=starting_point, window_length=self.window_length,
-                           n_windows=self.n_windows, lag=self.lag, scoring_function=scoring_function)
+                           n_windows=self.n_windows, lag=self.lag, scoring_step=self.scoring_step,
+                           scoring_function=scoring_function)
         return score
 
 
-def _transform(time_series: np.ndarray, start_idx: int, window_length: int, n_windows: int, lag: int,
+def _transform(time_series: np.ndarray, start_idx: int, window_length: int, n_windows: int, lag: int, scoring_step: int,
                scoring_function: Callable) -> np.ndarray:
     """
     Compute heavy and hopefully jit compilable score computation for the SST method. It does not do any parameter
     checking and can throw cryptic errors. It's only used for internal use as a private function.
 
     :param time_series: 1D array containing the time series to be scored
     :param start_idx: integer defining the start sample index for the score computation
     :param window_length: the size of the time series window for each column of the hankel matrix
     :param n_windows: amount of columns in the hankel matrix
     :param lag: sample distance between future and past hankel matrix
+    :param scoring_step: the distance between scoring steps in samples.
+    :param scoring_function: the function that is called every step to assess a scalar change point score
     """
 
     # create initial vector for ika method with feedback dominant eigenvector as proposed in [2]
     # with a norm of one
     x0 = np.random.rand(n_windows)
     x0 /= np.linalg.norm(x0)
 
     # initialize a scoring array with no values yet
     score = np.zeros_like(time_series)
 
+    # make an offset for the data construction
+    offset = n_windows//2+lag
+
     # iterate over all the values in the signal starting at start_idx computing the change point score
-    for idx in range(start_idx, time_series.shape[0]):
+    for idx in range(start_idx, time_series.shape[0], scoring_step):
 
         # compile the past hankel matrix (H1)
         hankel_past = lg.compile_hankel(time_series, idx-lag, window_length, n_windows)
 
         # compile the future hankel matrix (H2)
         hankel_future = lg.compile_hankel(time_series, idx, window_length, n_windows)
 
         # compute the score and save the returned feedback vector
-        score[idx], x1 = scoring_function(hankel_past, hankel_future, x0)
+        score[idx-offset-scoring_step//2:idx-offset+(scoring_step+1)//2], x1 = \
+            scoring_function(hankel_past, hankel_future, x0)
 
         # add noise to the dominant eigenvector and normalize it again
         x0 = x1 + 1e-3 * np.random.rand(x0.size)
         x0 /= np.linalg.norm(x0)
 
     return score
 
@@ -403,18 +412,18 @@
     length = 300
     x = np.hstack([1 * np.ones(length) + np.random.rand(length) * 1,
                    3 * np.ones(length) + np.random.rand(length) * 2,
                    5 * np.ones(length) + np.random.rand(length) * 1.5])
     x += np.random.rand(x.size)
 
     # create the sst method
-    ika_sst = SingularSpectrumTransformation(31, method='ika')
-    svd_sst = SingularSpectrumTransformation(31, method='svd')
-    rsvd_sst = SingularSpectrumTransformation(31, method='rsvd')
-    fbrsvd_sst = SingularSpectrumTransformation(31, method='fbrsvd')
+    ika_sst = SST(31, method='ika')
+    svd_sst = SST(31, method='svd')
+    rsvd_sst = SST(31, method='rsvd')
+    fbrsvd_sst = SST(31, method='fbrsvd')
 
     # make the scoring
     start = time()
     ika_sst.transform(x)
     print((time() - start) / (length * 3))
     svd_sst.transform(x)
     rsvd_sst.transform(x)
```

### Comparing `changepoynt-0.0.3/changepoynt/algorithms/ulsif.py` & `changepoynt-0.0.4/changepoynt/algorithms/ulsif.py`

 * *Files identical despite different names*

### Comparing `changepoynt-0.0.3/changepoynt/utils/densityratioestimation.py` & `changepoynt-0.0.4/changepoynt/utils/densityratioestimation.py`

 * *Files identical despite different names*

### Comparing `changepoynt-0.0.3/changepoynt/utils/linalg.py` & `changepoynt-0.0.4/changepoynt/utils/linalg.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,34 +252,35 @@
     # test irlbd
     eigval, eigvec, = implicit_restarted_lanczos_bidiagonalization(A, 20)
     eigvecs, eigvals, _ = np.linalg.svd(A)
     print(eigval, eigvals[0])
 
 
 @jit(nopython=True)
-def compile_hankel(time_series: np.ndarray, end_index: int, window_size: int, rank: int) -> np.ndarray:
+def compile_hankel(time_series: np.ndarray, end_index: int, window_size: int, rank: int, lag: int = 1) -> np.ndarray:
     """
     This function constructs a hankel matrix from a 1D time series. Please make sure constructing the matrix with
     the given parameters (end index, window size, etc.) is possible, as this function does no checks due to
     performance reasons.
 
     :param time_series: 1D array with float values as the time series
     :param end_index: the index (point in time) where the time series starts
     :param window_size: the size of the windows cut from the time series
     :param rank: the amount of time series in the matrix
+    :param lag: the lag between the time series of the different columns
     :return: The hankel matrix with lag one
     """
 
     # make an empty matrix to place the values
     #
     # almost no faster way:
     # https://stackoverflow.com/questions/71410927/vectorized-way-to-construct-a-block-hankel-matrix-in-numpy-or-scipy
     hankel = np.empty((window_size, rank))
 
     # go through the time series and make the hankel matrix
     for cx in range(rank):
-        hankel[:, cx] = time_series[(end_index-window_size-cx):(end_index-cx)]
+        hankel[:, cx] = time_series[(end_index-window_size-cx*lag):(end_index-cx*lag)]
     return hankel
 
 
 if __name__ == '__main__':
     examples()
```

### Comparing `changepoynt-0.0.3/changepoynt/utils/normalization.py` & `changepoynt-0.0.4/changepoynt/utils/normalization.py`

 * *Files 17% similar despite different names*

```diff
@@ -27,7 +27,37 @@
 
     # scale the time series to values between zero and one
     time_series = (time_series-np.min(time_series, axis=0)) / (np.max(time_series, axis=0)-np.min(time_series, axis=0))
 
     # scale into the wished value range
     time_series = time_series * (max_val - min_val) + min_val
     return time_series
+
+
+def z_scaling(time_series: np.ndarray, inplace: bool = False) -> np.ndarray:
+    """
+    This function applie z-normalization to an 1D-array. It is inspired by:
+    https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.StandardScaler.html
+    but lighter and reimplemented in order to not introduce unnecessary dependencies for small functionality.
+
+    :param time_series: 1D array containing consecutive values for one feature
+    :param min_val: the minimum value the scaled time series will reach
+    :param max_val: the maximum value the scale time series will reach
+    :param inplace: boolean to specify whether the input array will be scaled and changed in place
+
+    :return: the scaled input array.
+    """
+    # make some assertion checks
+    assert time_series.ndim == 1, 'Time series needs to be an 1D array.'
+
+    # copy the time series if specified
+    if not inplace: time_series = time_series.copy()
+
+    # compute sample mean and sample variance
+    mean = np.mean(time_series)
+    std = np.std(time_series)
+
+    # subtract the mean
+    time_series -= mean
+    if std:
+        time_series /= std
+    return time_series
```

### Comparing `changepoynt-0.0.3/changepoynt/visualization/score_plotting.py` & `changepoynt-0.0.4/changepoynt/visualization/score_plotting.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,7 +10,9 @@
     ax[1].set_title("change score")
     x_grid, y_grid = np.meshgrid(np.arange(len(score)), np.linspace(*ax[0].get_ylim()))
     if np.max(score):
         z_grid = (score/np.max(score))[x_grid]
     else:
         z_grid = score[x_grid]
     ax[0].contourf(x_grid, y_grid, z_grid, alpha=0.5, cmap="BuPu")
+    ax[1].set_xlim(ax[0].get_xlim())
+    return f
```

### Comparing `changepoynt-0.0.3/changepoynt.egg-info/SOURCES.txt` & `changepoynt-0.0.4/changepoynt.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -10,26 +10,30 @@
 changepoynt.egg-info/SOURCES.txt
 changepoynt.egg-info/dependency_links.txt
 changepoynt.egg-info/not-zip-safe
 changepoynt.egg-info/requires.txt
 changepoynt.egg-info/top_level.txt
 changepoynt/algorithms/__init__.py
 changepoynt/algorithms/base_algorithm.py
+changepoynt/algorithms/clasp.py
+changepoynt/algorithms/esst.py
 changepoynt/algorithms/floss.py
 changepoynt/algorithms/fluss.py
 changepoynt/algorithms/rulsif.py
 changepoynt/algorithms/si.py
 changepoynt/algorithms/sst.py
+changepoynt/algorithms/torch_esst.py
 changepoynt/algorithms/ulsif.py
 changepoynt/utils/__init__.py
 changepoynt/utils/densityratioestimation.py
 changepoynt/utils/linalg.py
 changepoynt/utils/normalization.py
 changepoynt/visualization/__init__.py
 changepoynt/visualization/score_plotting.py
+tests/test_clasp.py
 tests/test_floss.py
 tests/test_fluss.py
 tests/test_linalg.py
 tests/test_rulsif.py
 tests/test_si.py
 tests/test_sst.py
 tests/test_ulsif.py
```

### Comparing `changepoynt-0.0.3/setup.py` & `changepoynt-0.0.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,25 +6,30 @@
 # read the contents of requirements.txt
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'requirements.txt'), encoding='utf-8') as f:
     requirements = f.read().splitlines()
 with open(path.join(this_directory, 'requirements_tests.txt'), encoding='utf-8') as f:
     requirements_tests = f.read().splitlines()
 
+# read content of the readme
+with open(path.join(this_directory, 'README.md')) as f:
+    long_description = f.read()
+
 
 def main():
 
     setup(
         name="changepoynt",
-        version="0.0.3",
+        version="0.0.4",
         author="Lucas Weber",
         author_email="weber-lucas@web.de",
         url="https://github.com/Lucew/changepoynt",
-        description="Readable package for several change point detection methods implemented in python.",
-        long_description="This package contains several readable change point detections methods in python.",
+        description="Several change point detection methods implemented in python.",
+        long_description=long_description,
+        long_description_content_type='text/markdown',
         zip_safe=False,
         include_package_data=True,
         packages=find_packages(exclude=['tests']),
         install_requires=requirements,
         dependency_links=[],
         tests_require=requirements_tests,
         extras_require={'test': requirements_tests},
```

### Comparing `changepoynt-0.0.3/tests/test_floss.py` & `changepoynt-0.0.4/tests/test_floss.py`

 * *Files identical despite different names*

### Comparing `changepoynt-0.0.3/tests/test_fluss.py` & `changepoynt-0.0.4/tests/test_fluss.py`

 * *Files identical despite different names*

### Comparing `changepoynt-0.0.3/tests/test_linalg.py` & `changepoynt-0.0.4/tests/test_linalg.py`

 * *Files identical despite different names*

### Comparing `changepoynt-0.0.3/tests/test_rulsif.py` & `changepoynt-0.0.4/tests/test_rulsif.py`

 * *Files identical despite different names*

### Comparing `changepoynt-0.0.3/tests/test_si.py` & `changepoynt-0.0.4/tests/test_si.py`

 * *Files identical despite different names*

### Comparing `changepoynt-0.0.3/tests/test_sst.py` & `changepoynt-0.0.4/tests/test_sst.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,28 +21,28 @@
         self.signal = x
 
     def teardown_method(self):
         pass
 
     def test_all_methods(self):
         # initialize random default method
-        sst = ssts.SingularSpectrumTransformation(30)
+        sst = ssts.SST(30)
 
         # get the different method names
         methods = list(sst.methods.keys())
 
         # go through the methods and check execution
         for method in methods:
             LOGGER.info(f'Starting SST for method {method}')
-            ssts.SingularSpectrumTransformation(min(5, self.signal_length//2), rank=2,
+            ssts.SST(min(5, self.signal_length//2), rank=2,
                                                 method=method).transform(self.signal)
 
     def test_default(self):
-        ssts.SingularSpectrumTransformation(min(5, self.signal_length//2), rank=2).transform(self.signal)
+        ssts.SST(min(5, self.signal_length//2), rank=2).transform(self.signal)
 
     def test_unknown_method(self):
         with pytest.raises(AssertionError):
-            ssts.SingularSpectrumTransformation(10, method='asdafwegrhqh')
+            ssts.SST(10, method='asdafwegrhqh')
 
 
 if __name__ == "__main__":
     pytest.main()
```

### Comparing `changepoynt-0.0.3/tests/test_ulsif.py` & `changepoynt-0.0.4/tests/test_ulsif.py`

 * *Files identical despite different names*

