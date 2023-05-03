# Comparing `tmp/auto_shap-0.1.1.tar.gz` & `tmp/auto_shap-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/auto_shap-0.1.1.tar", last modified: Sun Sep  4 03:35:18 2022, max compression
+gzip compressed data, was "dist/auto_shap-0.2.0.tar", last modified: Wed May  3 23:47:03 2023, max compression
```

## Comparing `auto_shap-0.1.1.tar` & `auto_shap-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 micahmelling   (501) staff       (20)        0 2022-09-04 03:35:18.000000 auto_shap-0.1.1/
--rw-r--r--   0 micahmelling   (501) staff       (20)    13111 2022-09-04 03:35:18.000000 auto_shap-0.1.1/PKG-INFO
--rw-r--r--   0 micahmelling   (501) staff       (20)    10738 2022-09-04 03:22:07.000000 auto_shap-0.1.1/README.md
-drwxr-xr-x   0 micahmelling   (501) staff       (20)        0 2022-09-04 03:35:18.000000 auto_shap-0.1.1/auto_shap/
--rw-r--r--   0 micahmelling   (501) staff       (20)       48 2022-09-04 03:34:43.000000 auto_shap-0.1.1/auto_shap/__init__.py
--rw-r--r--   0 micahmelling   (501) staff       (20)    20541 2022-09-03 21:37:56.000000 auto_shap-0.1.1/auto_shap/auto_shap.py
--rw-r--r--   0 micahmelling   (501) staff       (20)      334 2022-09-03 19:43:26.000000 auto_shap-0.1.1/auto_shap/config.py
--rw-r--r--   0 micahmelling   (501) staff       (20)     1551 2022-09-03 20:18:38.000000 auto_shap-0.1.1/auto_shap/scratch.py
--rw-r--r--   0 micahmelling   (501) staff       (20)     8987 2022-09-04 03:11:34.000000 auto_shap-0.1.1/auto_shap/utilities.py
-drwxr-xr-x   0 micahmelling   (501) staff       (20)        0 2022-09-04 03:35:18.000000 auto_shap-0.1.1/auto_shap.egg-info/
--rw-r--r--   0 micahmelling   (501) staff       (20)    13111 2022-09-04 03:35:18.000000 auto_shap-0.1.1/auto_shap.egg-info/PKG-INFO
--rw-r--r--   0 micahmelling   (501) staff       (20)      301 2022-09-04 03:35:18.000000 auto_shap-0.1.1/auto_shap.egg-info/SOURCES.txt
--rw-r--r--   0 micahmelling   (501) staff       (20)        1 2022-09-04 03:35:18.000000 auto_shap-0.1.1/auto_shap.egg-info/dependency_links.txt
--rw-r--r--   0 micahmelling   (501) staff       (20)       59 2022-09-04 03:35:18.000000 auto_shap-0.1.1/auto_shap.egg-info/requires.txt
--rw-r--r--   0 micahmelling   (501) staff       (20)       10 2022-09-04 03:35:18.000000 auto_shap-0.1.1/auto_shap.egg-info/top_level.txt
--rw-r--r--   0 micahmelling   (501) staff       (20)       79 2022-09-04 03:35:18.000000 auto_shap-0.1.1/setup.cfg
--rw-r--r--   0 micahmelling   (501) staff       (20)      801 2022-09-04 03:34:43.000000 auto_shap-0.1.1/setup.py
+drwxr-xr-x   0 micahmelling   (501) staff       (20)        0 2023-05-03 23:47:03.000000 auto_shap-0.2.0/
+-rw-r--r--   0 micahmelling   (501) staff       (20)    13528 2023-05-03 23:47:03.000000 auto_shap-0.2.0/PKG-INFO
+-rw-r--r--   0 micahmelling   (501) staff       (20)    11091 2023-05-03 23:44:57.000000 auto_shap-0.2.0/README.md
+drwxr-xr-x   0 micahmelling   (501) staff       (20)        0 2023-05-03 23:47:03.000000 auto_shap-0.2.0/auto_shap/
+-rw-r--r--   0 micahmelling   (501) staff       (20)       48 2023-05-03 04:47:03.000000 auto_shap-0.2.0/auto_shap/__init__.py
+-rw-r--r--   0 micahmelling   (501) staff       (20)    20598 2023-05-03 04:18:28.000000 auto_shap-0.2.0/auto_shap/auto_shap.py
+-rw-r--r--   0 micahmelling   (501) staff       (20)      334 2022-09-03 19:43:26.000000 auto_shap-0.2.0/auto_shap/config.py
+-rw-r--r--   0 micahmelling   (501) staff       (20)     1551 2022-09-03 20:18:38.000000 auto_shap-0.2.0/auto_shap/scratch.py
+-rw-r--r--   0 micahmelling   (501) staff       (20)     8987 2023-04-27 03:57:35.000000 auto_shap-0.2.0/auto_shap/utilities.py
+drwxr-xr-x   0 micahmelling   (501) staff       (20)        0 2023-05-03 23:47:03.000000 auto_shap-0.2.0/auto_shap.egg-info/
+-rw-r--r--   0 micahmelling   (501) staff       (20)    13528 2023-05-03 23:47:03.000000 auto_shap-0.2.0/auto_shap.egg-info/PKG-INFO
+-rw-r--r--   0 micahmelling   (501) staff       (20)      301 2023-05-03 23:47:03.000000 auto_shap-0.2.0/auto_shap.egg-info/SOURCES.txt
+-rw-r--r--   0 micahmelling   (501) staff       (20)        1 2023-05-03 23:47:03.000000 auto_shap-0.2.0/auto_shap.egg-info/dependency_links.txt
+-rw-r--r--   0 micahmelling   (501) staff       (20)       59 2023-05-03 23:47:03.000000 auto_shap-0.2.0/auto_shap.egg-info/requires.txt
+-rw-r--r--   0 micahmelling   (501) staff       (20)       10 2023-05-03 23:47:03.000000 auto_shap-0.2.0/auto_shap.egg-info/top_level.txt
+-rw-r--r--   0 micahmelling   (501) staff       (20)       79 2023-05-03 23:47:03.000000 auto_shap-0.2.0/setup.cfg
+-rw-r--r--   0 micahmelling   (501) staff       (20)      801 2023-05-03 04:47:03.000000 auto_shap-0.2.0/setup.py
```

### Comparing `auto_shap-0.1.1/PKG-INFO` & `auto_shap-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto_shap
-Version: 0.1.1
+Version: 0.2.0
 Summary: Calculate SHAP values in parallel and automatically detect what explainer to use
 Home-page: https://github.com/micahmelling/auto-shap
 Author: Micah Melling
 Author-email: micahmelling@gmail.com
 License: MIT
 Description: # auto-shap
         The auto-shap library is your best friend when calculating SHAP values!
@@ -25,15 +25,16 @@
         following when using the library.
         
         * The correct type of explainer class must be declared.
         * Our code for extracting SHAP values will be slightly different when we
         have a regression model compared to when we have a classifier.
         * SHAP cannot natively handel scikit-learn's CalibratedClassifierCV, voting models,
         or stacking models.
-        * Boosting models often have distinct behavior when it comes to SHAP values.
+        * Boosting models often have distinct behavior when it comes to SHAP values. For
+        boosting models, auto-shap will employ the SHAP settings to return probabilities.
         
         Likewise, the native SHAP library does not take advantage of multiprocessing.
         The auto-shap library will run SHAP calculations in parallel to speed them
         up when possible! When we are using a Tree or Linear Explainer, we can calculate our
         SHAP values in parallel without issue. The results will be the same compared
         to when we run our calculations on a single core. Such situations are heavily
         tested in tests/tests.py in the
@@ -43,18 +44,22 @@
         especially on small datasets, if we re-run the KernelExplain back-to-back on the
         same data with the same model, we won't get the exact same feature-level attribution,
         though the total attribution will stay the same (which is tested in tests/tests.py).
         The foregoing points can be substantiated by looking at the
         [SHAP documentation](https://shap-lrjball.readthedocs.io/en/latest/generated/shap.KernelExplainer.html#shap.KernelExplainer.shap_values).
         [This article](https://edden-gerber.github.io/shapley-part-2/) discusses the deterministic
         nature of certain SHAP calculations.
+        
         In auto-shap, we still employ multiprocessing when using the KernelExplainer, knowing
         that our results would still not be perfectly deterministic even on a single core,
-        and by using multiprocessing, we get a nice speed improvement. Additionally, there
-        is a pickle error when using multiprocessing with a scikit-learn Voting or
+        and by using multiprocessing, we get a nice speed improvement. To turn off
+        multiprocessing in this case if desired, set n_jobs=1 when calling
+        generate_shap_values(). See more details on this function call below.
+        
+        Additionally, there is a pickle error when using multiprocessing with a scikit-learn Voting or
         Stacking model with SHAP. Therefore, no multiprocessing is used in such cases.
         
         At a high level, the library will automatically detect the type of model
         that has been trained (regressor vs. classifier, boosting model vs. other
         model, etc.) and apply the correct handling. If your model is not accurately
         identified by the library, it's easy to specify how it should be handled.
         
@@ -173,14 +178,17 @@
         * DecisionTreeClassifier
         * DecisionTreeRegressor
         * VotingClassifier
         * VotingRegressor
         * StackingClassifier
         * StackingRegressor
         
+        For models cannot detect model qualities, it will fallback to using the
+        Kernel Explainer, which is model agnostic.
+        
         ## CalibratedClassifierCV
         The auto-shap library provides support for scikit-learn's CalibratedClassifierCV.
         This implementation will extract the SHAP values for every base estimator in the
         calibration ensemble. The SHAP values will then be averaged. For details on the
         CalibratedClassifierCV, please go to the
         [documentation](https://scikit-learn.org/stable/modules/generated/sklearn.calibration.CalibratedClassifierCV.html).
         Since we are extracting only the SHAP values for the base estimator, we will miss
```

### Comparing `auto_shap-0.1.1/README.md` & `auto_shap-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 following when using the library.
 
 * The correct type of explainer class must be declared.
 * Our code for extracting SHAP values will be slightly different when we
 have a regression model compared to when we have a classifier.
 * SHAP cannot natively handel scikit-learn's CalibratedClassifierCV, voting models,
 or stacking models.
-* Boosting models often have distinct behavior when it comes to SHAP values.
+* Boosting models often have distinct behavior when it comes to SHAP values. For
+boosting models, auto-shap will employ the SHAP settings to return probabilities.
 
 Likewise, the native SHAP library does not take advantage of multiprocessing.
 The auto-shap library will run SHAP calculations in parallel to speed them
 up when possible! When we are using a Tree or Linear Explainer, we can calculate our
 SHAP values in parallel without issue. The results will be the same compared
 to when we run our calculations on a single core. Such situations are heavily
 tested in tests/tests.py in the
@@ -35,18 +36,22 @@
 especially on small datasets, if we re-run the KernelExplain back-to-back on the
 same data with the same model, we won't get the exact same feature-level attribution,
 though the total attribution will stay the same (which is tested in tests/tests.py).
 The foregoing points can be substantiated by looking at the
 [SHAP documentation](https://shap-lrjball.readthedocs.io/en/latest/generated/shap.KernelExplainer.html#shap.KernelExplainer.shap_values).
 [This article](https://edden-gerber.github.io/shapley-part-2/) discusses the deterministic
 nature of certain SHAP calculations.
+
 In auto-shap, we still employ multiprocessing when using the KernelExplainer, knowing
 that our results would still not be perfectly deterministic even on a single core,
-and by using multiprocessing, we get a nice speed improvement. Additionally, there
-is a pickle error when using multiprocessing with a scikit-learn Voting or
+and by using multiprocessing, we get a nice speed improvement. To turn off
+multiprocessing in this case if desired, set n_jobs=1 when calling
+generate_shap_values(). See more details on this function call below.
+
+Additionally, there is a pickle error when using multiprocessing with a scikit-learn Voting or
 Stacking model with SHAP. Therefore, no multiprocessing is used in such cases.
 
 At a high level, the library will automatically detect the type of model
 that has been trained (regressor vs. classifier, boosting model vs. other
 model, etc.) and apply the correct handling. If your model is not accurately
 identified by the library, it's easy to specify how it should be handled.
 
@@ -165,14 +170,17 @@
 * DecisionTreeClassifier
 * DecisionTreeRegressor
 * VotingClassifier
 * VotingRegressor
 * StackingClassifier
 * StackingRegressor
 
+For models cannot detect model qualities, it will fallback to using the
+Kernel Explainer, which is model agnostic.
+
 ## CalibratedClassifierCV
 The auto-shap library provides support for scikit-learn's CalibratedClassifierCV.
 This implementation will extract the SHAP values for every base estimator in the
 calibration ensemble. The SHAP values will then be averaged. For details on the
 CalibratedClassifierCV, please go to the
 [documentation](https://scikit-learn.org/stable/modules/generated/sklearn.calibration.CalibratedClassifierCV.html).
 Since we are extracting only the SHAP values for the base estimator, we will miss
```

### Comparing `auto_shap-0.1.1/auto_shap/auto_shap.py` & `auto_shap-0.2.0/auto_shap/auto_shap.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,40 +8,37 @@
 
 from auto_shap.utilities import (determine_model_qualities,
                                  make_directories_if_not_exists, make_shap_df,
                                  run_shap_explainer_with_n_jobs,
                                  save_expected_value)
 
 
-def get_shap_expected_value(explainer: callable, boosting_model: bool, linear_model) -> float:
+def get_shap_expected_value(explainer: callable) -> float or np.ndarray:
     """
     Extracts a SHAP Explainer's expected value. For a classifier, this is the mean positive predicted probability.
-    For a regression model, this is the mean predicted value.
+    For a regression model, this is the mean predicted value. If the raw expected value is an array, we will pluck
+    the first or second element based on the length. If the length of the array is more than two, we return the entire
+    raw expected value.
 
     :param explainer: SHAP explainer object
-    :param boosting_model: Boolean of whether or not the explainer is for a boosting model
-    :param linear_model: Boolean of whether or not the explainer is for a linear model
     :returns: SHAP Explainer's expected value
     """
-    if linear_model:
-        expected_value = explainer.expected_value
-    elif boosting_model:
-        try:
-            expected_value = explainer.expected_value[0]
-        except TypeError:
-            expected_value = explainer.expected_value
+    expected_value = explainer.expected_value
+    if isinstance(expected_value, np.ndarray):
+        expected_value_len = len(expected_value)
+        if expected_value_len == 1:
+            return expected_value[0]
+        elif expected_value_len == 2:
+            return expected_value[1]
+        else:
+            return expected_value
+    elif isinstance(expected_value, float):
+        return expected_value
     else:
-        try:
-            expected_value = explainer.expected_value[1]
-        except Exception as e:
-            if str(e) == 'index 1 is out of bounds for axis 0 with size 1':
-                expected_value = explainer.expected_value[0]
-            else:
-                expected_value = explainer.expected_value
-    return expected_value
+        return expected_value
 
 
 def generate_shap_global_values(shap_values: np.array, x_df: pd.DataFrame) -> pd.DataFrame:
     """
     Extracts the global SHAP values for every feature.
 
     :param shap_values: numpy array of shap values
@@ -50,17 +47,17 @@
     """
     shap_values = np.abs(shap_values).mean(0)
     df = pd.DataFrame(list(zip(x_df.columns, shap_values)), columns=['feature', 'shap_value'])
     df.sort_values(by=['shap_value'], ascending=False, inplace=True)
     return df
 
 
-def produce_shap_output_with_kernel_explainer(model: callable, x_df: pd.DataFrame, boosting_model: bool,
-                                              regression_model: bool, linear_model: bool,
-                                              return_df: bool = True, n_jobs: int = None) -> tuple:
+def produce_shap_output_with_agnostic_explainer(model: callable, x_df: pd.DataFrame, boosting_model: bool,
+                                                regression_model: bool, linear_model: bool,
+                                                return_df: bool = True, n_jobs: int = None) -> tuple:
     """
     Using the Kernel Explainer, produces SHAP values and associated output: SHAP values for every row in x_df, the
     expected value from the SHAP explainer, and a dataframe of global SHAP values. Runs the SHAP explainer in parallel
     to increase speed.
 
     :param model: fitted model
     :param x_df: x dataframe
@@ -74,15 +71,15 @@
     and a dataframe of global SHAP values
     """
     if regression_model:
         explainer = shap.KernelExplainer(model.predict, x_df)
     else:
         explainer = shap.KernelExplainer(model.predict_proba, x_df)
     shap_values = run_shap_explainer_with_n_jobs(x_df, explainer, boosting_model, regression_model, linear_model, n_jobs)
-    shap_expected_value = get_shap_expected_value(explainer, boosting_model, linear_model)
+    shap_expected_value = get_shap_expected_value(explainer)
     global_shap_df = generate_shap_global_values(shap_values, x_df)
     if return_df:
         shap_values_df = make_shap_df(shap_values, x_df)
         return shap_values_df, shap_expected_value, global_shap_df
     else:
         return shap_values, shap_expected_value, global_shap_df
 
@@ -102,17 +99,20 @@
     classification model
     :param linear_model: Boolean of whether or not the explainer is for a linear model
     :param return_df: Boolean of whether to return a dataframe; if False, an array is returned
     :param n_jobs: number of cores to use when processing
     :return: tuple with three components: SHAP values (dataframe or array), the expected value from the SHAP explainer,
     and a dataframe of global SHAP values
     """
-    explainer = shap.TreeExplainer(model)
+    if boosting_model and not regression_model:
+        explainer = shap.TreeExplainer(model, model_output='probability', data=x_df)
+    else:
+        explainer = shap.TreeExplainer(model)
     shap_values = run_shap_explainer_with_n_jobs(x_df, explainer, boosting_model, regression_model, False, n_jobs)
-    shap_expected_value = get_shap_expected_value(explainer, boosting_model, linear_model)
+    shap_expected_value = get_shap_expected_value(explainer)
     global_shap_df = generate_shap_global_values(shap_values, x_df)
     if return_df:
         shap_values_df = make_shap_df(shap_values, x_df)
         return shap_values_df, shap_expected_value, global_shap_df
     else:
         return shap_values, shap_expected_value, global_shap_df
 
@@ -132,15 +132,15 @@
     :param return_df: Boolean of whether to return a dataframe; if False, an array is returned
     :param n_jobs: number of cores to use when processing
     :return: tuple with three components: SHAP values (dataframe or array), the expected value from the SHAP explainer,
     and a dataframe of global SHAP values
     """
     explainer = shap.LinearExplainer(model, x_df)
     shap_values = run_shap_explainer_with_n_jobs(x_df, explainer, False, regression_model, True, n_jobs)
-    shap_expected_value = get_shap_expected_value(explainer, False, linear_model)
+    shap_expected_value = get_shap_expected_value(explainer)
     global_shap_df = generate_shap_global_values(shap_values, x_df)
     if return_df:
         shap_values_df = make_shap_df(shap_values, x_df)
         return shap_values_df, shap_expected_value, global_shap_df
     else:
         return shap_values, shap_expected_value, global_shap_df
 
@@ -187,50 +187,50 @@
     shap_values = np.array(shap_values_list).sum(axis=0) / len(shap_values_list)
     shap_expected_value = mean(shap_expected_list)
     global_shap_df = generate_shap_global_values(shap_values, x_df)
     shap_values_df = make_shap_df(shap_values, x_df)
     return shap_values_df, shap_expected_value, global_shap_df
 
 
-def produce_raw_shap_values(model: callable, x_df: pd.DataFrame, use_kernel: bool, linear_model: bool, tree_model: bool,
-                            calibrated_model: bool, boosting_model: bool, regression_model: bool,
+def produce_raw_shap_values(model: callable, x_df: pd.DataFrame, use_agnostic: bool, linear_model: bool,
+                            tree_model: bool, calibrated_model: bool, boosting_model: bool, regression_model: bool,
                             voting_or_stacking_model: bool = False, n_jobs: int = None) -> tuple:
     """
     Produces SHAP output for every observation in x_df: SHAP values for every row in x_df, the expected value from the
     SHAP explainer, and a dataframe of global SHAP values. Runs the SHAP explainer in parallel to increase speed.
-    The appropriate explainer is used based on the boolean function arguments.
+    The appropriate explainer is used based on the boolean function arguments. The Kernel Explainer is used as the
+    fallback option.
 
     :param model: fitted model
     :param x_df: x dataframe
-    :param use_kernel: Boolean of whether or not to use Kernel SHAP
+    :param use_agnostic: Boolean of whether or not to use an agnostic SHAP explainer (i.e., the Kernel Explainer)
     :param linear_model: Boolean of whether model is a linear model, which would employ Linear SHAP
     :param tree_model: Boolean of whether model is a tree-based model, which would employ Tree SHAP
     :param calibrated_model: Boolean of whether or not the model is a CalibratedClassifierCV
     :param boosting_model: Boolean of whether or not the explainer is for a boosting model
     :param regression_model: Boolean of whether or not this is a regression model; if not, it's assumed this is a
     classification model
     :param voting_or_stacking_model: Boolean of whether or not this is a voting or stacking model
     :param n_jobs: number of cores to use when processing
     :return: tuple with three components: dataframe of SHAP values for every row in x_df, the expected value from the
     SHAP explainer, and a dataframe of global SHAP values
     """
-    if use_kernel:
-        return produce_shap_output_with_kernel_explainer(model, x_df, boosting_model, regression_model, linear_model,
-                                                         n_jobs=n_jobs)
-    if voting_or_stacking_model:
-        return produce_shap_output_with_kernel_explainer(model, x_df, boosting_model, regression_model, linear_model,
-                                                         n_jobs=n_jobs)
+    if not any([linear_model, tree_model, calibrated_model, boosting_model, voting_or_stacking_model]):
+        use_agnostic = True
+    if use_agnostic or voting_or_stacking_model:
+        return produce_shap_output_with_agnostic_explainer(model, x_df, boosting_model, regression_model, linear_model,
+                                                           n_jobs=n_jobs)
     else:
         if calibrated_model:
             return produce_shap_output_for_calibrated_classifier(model, x_df, boosting_model, linear_model,
                                                                  n_jobs=n_jobs)
         else:
             if tree_model:
                 return produce_shap_output_with_tree_explainer(model, x_df, boosting_model, regression_model, False,
-                                                       n_jobs=n_jobs)
+                                                               n_jobs=n_jobs)
             elif linear_model:
                 return produce_shap_output_with_linear_explainer(model, x_df, regression_model, True, n_jobs=n_jobs)
 
 
 def generate_shap_summary_plot(shap_values: np.array, x_df: pd.DataFrame, plot_type: str, save_path: str,
                                file_prefix: str = None):
     """
@@ -249,15 +249,15 @@
         file_name = f'{file_prefix}_shap_values_{plot_type}.png'
     plt.savefig(os.path.join(save_path, 'plots', file_name), bbox_inches='tight')
     plt.clf()
 
 
 def generate_shap_values(model: callable, x_df: pd.DataFrame, linear_model: bool = None, tree_model: bool = None,
                          boosting_model: bool = None, calibrated_model: bool = None, regression_model: bool = False,
-                         voting_or_stacking_model: bool = False, use_kernel: bool = False,
+                         voting_or_stacking_model: bool = False, use_agnostic: bool = False,
                          n_jobs: int = None) -> tuple:
     """
     Generates SHAP values for the provided model and x_df. Three pieces of output are generated: dataframe of SHAP
     values for every row in x_df, the expected value from the SHAP explainer, and a dataframe of global SHAP values.
     The function will attempt to use the best explainer for the model (e.g. linear vs. tree). It will also attempt
     to automatically detect if the model is a boosting model, which can require some special handling. Likewise, it
     will work to automatically detect if the model is for classification or regression, which again requires some
@@ -272,36 +272,36 @@
     :param linear_model: Boolean of whether model is a linear model, which would employ Linear SHAP
     :param tree_model: Boolean of whether model is a tree-based model, which would employ Tree SHAP
     :param boosting_model: Boolean of whether or not the explainer is for a boosting model
     :param calibrated_model: Boolean of whether or not the model is a CalibratedClassifierCV
     :param regression_model: Boolean of whether or not this is a regression model; if not, it's assumed this is a
     classification model
     :param voting_or_stacking_model: Boolean of whether or not this is a voting or stacking model
-    :param use_kernel: Boolean of whether or not to use Kernel SHAP
+    :param use_agnostic: Boolean of whether or not to use an agnostic explainer (the Kernel Explainer)
     :param n_jobs: number of cores to use when processing
     :return: tuple with three components: dataframe of SHAP values for every row in x_df, the expected value from the
     SHAP explainer, and a dataframe of global SHAP values
     """
     calibrated_model, linear_model, tree_model, boosting_model, regression_model, voting_or_stacking_model = \
         determine_model_qualities(
             model, linear_model, tree_model, boosting_model, calibrated_model, regression_model,
             voting_or_stacking_model
         )
     shap_values_df, shap_expected_value, global_shap_df = produce_raw_shap_values(
-        model, x_df, use_kernel, linear_model, tree_model, calibrated_model, boosting_model, regression_model,
+        model, x_df, use_agnostic, linear_model, tree_model, calibrated_model, boosting_model, regression_model,
         voting_or_stacking_model, n_jobs
     )
     return shap_values_df, shap_expected_value, global_shap_df
 
 
 def produce_shap_values_and_summary_plots(model: callable, x_df: pd.DataFrame, save_path: str,
-                                          linear_model: bool = None,  tree_model: bool = None,
+                                          linear_model: bool = None, tree_model: bool = None,
                                           boosting_model: bool = None, calibrated_model: bool = None,
                                           regression_model: bool = None, voting_or_stacking_model: bool = False,
-                                          use_kernel: bool = None, file_prefix: str = None, n_jobs: int = None) -> None:
+                                          use_agnostic: bool = None, file_prefix: str = None, n_jobs: int = None) -> None:
     """
     Produces SHAP values for x_df and writes associated diagnostics locally. The following output is saved in
     save_path in appropriate subdirectories: SHAP values for every row in x_df, global SHAP values for every feature
     in x_df, the expected value of the SHAP explainer, bar plot of global SHAP features, and dot plot of SHAP values for
     top features.
 
     The function will attempt to use the best explainer for the model (e.g. linear vs. tree). It will also attempt
@@ -318,15 +318,15 @@
     :param linear_model: Boolean of whether model is a linear model, which would employ Linear SHAP
     :param tree_model: Boolean of whether model is a tree-based model, which would employ Tree SHAP
     :param boosting_model: Boolean of whether or not the explainer is for a boosting model
     :param calibrated_model: Boolean of whether or not the model is a CalibratedClassifierCV
     :param regression_model: Boolean of whether or not this is a regression model; if not, it's assumed this is a
     classification model
     :param voting_or_stacking_model: Boolean of whether or not this is a voting or stacking model
-    :param use_kernel: Boolean of whether or not to use Kernel SHAP
+    :param use_agnostic: Boolean of whether or not to use an agnostic explained (the Kernel Explainer)
     :return: tuple with three components: dataframe of SHAP values for every row in x_df, the expected value from the
     SHAP explainer, and a dataframe of global SHAP values
     :param file_prefix: prefix to add to the file name
     :param n_jobs: number of cores to use when processing
     """
     save_file_path = os.path.join(save_path, 'files')
     save_plots_path = os.path.join(save_path, 'plots')
@@ -335,14 +335,14 @@
             save_path,
             save_file_path,
             save_plots_path,
         ]
     )
     shap_values_df, shap_expected_value, global_shap_df = generate_shap_values(
         model, x_df, linear_model, tree_model, boosting_model, calibrated_model, regression_model,
-        voting_or_stacking_model, use_kernel, n_jobs
+        voting_or_stacking_model, use_agnostic, n_jobs
     )
     shap_values_df.to_csv(os.path.join(save_file_path, 'local_shap_values.csv'), index=False)
     global_shap_df.to_csv(os.path.join(save_file_path, 'global_shap_values.csv'), index=False)
     save_expected_value(shap_expected_value, save_file_path)
     generate_shap_summary_plot(shap_values_df, x_df, 'bar', save_path, file_prefix)
     generate_shap_summary_plot(shap_values_df, x_df, 'dot', save_path, file_prefix)
```

### Comparing `auto_shap-0.1.1/auto_shap/scratch.py` & `auto_shap-0.2.0/auto_shap/scratch.py`

 * *Files identical despite different names*

### Comparing `auto_shap-0.1.1/auto_shap/utilities.py` & `auto_shap-0.2.0/auto_shap/utilities.py`

 * *Files identical despite different names*

### Comparing `auto_shap-0.1.1/auto_shap.egg-info/PKG-INFO` & `auto_shap-0.2.0/auto_shap.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-shap
-Version: 0.1.1
+Version: 0.2.0
 Summary: Calculate SHAP values in parallel and automatically detect what explainer to use
 Home-page: https://github.com/micahmelling/auto-shap
 Author: Micah Melling
 Author-email: micahmelling@gmail.com
 License: MIT
 Description: # auto-shap
         The auto-shap library is your best friend when calculating SHAP values!
@@ -25,15 +25,16 @@
         following when using the library.
         
         * The correct type of explainer class must be declared.
         * Our code for extracting SHAP values will be slightly different when we
         have a regression model compared to when we have a classifier.
         * SHAP cannot natively handel scikit-learn's CalibratedClassifierCV, voting models,
         or stacking models.
-        * Boosting models often have distinct behavior when it comes to SHAP values.
+        * Boosting models often have distinct behavior when it comes to SHAP values. For
+        boosting models, auto-shap will employ the SHAP settings to return probabilities.
         
         Likewise, the native SHAP library does not take advantage of multiprocessing.
         The auto-shap library will run SHAP calculations in parallel to speed them
         up when possible! When we are using a Tree or Linear Explainer, we can calculate our
         SHAP values in parallel without issue. The results will be the same compared
         to when we run our calculations on a single core. Such situations are heavily
         tested in tests/tests.py in the
@@ -43,18 +44,22 @@
         especially on small datasets, if we re-run the KernelExplain back-to-back on the
         same data with the same model, we won't get the exact same feature-level attribution,
         though the total attribution will stay the same (which is tested in tests/tests.py).
         The foregoing points can be substantiated by looking at the
         [SHAP documentation](https://shap-lrjball.readthedocs.io/en/latest/generated/shap.KernelExplainer.html#shap.KernelExplainer.shap_values).
         [This article](https://edden-gerber.github.io/shapley-part-2/) discusses the deterministic
         nature of certain SHAP calculations.
+        
         In auto-shap, we still employ multiprocessing when using the KernelExplainer, knowing
         that our results would still not be perfectly deterministic even on a single core,
-        and by using multiprocessing, we get a nice speed improvement. Additionally, there
-        is a pickle error when using multiprocessing with a scikit-learn Voting or
+        and by using multiprocessing, we get a nice speed improvement. To turn off
+        multiprocessing in this case if desired, set n_jobs=1 when calling
+        generate_shap_values(). See more details on this function call below.
+        
+        Additionally, there is a pickle error when using multiprocessing with a scikit-learn Voting or
         Stacking model with SHAP. Therefore, no multiprocessing is used in such cases.
         
         At a high level, the library will automatically detect the type of model
         that has been trained (regressor vs. classifier, boosting model vs. other
         model, etc.) and apply the correct handling. If your model is not accurately
         identified by the library, it's easy to specify how it should be handled.
         
@@ -173,14 +178,17 @@
         * DecisionTreeClassifier
         * DecisionTreeRegressor
         * VotingClassifier
         * VotingRegressor
         * StackingClassifier
         * StackingRegressor
         
+        For models cannot detect model qualities, it will fallback to using the
+        Kernel Explainer, which is model agnostic.
+        
         ## CalibratedClassifierCV
         The auto-shap library provides support for scikit-learn's CalibratedClassifierCV.
         This implementation will extract the SHAP values for every base estimator in the
         calibration ensemble. The SHAP values will then be averaged. For details on the
         CalibratedClassifierCV, please go to the
         [documentation](https://scikit-learn.org/stable/modules/generated/sklearn.calibration.CalibratedClassifierCV.html).
         Since we are extracting only the SHAP values for the base estimator, we will miss
```

### Comparing `auto_shap-0.1.1/setup.py` & `auto_shap-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="auto_shap",
-    version="0.1.1",
+    version="0.2.0",
     author="Micah Melling",
     author_email="micahmelling@gmail.com",
     description="Calculate SHAP values in parallel and automatically detect what explainer to use",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/micahmelling/auto-shap',
     license="MIT",
```

