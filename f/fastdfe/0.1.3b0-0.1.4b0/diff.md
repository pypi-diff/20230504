# Comparing `tmp/fastdfe-0.1.3b0.tar.gz` & `tmp/fastdfe-0.1.4b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastdfe-0.1.3b0.tar", max compression
+gzip compressed data, was "fastdfe-0.1.4b0.tar", max compression
```

## Comparing `fastdfe-0.1.3b0.tar` & `fastdfe-0.1.4b0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      322 2023-05-02 08:38:16.143704 fastdfe-0.1.3b0/README.md
--rw-r--r--   0        0        0     2590 2023-04-29 07:23:15.706767 fastdfe-0.1.3b0/fastdfe/__init__.py
--rw-r--r--   0        0        0    17303 2023-05-02 08:38:16.179841 fastdfe-0.1.3b0/fastdfe/abstract_inference.py
--rw-r--r--   0        0        0    42920 2023-05-02 08:43:30.818811 fastdfe-0.1.3b0/fastdfe/base_inference.py
--rw-r--r--   0        0        0     4762 2023-04-29 08:09:34.806177 fastdfe-0.1.3b0/fastdfe/bootstrap.py
--rw-r--r--   0        0        0     9585 2023-04-29 08:09:34.816833 fastdfe-0.1.3b0/fastdfe/config.py
--rw-r--r--   0        0        0    15043 2023-04-29 08:10:05.020182 fastdfe-0.1.3b0/fastdfe/discretization.py
--rw-r--r--   0        0        0     3902 2023-04-29 08:09:34.792156 fastdfe-0.1.3b0/fastdfe/json_handlers.py
--rw-r--r--   0        0        0     1541 2023-04-29 08:10:05.029271 fastdfe-0.1.3b0/fastdfe/mle.py
--rw-r--r--   0        0        0    33480 2023-05-02 08:38:16.181798 fastdfe-0.1.3b0/fastdfe/optimization.py
--rw-r--r--   0        0        0    21091 2023-05-02 08:38:16.182403 fastdfe-0.1.3b0/fastdfe/parametrization.py
--rw-r--r--   0        0        0    11316 2023-04-29 08:12:55.242293 fastdfe-0.1.3b0/fastdfe/parser.py
--rw-r--r--   0        0        0    12467 2023-05-02 08:38:16.183198 fastdfe-0.1.3b0/fastdfe/polydfe.py
--rw-r--r--   0        0        0     5254 2023-04-29 07:57:26.449161 fastdfe-0.1.3b0/fastdfe/polydfe_utils.py
--rw-r--r--   0        0        0    36485 2023-05-02 08:49:18.285827 fastdfe-0.1.3b0/fastdfe/shared_inference.py
--rw-r--r--   0        0        0    17957 2023-04-28 16:01:50.245576 fastdfe-0.1.3b0/fastdfe/spectrum.py
--rw-r--r--   0        0        0    30684 2023-05-02 08:38:16.185031 fastdfe-0.1.3b0/fastdfe/visualization.py
--rw-r--r--   0        0        0      642 2023-05-02 08:50:43.544962 fastdfe-0.1.3b0/pyproject.toml
--rw-r--r--   0        0        0     1347 1970-01-01 00:00:00.000000 fastdfe-0.1.3b0/PKG-INFO
+-rw-r--r--   0        0        0      322 2023-05-02 08:38:16.143704 fastdfe-0.1.4b0/README.md
+-rw-r--r--   0        0        0     2603 2023-05-04 15:03:08.858314 fastdfe-0.1.4b0/fastdfe/__init__.py
+-rw-r--r--   0        0        0    18451 2023-05-04 14:38:07.386884 fastdfe-0.1.4b0/fastdfe/abstract_inference.py
+-rw-r--r--   0        0        0    44975 2023-05-04 14:38:07.369531 fastdfe-0.1.4b0/fastdfe/base_inference.py
+-rw-r--r--   0        0        0     4762 2023-04-29 08:09:34.806177 fastdfe-0.1.4b0/fastdfe/bootstrap.py
+-rw-r--r--   0        0        0     9934 2023-05-03 08:58:25.701024 fastdfe-0.1.4b0/fastdfe/config.py
+-rw-r--r--   0        0        0    15051 2023-05-02 14:22:16.509178 fastdfe-0.1.4b0/fastdfe/discretization.py
+-rw-r--r--   0        0        0     3902 2023-04-29 08:09:34.792156 fastdfe-0.1.4b0/fastdfe/json_handlers.py
+-rw-r--r--   0        0        0     1541 2023-04-29 08:10:05.029271 fastdfe-0.1.4b0/fastdfe/mle.py
+-rw-r--r--   0        0        0    35979 2023-05-04 07:31:00.022451 fastdfe-0.1.4b0/fastdfe/optimization.py
+-rw-r--r--   0        0        0    21091 2023-05-02 08:38:16.182403 fastdfe-0.1.4b0/fastdfe/parametrization.py
+-rw-r--r--   0        0        0    11316 2023-04-29 08:12:55.242293 fastdfe-0.1.4b0/fastdfe/parser.py
+-rw-r--r--   0        0        0    12467 2023-05-02 08:38:16.183198 fastdfe-0.1.4b0/fastdfe/polydfe.py
+-rw-r--r--   0        0        0     5254 2023-04-29 07:57:26.449161 fastdfe-0.1.4b0/fastdfe/polydfe_utils.py
+-rw-r--r--   0        0        0    40670 2023-05-04 14:38:07.348375 fastdfe-0.1.4b0/fastdfe/shared_inference.py
+-rw-r--r--   0        0        0    17957 2023-04-28 16:01:50.245576 fastdfe-0.1.4b0/fastdfe/spectrum.py
+-rw-r--r--   0        0        0    30801 2023-05-02 11:01:44.227968 fastdfe-0.1.4b0/fastdfe/visualization.py
+-rw-r--r--   0        0        0      642 2023-05-04 15:03:08.851472 fastdfe-0.1.4b0/pyproject.toml
+-rw-r--r--   0        0        0     1347 1970-01-01 00:00:00.000000 fastdfe-0.1.4b0/PKG-INFO
```

### Comparing `fastdfe-0.1.3b0/fastdfe/__init__.py` & `fastdfe-0.1.4b0/fastdfe/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 fastDFE package.
 """
 
 __author__ = "Janek Sendrowski"
 __contact__ = "sendrowski.janek@gmail.com"
 __date__ = "2023-03-10"
 
-__version__ = 'beta'
+__version__ = '0.1.4-beta'
 
 import logging
 import sys
 import warnings
 
 import jsonpickle
 import numpy as np
@@ -28,15 +28,15 @@
 # configure logger
 logger = logging.getLogger('fastdfe')
 handler = logging.StreamHandler(sys.stdout)
 handler.setFormatter(logging.Formatter('%(levelname)s:%(name)s:%(message)s'))
 logger.addHandler(handler)
 logger.setLevel(logging.INFO)
 
-# whether to show progress bar
+# whether to disable the progress bar
 disable_pbar = False
 
 
 def raise_on_warning(message, category, filename, lineno, file=None, line=None):
     """
     Raise exception on warning.
     """
```

### Comparing `fastdfe-0.1.3b0/fastdfe/abstract_inference.py` & `fastdfe-0.1.4b0/fastdfe/abstract_inference.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,19 +178,59 @@
         :return: Axes of the plot.
         :raises ValueError: If no inference objects are given.
         """
         if len(inferences) == 0:
             raise ValueError('No inference objects given.')
 
         # get sorted list of parameter names
-        param_names = sorted(inferences[0].get_bootstrap_param_names())
+        param_names = sorted(list(inferences[0].get_bootstrap_param_names()))
 
-        if labels is None:
-            labels = list()
+        # get errors and values
+        errors, values = Inference.get_errors_and_values(
+            bootstrap_type=bootstrap_type,
+            ci_level=ci_level,
+            confidence_intervals=confidence_intervals,
+            inferences=inferences,
+            labels=labels,
+            param_names=param_names
+        )
+
+        return Visualization.plot_inferred_parameters(
+            values=values,
+            errors=errors,
+            param_names=param_names,
+            file=file,
+            show=show,
+            title=title,
+            labels=labels,
+            scale=scale,
+            legend=len(labels) > 1,
+            ax=ax
+        )
 
+    @staticmethod
+    def get_errors_and_values(
+            bootstrap_type: Literal['percentile', 'bca'],
+            ci_level: float,
+            confidence_intervals: bool,
+            inferences: List['AbstractInference'],
+            labels: list | np.ndarray,
+            param_names: list | np.ndarray
+    ):
+        """
+        Get errors and values for inferences.
+
+        :param bootstrap_type: Type of bootstrap to use.
+        :param ci_level: Confidence level for confidence intervals.
+        :param confidence_intervals: Whether to compute confidence intervals.
+        :param inferences: List of inference objects.
+        :param labels: Labels for the inferences.
+        :param param_names: Names of the parameters to get errors and values for.
+        :return: dictionary of errors and dictionary of values
+        """
         errors = {}
         values = {}
         for label, inf in zip(labels, inferences):
 
             values[label] = list(inf.get_bootstrap_params()[k] for k in param_names)
 
             # whether to compute errors
@@ -206,26 +246,15 @@
                     bs=inf.bootstraps[param_names].to_numpy(),
                     bootstrap_type=bootstrap_type,
                     ci_level=ci_level
                 )
             else:
                 errors[label] = None
 
-        return Visualization.plot_inferred_parameters(
-            values=values,
-            errors=errors,
-            param_names=param_names,
-            file=file,
-            show=show,
-            title=title,
-            labels=labels,
-            scale=scale,
-            legend=len(labels) > 1,
-            ax=ax
-        )
+        return errors, values
 
     @staticmethod
     def get_discretized(
             bootstraps: pd.DataFrame,
             params: dict,
             model: Parametrization,
             intervals: np.ndarray = np.array([-np.inf, -100, -10, -1, 0, 1, np.inf]),
```

### Comparing `fastdfe-0.1.3b0/fastdfe/base_inference.py` & `fastdfe-0.1.4b0/fastdfe/base_inference.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import copy
 import functools
 import itertools
 import json
 import logging
 import time
-from typing import List, Optional, Dict, Literal, cast
+from typing import List, Optional, Dict, Literal, cast, Tuple
 
 import jsonpickle
 import multiprocess as mp
 import numpy as np
 import pandas as pd
 from matplotlib import pyplot as plt
 from numpy.linalg import norm
@@ -25,15 +25,15 @@
 from typing_extensions import Self
 
 from . import parametrization, optimization
 from .abstract_inference import AbstractInference, Inference
 from .config import Config
 from .discretization import Discretization
 from .json_handlers import CustomEncoder
-from .optimization import Optimization, flatten_dict, pack_params, expand_fixed, scale_values
+from .optimization import Optimization, flatten_dict, pack_params, expand_fixed, scale_values, unpack_shared
 from .parametrization import Parametrization, from_string
 from .spectrum import Spectrum, Spectra
 from .spectrum import standard_kingman
 from .visualization import Visualization
 
 # get logger
 logger = logging.getLogger('fastdfe')
@@ -42,15 +42,14 @@
 class BaseInference(AbstractInference):
     """
     Base inference class for inferring the SFS given one neutral and one selected SFS.
     Note that BaseInference is by default seeded.
 
     .. warning::
         TODO add confidence intervals for inferred SFS.
-        TODO take average of likelihood after bootstrapping?
     """
 
     #: Default parameters not connected to the DFE parametrization
     default_x0 = dict(
         eps=0.0
     )
 
@@ -77,15 +76,16 @@
             intervals_del: (float, float, int) = (-1.0e+8, -1.0e-5, 1000),
             intervals_ben: (float, float, int) = (1.0e-5, 1.0e4, 1000),
             integration_mode: Literal['midpoint', 'quad'] = 'midpoint',
             linearized: bool = True,
             model: Parametrization | str = 'GammaExpParametrization',
             seed: int = 0,
             x0: Dict[str, Dict[str, float]] = {},
-            bounds: Dict[str, tuple] = {},
+            bounds: Dict[str, Tuple[float, float]] = {},
+            scales: Dict[str, Literal['lin', 'log', 'symlog']] = {},
             loss_type: Literal['likelihood', 'L2'] = 'likelihood',
             opts_mle: dict = {},
             n_runs: int = 10,
             fixed_params: Dict[str, Dict[str, float]] = {},
             do_bootstrap: bool = False,
             n_bootstraps: int = 100,
             parallelize: bool = True,
@@ -95,24 +95,25 @@
             **kwargs
     ):
         """
         Create BaseInference instance.
 
         :param sfs_neut: The neutral SFS. Spectra | Spectrum
         :param sfs_sel: The selected SFS.
-        :param intervals_del: (start, stop, n_interval) for deleterious population-scaled
+        :param intervals_del: ``(start, stop, n_interval)`` for deleterious population-scaled
         selection coefficients. The intervals will be log10-spaced.
         :param intervals_ben: Same as for intervals_del but for beneficial selection coefficients.
         :param model: Instance of DFEParametrization which parametrized the DFE
         :param seed: Seed for the random number generator.
-        :param x0: Initial values for the optimization.
-        :param bounds: Bounds for the optimization.
+        :param x0: Dictionary of initial values in the form {'all': {param: value}}
+        :param bounds: Bounds for the optimization in the form {param: (lower, upper)}
+        :param scales: Scales for the optimization in the form {param: scale}
         :param loss_type: Type of loss function to use for optimization.
         :param opts_mle: Options for the optimization.
-        :param n_runs: Number of optimization runs.
+        :param n_runs: Number of optimization runs. The first run will use the initial values if provided.
         :param fixed_params: Fixed parameters for the optimization.
         :param do_bootstrap: Whether to do bootstrapping.
         :param n_bootstraps: Number of bootstraps.
         :param parallelize: Whether to parallelize the bootstrapping.
         :param discretization: Discretization instance. Mainly intended for internal use.
         :param optimization: Optimization instance. Mainly intended for internal use.
         :param locked: Whether to lock the instance.
@@ -156,30 +157,33 @@
         else:
             # otherwise assign instance
             self.discretization: Discretization = discretization
 
         #: Estimate of theta from neutral SFS
         self.theta: float = self.sfs_neut.theta
 
-        #: MLE params
+        #: MLE estimates of the initial optimization
         self.params_mle: Optional[Dict[str, float]] = None
 
         #: Modelled MLE SFS
         self.sfs_mle: Optional[Spectrum] = None
 
-        #: Likelihood of the MLE
+        #: Likelihood of the MLE, this value may be updated after bootstrapping
         self.likelihood: Optional[float] = None
 
+        #: Likelihoods of the different ML runs, controlled by ``n_runs``
+        self.likelihoods: Optional[List[float]] = None
+
         #: Number of MLE runs to perform
         self.n_runs: int = n_runs
 
         #: Numerical optimization result
         self.result: Optional[OptimizeResult] = None
 
-        # bootstrap options
+        # Bootstrap options
 
         #: Whether to do bootstrapping
         self.do_bootstrap: bool = do_bootstrap
 
         #: Number of bootstraps
         self.n_bootstraps: int = n_bootstraps
 
@@ -189,23 +193,26 @@
         # expand 'all' type
         #: Fixed parameters
         self.fixed_params: Dict[str, Dict[str, float]] = expand_fixed(fixed_params, ['all'])
 
         # check that the fixed parameters are valid
         self.check_fixed_params_exist()
 
-        #: scale for all parameters
-        self.scales = self.model.scales | self.default_scales
+        #: parameter scales
+        self.scales: Dict[str, Literal['lin', 'log', 'symlog']] = self.model.scales | self.default_scales | scales
+
+        #: parameter bounds
+        self.bounds: Dict[str, Tuple[float, float]] = self.model.bounds | self.default_bounds | bounds
 
         if optimization is None:
             # create optimization instance
             # merge with default values of inference and model
             #: Optimization instance
             self.optimization: Optimization = Optimization(
-                bounds=self.model.bounds | self.default_bounds | bounds,
+                bounds=self.bounds,
                 scales=self.scales,
                 opts_mle=self.default_opts_mle | opts_mle,
                 loss_type=loss_type,
                 param_names=self.param_names,
                 parallelize=self.parallelize,
                 fixed_params=fixed_params,
                 seed=seed
@@ -345,19 +352,26 @@
         # performed in each thread.
         _ = self.discretization.dfe_to_sfs
 
         # perform numerical minimization
         result, params_mle = self.optimization.run(
             x0=self.x0,
             scales=self.scales,
+            bounds=self.bounds,
             get_counts=self.get_counts(),
             n_runs=self.n_runs,
             pbar=pbar
         )
 
+        # assign likelihoods
+        self.likelihoods = self.optimization.likelihoods
+
+        # unpack shared parameters
+        params_mle = unpack_shared(params_mle)
+
         # normalize parameters
         params_mle['all'] = self.model.normalize(params_mle['all'])
 
         # assign optimization result and MLE parameters
         self.assign_result(result, params_mle['all'])
 
         # report on optimization result
@@ -524,38 +538,44 @@
 
         # add estimates for alpha to the bootstraps
         self.add_alpha_to_bootstraps()
 
         # add execution time
         self.execution_time += time.time() - start_time
 
-        # determine average likelihood of successful runs
+        # assign average likelihood of successful runs
         if update_likelihood:
             self.likelihood = np.mean([-res.fun for res in result[:, 0] if res.success] + [self.likelihood])
 
         return self.bootstraps
 
     def add_alpha_to_bootstraps(self):
         """
         Add estimates for alpha to the bootstraps.
         """
         logger.debug('Computing estimates for alpha.')
 
         # add alpha estimates
         self.bootstraps['alpha'] = self.bootstraps.apply(lambda r: self.get_alpha(dict(r)), axis=1)
 
-    def resample_sfs(self, sfs: Spectrum) -> Spectrum:
+    def resample_sfs(self, sfs: Spectrum, seed: int = None) -> Spectrum:
         """
         Resample SFS assuming independent Poisson counts.
 
         :param sfs: Spectrum to resample.
+        :param seed: Seed for random number generator.
         :return: Resampled spectrum.
         """
+        if seed is not None:
+            rng = np.random.default_rng(seed=seed)
+        else:
+            rng = self.rng
+
         # resample polymorphic sites only
-        polymorphic = self.rng.poisson(lam=sfs.polymorphic)
+        polymorphic = rng.poisson(lam=sfs.polymorphic)
 
         return Spectrum.from_polydfe(
             polymorphic=polymorphic,
             n_sites=sfs.n_sites,
             n_div=sfs.n_div
         )
 
@@ -563,48 +583,67 @@
         """
         Resample the observed selected SFS and rerun the optimization procedure.
         We take the MLE params as initial params here.
 
         :param seed: Seed for random number generator.
         :return: Optimization result and MLE parameters.
         """
-        if seed is not None:
-            self.rng = np.random.default_rng(seed=seed)
-
         # resample spectra
-        sfs_sel = self.resample_sfs(self.sfs_sel)
-        sfs_neut = self.resample_sfs(self.sfs_neut)
+        sfs_sel = self.resample_sfs(self.sfs_sel, seed=seed)
+        sfs_neut = self.resample_sfs(self.sfs_neut, seed=seed)
 
         # perform numerical minimization
         result, params_mle = self.optimization.run(
             x0=dict(all=self.params_mle),
             scales=self.get_scales_linear(),
+            bounds=self.get_bounds_linear(),
             n_runs=1,
             debug_iterations=False,
             print_info=False,
             get_counts=dict(all=lambda params: self.model_sfs(
                 params,
                 sfs_neut=sfs_neut,
                 sfs_sel=sfs_sel
             ))
         )
 
+        # unpack shared parameters
+        params_mle = unpack_shared(params_mle)
+
         # normalize MLE estimates
         params_mle['all'] = self.model.normalize(params_mle['all'])
 
         return result, params_mle
 
     def get_scales_linear(self) -> Dict[str, Literal['lin']]:
         """
         Get linear scales for all parameters. We do this for the bootstraps as x0 should be close to MLE.
 
         :return: Dictionary of scales.
         """
         return cast(Dict[str, Literal['lin']], dict((p, 'lin') for p in self.scales.keys()))
 
+    def get_bounds_linear(self) -> Dict[str, Tuple[float, float]]:
+        """
+        Get linear bounds for all parameters. We do this for the bootstraps as x0 should be close to MLE.
+
+        :return: Dictionary of bounds.
+        """
+        scaled_bounds = {}
+
+        for key, bounds in self.bounds.items():
+
+            # for symlog we need to convert the bounds to linear scale
+            if self.scales[key] == 'symlog':
+                scaled_bounds[key] = (-bounds[1], bounds[1])
+            else:
+                scaled_bounds[key] = bounds
+
+        return scaled_bounds
+
     def model_sfs(self, params: dict, sfs_neut: Spectrum, sfs_sel: Spectrum) -> (np.ndarray, np.ndarray):
         """
         Model the selected SFS from the given parameters.
 
         :param sfs_sel: Observed spectrum of selected sites.
         :param sfs_neut: Observed spectrum of neutral sites.
         :param params: Dictionary of parameters.
@@ -933,15 +972,15 @@
         :param title: Plot title.
         :param file: File to save plot to.
         :param show: Whether to show plot.
         :param ax: Axes object to plot on.
         :return: Axes object
         """
         return Visualization.plot_likelihoods(
-            likelihoods=self.optimization.likelihoods,
+            likelihoods=self.likelihoods,
             file=file,
             show=show,
             title=title,
             scale=scale,
             ax=ax
         )
 
@@ -984,19 +1023,20 @@
         else:
             return None
 
         return self.lrt(self.likelihood, complex.likelihood, d)
 
     @run_if_required_wrapper
     @functools.lru_cache
-    def compare_nested_models(self) -> (np.ndarray, Dict[str, 'BaseInference']):
+    def compare_nested_models(self, do_bootstrap: bool = True) -> (np.ndarray, Dict[str, 'BaseInference']):
         """
         Compare the various nested versions of the specified
         model using likelihood ratio tests.
 
+        :param do_bootstrap: Whether to perform bootstrapping. This is recommended to get more accurate p-values.
         :return: Matrix of p-values, dict of base inference objects
         """
 
         # get sub-model specifications
         submodels_dfe = from_string(self.model).submodels
         submodels_outer = dict(
             no_anc=dict(eps=0),
@@ -1006,15 +1046,15 @@
         # take outer product to get fixed parameters for each model
         inferences: Dict[str, BaseInference] = {}
         for p in itertools.product(submodels_dfe.keys(), submodels_outer.keys()):
             # create deep copy of object
             inference = copy.deepcopy(self)
 
             # disable bootstraps
-            inference.do_bootstrap = False
+            inference.do_bootstrap = do_bootstrap
 
             # dict of params to be fixed
             params = dict(all=submodels_dfe[p[0]] | submodels_outer[p[1]])
 
             # assign fixed parameters
             inference.set_fixed_params(params)
 
@@ -1049,30 +1089,32 @@
             file: str = None,
             show: bool = True,
             remove_empty: bool = False,
             transpose: bool = False,
             cmap: str = None,
             title: str = 'nested model comparison',
             ax: plt.Axes = None,
+            do_bootstrap: bool = True
 
     ) -> plt.Axes:
         """
         Plot the p-values of nested likelihoods.
 
         :param file: File to save plot to.
         :param show: Whether to show plot.
         :param remove_empty: Whether to remove empty rows and columns.
         :param transpose: Whether to transpose the matrix.
         :param cmap: Colormap to use.
         :param title: Plot title.
         :param ax: Axes object to plot on.
+        :param do_bootstrap: Whether to perform bootstrapping. This is recommended to get more accurate p-values.
         :return: Axes object
         """
         # get p-values and names
-        P, inferences = self.compare_nested_models()
+        P, inferences = self.compare_nested_models(do_bootstrap=do_bootstrap)
 
         # define labels
         labels_x = np.array(list(inferences.keys()))
         labels_y = np.array(list(inferences.keys()))
 
         if remove_empty:
             # remove empty columns
@@ -1115,15 +1157,15 @@
     @functools.cached_property
     def alpha(self) -> float:
         """
         Cache alpha, the proportion of beneficial non-synonymous substitutions.
         """
         return self.get_alpha()
 
-    def get_bootstrap_params(self) -> dict:
+    def get_bootstrap_params(self) -> Dict[str, float]:
         """
         Get the parameters to be included in the bootstraps.
 
         :return: Parameters to be included in the bootstraps.
         """
         return self.params_mle | dict(alpha=self.alpha)
 
@@ -1163,17 +1205,20 @@
             sfs_sel=Spectra.from_spectrum(self.sfs_sel),
             intervals_ben=self.discretization.intervals_ben,
             intervals_del=self.discretization.intervals_del,
             integration_mode=self.discretization.integration_mode,
             linearized=self.discretization.linearized,
             model=self.model.__class__.__name__,
             seed=self.seed,
-            opts_mle=self.optimization.opts_mle,
             x0=self.x0,
-            bounds=self.optimization.bounds,
+            bounds=self.bounds,
+            scales=self.scales,
+            loss_type=self.optimization.loss_type,
+            opts_mle=self.optimization.opts_mle,
+            n_runs=self.n_runs,
             fixed_params=self.fixed_params,
             do_bootstrap=self.do_bootstrap,
             n_bootstraps=self.n_bootstraps,
             parallelize=self.parallelize
         )
 
     @classmethod
```

### Comparing `fastdfe-0.1.3b0/fastdfe/bootstrap.py` & `fastdfe-0.1.4b0/fastdfe/bootstrap.py`

 * *Files identical despite different names*

### Comparing `fastdfe-0.1.3b0/fastdfe/config.py` & `fastdfe-0.1.4b0/fastdfe/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 __author__ = "Janek Sendrowski"
 __contact__ = "sendrowski.janek@gmail.com"
 __date__ = "2023-02-26"
 
 import json
 import logging
-from typing import List, Literal, Dict
+from typing import List, Literal, Dict, Tuple
 
 import yaml
 
 from .json_handlers import CustomEncoder
 from .optimization import Covariate
 from .optimization import SharedParams, merge_dicts
 from .parametrization import Parametrization, from_string, to_string
@@ -38,15 +38,16 @@
             intervals_del: (float, float, int) = (-1.0e+8, -1.0e-5, 1000),
             intervals_ben: (float, float, int) = (1.0e-5, 1.0e4, 1000),
             integration_mode: Literal['midpoint', 'quad'] = 'midpoint',
             linearized: bool = True,
             model: Parametrization | str = 'GammaExpParametrization',
             seed: int = 0,
             x0: Dict[str, Dict[str, float]] = {},
-            bounds: Dict[str, tuple] = {},
+            bounds: Dict[str, Tuple[float, float]] = {},
+            scales: Dict[str, Literal['lin', 'log', 'symlog']] = {},
             loss_type: Literal['likelihood', 'L2'] = 'likelihood',
             opts_mle: dict = {},
             n_runs: int = 10,
             fixed_params: Dict[str, Dict[str, float]] = {},
             shared_params: List[SharedParams] = [],
             covariates: List[Covariate] = [],
             do_bootstrap: bool = False,
@@ -63,19 +64,21 @@
         :param sfs_sel: Selected SFS.
         :param intervals_del: Integration intervals for deleterious mutations in log space.
         :param intervals_ben: Integration intervals for beneficial mutations in log space.
         :param integration_mode: Integration mode.
         :param linearized: Whether to use the linearized version of the DFE.
         :param model: Parametrization of the DFE.
         :param seed: Seed for the random number generator.
-        :param x0: Initial parameters for the optimization.
-        :param bounds: Bounds for the optimization.
+        :param x0: Dictionary of initial values in the form ``{type: {param: value}}``
+        :param bounds: Bounds for the optimization in the form {param: (lower, upper)}
+        :param scales: Scales for the optimization in the form {param: scale}
         :param loss_type: Loss function to use.
         :param opts_mle: Options for the optimization.
-        :param n_runs: Number of optimization runs.
+        :param n_runs: Number of optimization runs. Number of optimization runs.
+        The first run will use the initial values if provided.
         :param fixed_params: Fixed parameters for the optimization.
         :param shared_params: Shared parameters for the optimization.
         :param covariates: Covariates for the optimization.
         :param do_bootstrap: Whether to do bootstrapping automatically.
         :param n_bootstraps: Number of bootstraps.
         :param parallelize: Whether to parallelize the optimization.
         """
@@ -88,14 +91,15 @@
             integration_mode=integration_mode,
             linearized=linearized,
             seed=seed,
             opts_mle=opts_mle,
             n_runs=n_runs,
             x0=x0,
             bounds=bounds,
+            scales=scales,
             fixed_params=fixed_params,
             shared_params=shared_params,
             covariates=covariates,
             sfs_neut=sfs_neut,
             sfs_sel=sfs_sel,
             do_bootstrap=do_bootstrap,
             n_bootstraps=n_bootstraps,
```

### Comparing `fastdfe-0.1.3b0/fastdfe/discretization.py` & `fastdfe-0.1.4b0/fastdfe/discretization.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,16 +206,16 @@
             integration_mode: Literal['midpoint', 'quad'] = 'midpoint',
             linearized: bool = True
     ):
         """
         Create Discretization instance.
 
         :return: Number of individuals
-        :param intervals_del: (start, stop, n_interval) for deleterious population-scaled selection coefficients.
-        :param intervals_ben: (start, stop, n_interval) for beneficial population-scaled selection coefficients.
+        :param intervals_del: ``(start, stop, n_interval)`` for deleterious population-scaled selection coefficients.
+        :param intervals_ben: ``(start, stop, n_interval)`` for beneficial population-scaled selection coefficients.
         :param integration_mode : 'midpoint' or 'quad' for midpoint integration or Scipy's quad method.
         :return: Whether to linearize the integral
         """
         self.n = n
 
         # make sure lower bounds are lower than upper bounds
         if not intervals_del[0] < intervals_del[1] or not intervals_ben[0] < intervals_ben[1]:
```

### Comparing `fastdfe-0.1.3b0/fastdfe/json_handlers.py` & `fastdfe-0.1.4b0/fastdfe/json_handlers.py`

 * *Files identical despite different names*

### Comparing `fastdfe-0.1.3b0/fastdfe/mle.py` & `fastdfe-0.1.4b0/fastdfe/mle.py`

 * *Files identical despite different names*

### Comparing `fastdfe-0.1.3b0/fastdfe/optimization.py` & `fastdfe-0.1.4b0/fastdfe/optimization.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import logging
 from dataclasses import dataclass
 from typing import Callable, List, Dict, Literal, Tuple, Optional
 
 import multiprocess as mp
 import numpy as np
 from numpy.linalg import norm
+from numpy.random import Generator
 from scipy.optimize import minimize, OptimizeResult
 from scipy.stats import loguniform, uniform
 from tqdm import tqdm
 
 from .mle import MLE
 
 # get logger
@@ -235,15 +236,15 @@
 def expand_fixed(
         fixed_params: Dict[str, Dict[str, float]],
         types: List[str]
 ) -> Dict[str, Dict[str, float]]:
     """
     Expand 'all' type for shared parameters.
 
-    :param fixed_params: Dictionary of fixed parameters
+    :param fixed_params: Dictionary of fixed parameters indexed by type and parameter
     :param types: List of types
     :return: Expanded dictionary of fixed parameters
     """
     expanded = {}
 
     # loop through fixed parameters
     for key_type, params in fixed_params.items():
@@ -257,14 +258,41 @@
 
             for param, value in params.items():
                 expanded[t][param] = value
 
     return expanded
 
 
+def collapse_fixed(
+        expanded_params: Dict[str, Dict[str, float]],
+        types: List[str]
+) -> Dict[str, Dict[str, float]]:
+    """
+    Collapse expanded fixed parameters to 'all' type if all types have the same fixed parameter.
+
+    :param expanded_params: Expanded dictionary of fixed parameters
+    :param types: List of types
+    :return: Collapsed dictionary of fixed parameters
+    """
+    all_params = {param: [] for params in expanded_params.values() for param in params}
+
+    # Collect parameter values for all types
+    for params in expanded_params.values():
+        for param, value in params.items():
+            all_params[param].append(value)
+
+    # Calculate the mean and check if parameters can be collapsed
+    collapsed = {}
+    for param, values in all_params.items():
+        if len(values) == len(types):
+            collapsed[param] = np.mean(values)
+
+    return {'all': collapsed} if len(collapsed) > 0 else expanded_params
+
+
 def merge_dicts(dict1: dict, dict2: dict) -> dict:
     """
     Merge two dictionaries recursively.
 
     :param dict1: First dictionary
     :param dict2: Second dictionary
     :return: Merged dictionary
@@ -284,41 +312,68 @@
         else:
             # simply assign the value from dict2 to the result dictionary
             result[key] = value
 
     return result
 
 
-def correct_values(params: Dict[str, float], bounds: Dict[str, tuple], warn: bool = False) -> Dict[str, float]:
+def correct_values(
+        params: Dict[str, float],
+        bounds: Dict[str, Tuple[float, float]],
+        scales: Dict[str, Literal['lin', 'log', 'symlog']],
+        warn: bool = False
+) -> Dict[str, float]:
     """
     Correct initial values so that they are within the specified bounds.
 
     :param bounds: Dictionary of bounds
-    :param params: Dictionary of initial values
+    :param params: Flattened dictionary of parameters
+    :param scales: Dictionary of scales
     :param warn: Whether to warn if values are corrected
     :return: Corrected dictionary
     """
-    # create a copy of x0
+    # create a copy of params
     corrected = params.copy()
 
     for key, value in params.items():
         # get base name
         name = key.split('.')[-1]
 
-        if value < bounds[name][0]:
-            corrected[key] = bounds[name][0]
-        elif value > bounds[name][1]:
-            corrected[key] = bounds[name][1]
+        # get real bounds
+        bound = get_real_bounds(bounds[name], scale=scales[name])
 
-    if corrected != params and warn:
-        logger.warning(f'Given initial values outside bounds. Adjusting {params} to {corrected}.')
+        # correct value if outside bounds
+        if value < bound[0]:
+            corrected[key] = bound[0]
+        elif value > bound[1]:
+            corrected[key] = bound[1]
+
+    # differences between the original and corrected dictionaries
+    differences = {key: f"{params[key]} -> {corrected[key]}" for key in params if params[key] != corrected[key]}
+
+    # warn if there are differences
+    if differences and warn:
+        logger.warning(f'Given initial values outside bounds. Adjusting {differences}.')
 
     return corrected
 
 
+def get_real_bounds(bounds: Tuple[float, float], scale: Literal['lin', 'log', 'symlog']) -> Tuple[float, float]:
+    """
+    Get real bounds from the given bounds.
+
+    :param bounds:
+    :return:
+    """
+    if scale == 'symlog':
+        return -bounds[1], bounds[1]
+
+    return bounds
+
+
 def evaluate_counts(get_counts: dict, params: dict):
     """
     Evaluate counts using the given parameters.
     Here we assign the parameters to the appropriate types
     obtaining the counts for each type.
 
     :param get_counts: Dictionary of functions to evaluate counts for each type
@@ -646,15 +701,15 @@
 class Optimization:
     """
     Class for optimizing the DFE.
     """
 
     def __init__(
             self,
-            bounds: Dict[str, tuple],
+            bounds: Dict[str, Tuple[float, float]],
             param_names: List[str],
             loss_type: Literal['likelihood', 'L2'] = 'likelihood',
             opts_mle: dict = {},
             parallelize: bool = True,
             fixed_params: Dict[str, Dict[str, float]] = {},
             scales: Dict[str, Literal['lin', 'log', 'symlog']] = {},
             seed: int = None
@@ -675,15 +730,15 @@
 
         self.opts_mle = opts_mle
         self.loss_type = loss_type
 
         self.fixed_params = flatten_dict(fixed_params)
 
         # check if fixed parameters are within the specified bounds
-        if correct_values(self.fixed_params, self.bounds, warn=False) != self.fixed_params:
+        if correct_values(self.fixed_params, self.bounds, warn=False, scales=scales) != self.fixed_params:
             raise ValueError('Fixed parameters are outside the specified bounds. '
                              f'Fixed params: {self.fixed_params}, bounds: {self.bounds}.')
 
         self.param_names = param_names
         self.parallelize = parallelize
 
         # the initial values
@@ -699,36 +754,44 @@
         self.rng = np.random.default_rng(seed=seed)
 
     def run(
             self,
             get_counts: Dict[str, Callable],
             x0: Dict[str, Dict[str, float]] = {},
             scales: Dict[str, Literal['lin', 'log', 'symlog']] = {},
+            bounds: Dict[str, Tuple[float, float]] = {},
             n_runs: int = 1,
             debug_iterations: bool = True,
             print_info: bool = True,
             pbar: bool = None
     ) -> (OptimizeResult, dict):
         """
         Perform the optimization procedure.
 
         :param scales: Scales of the parameters
+        :param bounds: Bounds of the parameters
         :param pbar: Whether to show a progress bar
         :param print_info: Whether to inform the user about the bounds
-        :param n_runs: Number of optimization runs
-        :param x0: Dictionary of initial values
+        :param n_runs: Number of optimization runs. Number of optimization runs. The first run will use the
+        initial values if provided.
+        :param x0: Dictionary of initial values in the form ``{type: {param: value}}``
         :param get_counts: Dictionary of functions to evaluate counts for each type
         :param debug_iterations: Whether to print debug messages for each iteration
         :return: The optimization result and the likelihoods
         """
         # number of optimization runs
         self.n_runs = n_runs
 
         # store the scales of the parameters
-        self.scales = scales
+        if scales:
+            self.scales = scales
+
+        # store the bounds of the parameters
+        if bounds:
+            self.bounds = bounds
 
         # filter out unneeded values
         # this also holds the fixed parameters
         self.x0 = filter_dict(x0, self.param_names)
 
         # flatten initial values
         flattened = flatten_dict(self.x0)
@@ -743,24 +806,24 @@
 
         # issue warning when the number of parameters to be optimized is large
         if len(optimized_param_names) > 10 and print_info:
             logger.warning(f'A large number of parameters is optimized jointly ({len(optimized_param_names)}). '
                            f'Please be aware that this makes it harder to find a good optimum.')
 
         # correct initial values to be within bounds
-        self.x0 = unflatten_dict(correct_values(flattened, self.bounds, warn=True))
+        self.x0 = unflatten_dict(correct_values(flattened, self.bounds, warn=True, scales=self.scales))
 
         # determine parameter bounds
         bounds = self.get_bounds(flatten_dict(self.x0))
 
         def optimize(x0: Dict[str, Dict[str, float]]) -> OptimizeResult:
             """
             Perform numerical minimization.
 
-            :param x0: Initial values
+            :param x0: Dictionary of initial values in the form ``{type: {param: value}}``
             :return: Optimization result
             """
             logger.debug(f"Initial parameters: {x0}.")
 
             return minimize(
                 fun=self.get_loss_function(
                     get_counts=get_counts,
@@ -790,24 +853,21 @@
         # unscale parameters
         params_mle = unscale_values(params_mle, self.bounds, self.scales)
 
         # check if the MLE reached one of the bounds
         if print_info:
             self.check_bounds(flatten_dict(params_mle))
 
-        # unpack shared parameters
-        params_mle = unpack_shared(params_mle)
-
         return result, params_mle
 
     def scale_values(self, x0: Dict[str, Dict[str, float]]) -> Dict[str, Dict[str, float]]:
         """
         Scale the values of the parameters.
 
-        :param x0: Dictionary of initial values
+        :param x0: Dictionary of initial values in the form ``{type: {param: value}}``
         :return: Dictionary of scaled initial values
         """
         return scale_values(x0, self.bounds, self.scales)
 
     def get_loss_function(
             self,
             get_counts: Dict[str, Callable],
@@ -883,49 +943,55 @@
         """
         sample = {}
 
         for key, value in example.items():
             if isinstance(value, dict):
                 sample[key] = self.sample_x0(value)
             else:
-                sample[key] = self.sample_value(self.bounds[key], self.scales[key])
+                sample[key] = self.sample_value(self.bounds[key], self.scales[key], random_state=self.rng)
 
         return sample
 
     @staticmethod
-    def sample_value(bounds: Tuple[float, float], scale: Literal['lin', 'log', 'symlog']) -> float:
+    def sample_value(
+            bounds: Tuple[float, float],
+            scale: Literal['lin', 'log', 'symlog'],
+            random_state: int | Generator = None
+    ) -> float:
         """
         Sample a value between given bounds using the given scaling.
         This function works for positive, negative, and mixed bounds.
         Note that when ``scale == 'symlog'``, ``bounds[0]`` defines the linear threshold and
         the actual bounds are ``(-bounds[1], bounds[1])``.
 
         :param bounds: Tuple of lower and upper bounds
         :param scale: Scaling of the parameter.
+        :param random_state: Random state
         :return: Sampled value
         """
 
         def flip(bounds: Tuple[float, float]) -> Tuple[float, float]:
             """
             Flip the bounds.
 
-            :param bounds:
-            :return: flipped bounds
+            :param bounds: Tuple of lower and upper bounds
+            :return: Flipped bounds
             """
             return -bounds[1], -bounds[0]
 
-        def symlog_rvs(lower: float, upper: float) -> float:
+        def symlog_rvs(lower: float, upper: float, random_state: int | Generator = None) -> float:
             """
             Sample from a symmetric log-uniform distribution.
 
-            :param lower: lower bound which is the linear threshold
-            :param upper: upper bound so that the actual bounds are (-upper, upper)
-            :return: sampled value
+            :param lower: Lower bound which is the linear threshold
+            :param upper: Upper bound so that the actual bounds are (-upper, upper)
+            :param random_state: Random state
+            :return: Sampled value
             """
-            val = loguniform.rvs(lower, upper)
+            val = loguniform.rvs(lower, upper, random_state=random_state)
 
             # flip sign with 50% probability
             return val if uniform.rvs() < 0.5 else -val
 
         # dictionary of scaling functions
         scaling_functions = {
             'lin': uniform.rvs,
@@ -947,15 +1013,15 @@
 
         # flip bounds if they are negative
         flipped = bounds[0] < 0
         if flipped:
             bounds = flip(bounds)
 
         # sample a value using the appropriate scaling function
-        sample = scaling_functions[scale](bounds[0], bounds[1] - bounds[0])
+        sample = scaling_functions[scale](bounds[0], bounds[1] - bounds[0], random_state=random_state)
 
         # return the sampled value, flipping back if necessary
         return -sample if flipped else sample
 
     def get_bounds(self, x0: Dict[str, float]) -> Dict[str, Tuple[float, float]]:
         """
         Get a nested dictionary of bounds the same structure as the given initial values.
```

### Comparing `fastdfe-0.1.3b0/fastdfe/parametrization.py` & `fastdfe-0.1.4b0/fastdfe/parametrization.py`

 * *Files identical despite different names*

### Comparing `fastdfe-0.1.3b0/fastdfe/parser.py` & `fastdfe-0.1.4b0/fastdfe/parser.py`

 * *Files identical despite different names*

### Comparing `fastdfe-0.1.3b0/fastdfe/polydfe.py` & `fastdfe-0.1.4b0/fastdfe/polydfe.py`

 * *Files identical despite different names*

### Comparing `fastdfe-0.1.3b0/fastdfe/polydfe_utils.py` & `fastdfe-0.1.4b0/fastdfe/polydfe_utils.py`

 * *Files identical despite different names*

### Comparing `fastdfe-0.1.3b0/fastdfe/shared_inference.py` & `fastdfe-0.1.4b0/fastdfe/shared_inference.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,19 +14,22 @@
 
 import jsonpickle
 import multiprocess as mp
 import numpy as np
 import pandas as pd
 from matplotlib import pyplot as plt
 from scipy.optimize import OptimizeResult
+from numpy.linalg import norm
 
-from .base_inference import BaseInference
+from . import Config
 from .abstract_inference import Inference
+from .base_inference import BaseInference
 from .optimization import Optimization, SharedParams, pack_shared, expand_shared, \
-    Covariate, flatten_dict, merge_dicts, correct_values, parallelize as parallelize_func, expand_fixed
+    Covariate, flatten_dict, merge_dicts, correct_values, parallelize as parallelize_func, expand_fixed, collapse_fixed, \
+    unpack_shared
 from .parametrization import Parametrization
 from .spectrum import Spectrum, Spectra
 
 # get logger
 logger = logging.getLogger('fastdfe')
 
 
@@ -43,15 +46,16 @@
             intervals_del: (float, float, int) = (-1.0e+8, -1.0e-5, 1000),
             intervals_ben: (float, float, int) = (1.0e-5, 1.0e4, 1000),
             integration_mode: Literal['midpoint', 'quad'] = 'midpoint',
             linearized: bool = True,
             model: Parametrization | str = 'GammaExpParametrization',
             seed: int = 0,
             x0: Dict[str, Dict[str, float]] = {},
-            bounds: Dict[str, tuple] = {},
+            bounds: Dict[str, Tuple[float, float]] = {},
+            scales: Dict[str, Literal['lin', 'log', 'symlog']] = {},
             loss_type: Literal['likelihood', 'L2'] = 'likelihood',
             opts_mle: dict = {},
             n_runs: int = 10,
             fixed_params: Dict[str, Dict[str, float]] = {},
             shared_params: List[SharedParams] = [],
             covariates: List[Covariate] = [],
             do_bootstrap: bool = False,
@@ -60,27 +64,28 @@
     ):
         """
         Create instance.
 
         :param sfs_neut: Neutral SFS
         :param sfs_sel: Selected SFS
         :param include_divergence: Whether to include divergence in the likelihood
-        :param intervals_del: (start, stop, n_interval) for deleterious population-scaled
+        :param intervals_del: ``(start, stop, n_interval)`` for deleterious population-scaled
         selection coefficients. The intervals will be log10-spaced.
         :param intervals_ben: Same as intervals_del but for beneficial selection coefficients
         :param integration_mode: Integration mode
         :param linearized: Whether to use the linearized model
         :param model: DFE parametrization
         :param seed: Random seed
-        :param x0: dictionary of initial values in the form {type: {param: Value}}
-        :param bounds: Bounds for the parameters in the form {param: (lower, upper)}
+        :param x0: Dictionary of initial values in the form ``{type: {param: value}}``
+        :param bounds: Bounds for the optimization in the form {param: (lower, upper)}
+        :param scales: Scales for the optimization in the form {param: scale}
         :param loss_type: Loss type
         :param opts_mle: Options for the optimization
         :param n_runs: Number of independent optimization runs
-        :param fixed_params: dictionary of fixed parameters in the form {type: {param: Value}}
+        :param fixed_params: dictionary of fixed parameters in the form ``{type: {param: value}}``
         :param shared_params: List of shared parameters
         :param do_bootstrap: Whether to perform bootstrapping
         :param n_bootstraps: Number of bootstraps
         :param parallelize: Whether to parallelize the optimization
         """
         # check whether types are equal
         if set(sfs_neut.types) != set(sfs_sel.types):
@@ -88,14 +93,17 @@
 
         #: SFS types
         self.types: List[str] = sfs_neut.types
 
         # initialize parent
         BaseInference.__init__(**locals())
 
+        #: original MLE parameters before adding covariates and unpacked shared
+        self.params_mle_raw: Optional[Dict[str, Dict[str, float]]] = None
+
         #: Shared parameters with expanded 'all' type
         self.shared_params = expand_shared(shared_params, self.types, self.optimization.param_names)
 
         # add covariates as shared parameters
         self.add_covariates_as_shared(covariates)
 
         # check if the shared parameters were specified correctly
@@ -127,53 +135,61 @@
 
         #: Initial values for covariates
         self.x0_cov = dict((k, cov.x0) for k, cov in self.covariates.items())
 
         # use linear scale for covariates
         scales_cov = dict((k, cov.bounds_scale) for k, cov in self.covariates.items())
 
+        #: fixed parameters with expanded 'all' type
+        self.fixed_params: Dict[str, Dict[str, float]] = expand_fixed(fixed_params, self.types)
+
+        # collapse fixed parameters
+        fixed_collapsed = collapse_fixed(self.fixed_params, self.types)
+
         # include 'all' type with infers the DFE for all spectra added together
         #: Dictionary of marginal inferences indexed by type
         self.marginal_inferences: Dict[str, BaseInference] = dict(
             all=BaseInference(
                 sfs_neut=sfs_neut,
                 sfs_sel=sfs_sel,
                 discretization=self.discretization,
                 include_divergence=include_divergence,
                 model=model,
                 seed=seed,
                 x0=x0,
                 bounds=bounds,
+                scales=scales,
                 loss_type=loss_type,
                 opts_mle=opts_mle,
-                fixed_params=dict(all=fixed_params['all']) if 'all' in fixed_params else {},
+                fixed_params=dict(all=fixed_collapsed['all']) if 'all' in fixed_collapsed else {},
                 do_bootstrap=do_bootstrap,
                 n_bootstraps=n_bootstraps,
                 parallelize=parallelize,
                 n_runs=n_runs)
         )
 
-        #: fixed parameters with expanded 'all' type
-        self.fixed_params: Dict[str, Dict[str, float]] = expand_fixed(fixed_params, self.types)
-
         # check that the fixed parameters are valid
         self.check_fixed_params_exist()
 
         # check if the fixed parameters are compatible with the shared parameters
         self.check_no_shared_params_fixed()
 
-        # scales for all parameters
-        self.scales = self.model.scales | self.default_scales | scales_cov
+        #: parameter scales
+        self.scales: Dict[str, Literal['lin', 'log', 'symlog']] = \
+            self.model.scales | self.default_scales | scales_cov | scales
+
+        #: parameter bounds
+        self.bounds: Dict[str, Tuple[float, float]] = self.model.bounds | self.default_bounds | bounds | bounds_cov
 
         # create optimization instance for joint inference
         # take initial values and bounds from marginal inferences
         # and from this inference for type 'all'
         #: Joint optimization instance
         self.optimization: Optimization = Optimization(
-            bounds=self.model.bounds | self.default_bounds | bounds | bounds_cov,
+            bounds=self.bounds,
             scales=self.scales,
             opts_mle=self.optimization.opts_mle,
             loss_type=self.optimization.loss_type,
             param_names=self.model.param_names + ['eps'] + args_cov,
             parallelize=self.parallelize,
             fixed_params=self.fixed_params,
             seed=self.seed
@@ -190,14 +206,15 @@
                 sfs_sel=sfs_sel[[t]],
                 discretization=self.discretization,
                 include_divergence=include_divergence,
                 model=model,
                 seed=seed,
                 x0=x0,
                 bounds=bounds,
+                scales=scales,
                 loss_type=loss_type,
                 opts_mle=opts_mle,
                 fixed_params=dict(all=self.fixed_params[t]) if t in self.fixed_params else {},
                 do_bootstrap=do_bootstrap,
                 n_bootstraps=n_bootstraps,
                 parallelize=parallelize,
                 n_runs=n_runs
@@ -215,14 +232,15 @@
                     sfs_sel=sfs_sel[[t]],
                     discretization=self.discretization,
                     include_divergence=include_divergence,
                     model=model,
                     seed=seed,
                     x0=x0,
                     bounds=bounds,
+                    scales=scales,
                     loss_type=loss_type,
                     opts_mle=opts_mle,
                     fixed_params=dict(all=self.fixed_params[t]) if t in self.fixed_params else {},
                     do_bootstrap=do_bootstrap,
                     n_bootstraps=n_bootstraps,
                     parallelize=parallelize,
                     n_runs=n_runs,
@@ -276,34 +294,42 @@
 
     def add_covariates_as_shared(self, covariates: List[Covariate]):
         """
         Add covariates as shared parameters.
 
         :param covariates: List of covariates.
         """
+        cov_but_not_shared = self.determine_unshared_covariates(covariates)
+
+        # add parameters with covariates to shared parameters
+        if len(cov_but_not_shared) > 0:
+            logger.info(f'Parameters {cov_but_not_shared} have '
+                        f'covariates and thus need to be shared. '
+                        f'Adding them to shared parameters.')
+
+            # add to shared parameters
+            self.shared_params.append(SharedParams(params=cov_but_not_shared, types=self.types))
+
+    def determine_unshared_covariates(self, covariates):
+        """
+        Determine which covariates are not shared.
+        :param covariates:
+        :return:
+        """
         # determine completely shared parameters
         completely_shared = []
         for shared in self.shared_params:
             if len(shared.types) == len(self.types):
                 completely_shared += shared.params
 
         # determine parameters with covariates
         params_with_covariates = [cov.param for cov in covariates]
 
         # determine parameters with covariates that are not shared
-        cov_but_not_shared = list(set(params_with_covariates) - set(completely_shared))
-
-        # add parameters with covariates to shared parameters
-        if len(cov_but_not_shared) > 0:
-            logger.info(f'Parameters {cov_but_not_shared} have '
-                        f'covariates and thus need to be shared. '
-                        f'Adding them to shared parameters.')
-
-            # add to shared parameters
-            self.shared_params.append(SharedParams(params=cov_but_not_shared, types=self.types))
+        return list(set(params_with_covariates) - set(completely_shared))
 
     def run(
             self,
             do_bootstrap: bool = None,
             pbar: bool = True,
             **kwargs
     ) -> Spectrum:
@@ -397,44 +423,61 @@
                     'independently initialized samples which are run ' +
                     ('in parallel.' if self.parallelize else 'sequentially.'))
 
         # starting time of joint inference
         start_time = time.time()
 
         # Perform joint optimization.
-        self.result, self.params_mle = self.optimization.run(
+        self.result, params_mle = self.optimization.run(
             x0=self.get_x0(),
             scales=self.scales,
+            bounds=self.bounds,
             n_runs=self.n_runs,
             get_counts=self.get_counts()
         )
 
+        # assign likelihoods
+        self.likelihoods = self.optimization.likelihoods
+
+        # store packed MLE params for later usage
+        self.params_mle_raw = copy.deepcopy(params_mle)
+
+        # unpack shared parameters
+        params_mle = unpack_shared(params_mle)
+
         # normalize parameters for each type
         for t in self.types:
-            self.params_mle[t] = self.model.normalize(self.params_mle[t])
+            params_mle[t] = self.model.normalize(params_mle[t])
 
         # report on optimization result
-        self.report_result(self.result, self.params_mle)
+        self.report_result(self.result, params_mle)
 
         # assign optimization result and MLE parameters for each type
         for t, inf in self.joint_inferences.items():
-            self.params_mle[t] = correct_values(
-                params=self.add_covariates(self.params_mle[t], t),
-                bounds=self.optimization.bounds
+            params_mle[t] = correct_values(
+                params=self.add_covariates(params_mle[t], t),
+                bounds=self.bounds,
+                scales=self.scales
             )
 
             # remove effect of covariates and assign result
-            inf.assign_result(self.result, self.params_mle[t])
+            inf.assign_result(self.result, params_mle[t])
 
             # assign execution time
             inf.execution_time = time.time() - start_time
 
+        # assign MLE params
+        self.params_mle = params_mle
+
         # assign joint likelihood
         self.likelihood = -self.result.fun
 
+        # calculate L2 residual
+        self.L2_residual = self.get_L2_residual()
+
         # add execution time
         self.execution_time += time.time() - start_time
 
         # perform bootstrap if configured
         if self.do_bootstrap:
             self.bootstrap()
 
@@ -453,53 +496,96 @@
         Get callback functions for modelling SFS counts from given parameters.
 
         :return: Dict of callback functions indexed by type.
         """
         # Note that it's important we bind t into the lambda function
         # at the time of creation.
         return dict((t, (lambda params, t=t: inf.model_sfs(
-            correct_values(self.add_covariates(params, t), self.optimization.bounds),
+            correct_values(self.add_covariates(params, t), self.bounds, self.scales),
             sfs_neut=self.joint_inferences[t].sfs_neut,
             sfs_sel=self.joint_inferences[t].sfs_sel
         ))) for t, inf in self.joint_inferences.items())
 
+    @BaseInference.run_if_required_wrapper
     @functools.lru_cache
-    def run_joint_without_covariates(self) -> 'SharedInference':
+    def run_joint_without_covariates(self, do_bootstrap: bool = True) -> 'SharedInference':
         """
         Run joint inference without covariates. Note that the result of this function is cached.
 
         :return: Joint inference instance devoid of covariates.
         """
-        # create copy
-        other = copy.deepcopy(self)
+        config = self.create_config()
 
-        # remove covariates
-        other.covariates = {}
+        # retain shared parameters but remove covariates
+        config.update(
+            shared_params=self.shared_params,
+            covariates={},
+            do_bootstrap=do_bootstrap
+        )
+
+        # create copy
+        other = SharedInference.from_config(config)
 
         # issue notice
         logger.info('Running joint inference without covariates.')
 
-        # run joint inference
-        other.run_joint()
+        # run inference
+        other.run()
 
         return other
 
+    def create_config(self) -> 'Config':
+        """
+        Create a config object from the inference object.
+
+        :return: Config object.
+        """
+        return Config(
+            sfs_neut=Spectra.from_spectra(dict((t, inf.sfs_neut) for t, inf in self.marginals_without_all().items())),
+            sfs_sel=Spectra.from_spectra(dict((t, inf.sfs_sel) for t, inf in self.marginals_without_all().items())),
+            intervals_ben=self.discretization.intervals_ben,
+            intervals_del=self.discretization.intervals_del,
+            integration_mode=self.discretization.integration_mode,
+            linearized=self.discretization.linearized,
+            model=self.model.__class__.__name__,
+            seed=self.seed,
+            opts_mle=self.optimization.opts_mle,
+            x0=self.x0,
+            bounds=self.bounds,
+            scales=self.scales,
+            loss_type=self.optimization.loss_type,
+            fixed_params=self.fixed_params,
+            covariates=[c for c in self.covariates.values()],
+            shared_params=self.shared_params,
+            do_bootstrap=self.do_bootstrap,
+            n_bootstraps=self.n_bootstraps,
+            parallelize=self.parallelize,
+            n_runs=self.n_runs
+        )
+
     @BaseInference.run_if_required_wrapper
-    def perform_lrt_covariates(self) -> float:
+    def perform_lrt_covariates(self, do_bootstrap: bool = True) -> float:
         """
         Perform likelihood ratio test against joint inference without covariates.
-        In the simple model we share parameters across types.
+        In the simple model we share parameters across types. Low p-values indicate that
+        the covariates provide a significant improvement in the fit.
 
+        :param do_bootstrap: Whether to bootstrap. This improves the accuracy of the p-value. Note
+        that if bootstrapping was performed previously without updating the likelihood, this won't have any effect.
         :return: Likelihood ratio test statistic.
         """
         if len(self.covariates) == 0:
             raise ValueError('No covariates were specified.')
 
+        # bootstrap if required
+        if do_bootstrap:
+            self.bootstrap_if_required()
+
         # run joint inference without covariates
-        simple = self.run_joint_without_covariates()
+        simple = self.run_joint_without_covariates(do_bootstrap=do_bootstrap)
 
         return self.lrt(simple.likelihood, self.likelihood, len(self.covariates))
 
     def add_covariates(self, params: dict, type: str) -> dict:
         """
         Add covariates to parameters.
 
@@ -541,15 +627,16 @@
 
         logger.info("Bootstrapping marginal inferences.")
 
         # bootstrap marginal inferences
         for inf in self.marginal_inferences.values():
             inf.bootstrap(
                 n_samples=n_samples,
-                parallelize=self.parallelize
+                parallelize=self.parallelize,
+                update_likelihood=update_likelihood
             )
 
         start_time = time.time()
 
         logger.info("Bootstrapping joint inference.")
 
         # parallelize computations if desired
@@ -581,94 +668,78 @@
         # issue warning if some runs did not finish successfully
         if n_success < self.n_bootstraps:
             logger.warning(f"{self.n_bootstraps - n_success} out of {self.n_bootstraps} bootstrap samples "
                            "did not terminate normally during numerical optimization. "
                            "The confidence intervals might thus be unreliable.")
 
         # dataframe of MLE estimates in flattened format
-        bootstraps = pd.DataFrame([flatten_dict(r) for r in result[:, 1]])
+        self.bootstraps = pd.DataFrame([flatten_dict(r) for r in result[:, 1]])
 
         # assign bootstrap parameters to joint inferences
         for t, inf in self.joint_inferences.items():
-            inf.bootstraps = bootstraps.filter(regex=f'{t}.*').rename(columns=lambda x: x.split('.')[-1])
+            inf.bootstraps = self.bootstraps.filter(regex=f'{t}.*').rename(columns=lambda x: x.split('.')[-1])
 
             # add estimates for alpha to the bootstraps
             inf.add_alpha_to_bootstraps()
 
         # add execution time
         self.execution_time += time.time() - start_time
 
-        # determine average likelihood of successful runs
+        # assign average likelihood of successful runs
         if update_likelihood:
             self.likelihood = np.mean([-res.fun for res in result[:, 0] if res.success] + [self.likelihood])
 
         return self.bootstraps
 
+    def bootstrap_if_required(self):
+        """
+        Bootstrap if not done yet.
+        """
+        if self.bootstraps is None:
+            self.bootstrap()
+
     def run_joint_bootstrap_sample(self, seed: int = None) -> (OptimizeResult, dict):
         """
         Resample the observed selected SFS and rerun the optimization procedure.
         We take the MLE params as initial params here.
 
         :return: Optimization result and dictionary of MLE params
         """
-        if seed is not None:
-            self.rng = np.random.default_rng(seed=seed)
-
         # perform joint optimization
         # Note that it's important we bind t into the lambda function
         # at the time of creation.
         result, params_mle = self.optimization.run(
-            x0=self.params_mle_shared,
+            x0=self.params_mle_raw,
             scales=self.get_scales_linear(),
+            bounds=self.get_bounds_linear(),
             n_runs=1,
             debug_iterations=False,
             print_info=False,
             get_counts=dict((t, lambda params, t=t: inf.model_sfs(
-                correct_values(self.add_covariates(params, t), self.optimization.bounds),
-                sfs_neut=self.resample_sfs(self.marginal_inferences[t].sfs_neut),
-                sfs_sel=self.resample_sfs(self.marginal_inferences[t].sfs_sel)
+                correct_values(self.add_covariates(params, t), self.bounds, self.scales),
+                sfs_neut=self.resample_sfs(self.marginal_inferences[t].sfs_neut, seed=seed),
+                sfs_sel=self.resample_sfs(self.marginal_inferences[t].sfs_sel, seed=seed)
             )) for t, inf in self.marginals_without_all().items())
         )
 
-        # normalize parameters for each type
-        for t in self.types:
-            self.params_mle[t] = self.model.normalize(self.params_mle[t])
+        # unpack shared parameters
+        params_mle = unpack_shared(params_mle)
 
-        return result, params_mle
-
-    @property
-    def params_mle_shared(self) -> Dict[str, Dict[str, float]]:
-        """
-        Get MLE parameters with shared parameters.
-
-        :return: Dictionary of MLE parameters with shared parameters as joint-types
-        """
-        shared = {}
-
-        # get dict of shared parameters
-        for s in self.shared_params:
-            for p in s.params:
-                # simply take value of first type as representative
-                shared[':'.join(s.types) + '.' + p] = self.params_mle[s.types[0]][p]
-
-        # create copy of MLE params
-        params_mle = self.params_mle.copy()
-
-        # remove covariates from types
-        for t in params_mle:
-            for p in self.covariates.keys():
-                params_mle[t].pop(p)
-
-        # pack shared parameters
-        packed = pack_shared(self.params_mle, self.shared_params, shared)
+        for t in self.types:
+            # normalize parameters for each type
+            params_mle[t] = self.model.normalize(params_mle[t])
 
-        # add parameters for covariates
-        packed = merge_dicts(packed, {':'.join(self.types): self.x0_cov})
+            # add covariates for each type
+            params_mle[t] = correct_values(
+                params=self.add_covariates(params_mle[t], t),
+                bounds=self.bounds,
+                scales=self.scales
+            )
 
-        return packed
+        return result, params_mle
 
     def get_x0(self) -> Dict[str, Dict[str, float]]:
         """
         Get initial values for joint inference.
 
         :return: Dictionary of initial values indexed by type
         """
@@ -696,23 +767,31 @@
         # pack shared parameters
         packed = pack_shared(x0, self.shared_params, shared)
 
         # add parameters for covariates and return
         return merge_dicts(packed, {':'.join(self.types): self.x0_cov})
 
     @BaseInference.run_if_required_wrapper
-    def perform_lrt_shared(self) -> float:
+    def perform_lrt_shared(self, do_bootstrap: bool = True) -> float:
         """
         Compare likelihood of shared inference with product of marginal likelihoods.
         This provides information about the goodness of fit achieved by the parameter sharing.
-        Note that it is more difficult to properly optimize the joint likelihood, which makes
-        this test conservative, i.e. the p-value might be larger than it should be.
+        Low p-values indicate that parameter sharing is not justified, i.e., that the marginal
+        inferences provide a better fit to the data. Note that it is more difficult to properly
+        optimize the joint likelihood, which makes this test conservative, i.e., the p-value
+        might be larger than it should be.
 
+        :param do_bootstrap: Whether to perform bootstrapping. This improves the accuracy of the p-value. Note
+        that if bootstrapping was performed previously without updating the likelihood, this won't have any effect.
         :return: p-value
         """
+        if do_bootstrap:
+            self.bootstrap_if_required()
+
+        # determine likelihood of marginal inferences
         ll_marginal = sum([inf.likelihood for inf in self.marginals_without_all().values()])
 
         # determine number of parameters
         n_marginal = np.sum([len(inf.params_mle) for inf in self.marginals_without_all().values()])
         n_joint = len(flatten_dict(self.get_x0()))
 
         return self.lrt(ll_simple=self.likelihood, ll_complex=ll_marginal, df=n_marginal - n_joint)
@@ -914,14 +993,22 @@
         :param ax: Axes object
         :return: Axes object
         """
         labels, inferences = zip(*self.get_inferences(labels=labels).items())
 
         return Inference.plot_inferred_parameters(**locals())
 
+    def get_bootstrap_params(self) -> Dict[str, float]:
+        """
+        Get bootstrap parameters.
+
+        :return: Bootstrap parameters
+        """
+        return flatten_dict(dict((t, self.joint_inferences[t].get_bootstrap_params()) for t in self.types))
+
     @BaseInference.run_if_required_wrapper
     def plot_covariates(
             self,
             file: str = None,
             show: bool = True,
             axs: List[plt.Axes] = None
     ) -> List[plt.Axes]:
@@ -983,7 +1070,17 @@
             self.joint_inferences[t].set_fixed_params(dict(all=self.fixed_params[t]))
 
         # propagate to optimization
         self.optimization.set_fixed_params(self.fixed_params)
 
         # check if the fixed parameters are compatible with the shared parameters
         self.check_no_shared_params_fixed()
+
+    def get_L2_residual(self) -> float:
+        """
+        L2 residual of joint inference. We calculate the residual over
+        the jointly inferred SFS for all types.
+        """
+        counts_mle = np.array([inf.sfs_mle.polymorphic for inf in self.joint_inferences.values()]).flatten()
+        counts_sel = np.array([inf.sfs_sel.polymorphic for inf in self.joint_inferences.values()]).flatten()
+
+        return norm(counts_mle - counts_sel, 2)
```

### Comparing `fastdfe-0.1.3b0/fastdfe/spectrum.py` & `fastdfe-0.1.4b0/fastdfe/spectrum.py`

 * *Files identical despite different names*

### Comparing `fastdfe-0.1.3b0/fastdfe/visualization.py` & `fastdfe-0.1.4b0/fastdfe/visualization.py`

 * *Files 1% similar despite different names*

```diff
@@ -869,15 +869,14 @@
 
         # set title
         ax.set_title(title)
 
         return ax
 
     @staticmethod
-    @clear_show_save
     def plot_covariates(
             covariates: Dict[str, 'Covariate'],
             params_marginal: Dict[str, Dict[str, float]],
             params_joint: Dict[str, Dict[str, float]],
             axs: List[plt.Axes],
             scale: Literal['lin', 'log', 'symlog'] = 'log',
             file: str = None,
@@ -904,15 +903,17 @@
         types = list(params_joint.keys())
 
         num_covariates = len(covariates)
 
         n_cols = min(3, num_covariates)
         n_rows = int(np.ceil(num_covariates / n_cols))
 
+        # create axes if not provided
         if not isinstance(axs, np.ndarray | list):
+            plt.clf()
             _, axs = plt.subplots(n_rows, n_cols, figsize=(6.4 * n_cols, 4.8 * n_rows), squeeze=False)
 
         n_intervals = len(types)
         width_total = 0.9
         width = width_total / 2
 
         for i, (p, cov) in enumerate(covariates.items()):
@@ -952,14 +953,17 @@
             # set legend
             ax.legend()
 
             # set y-scale
             if scale == 'log':
                 ax.set_yscale('log')
 
+        # show and save plot
+        Visualization.show_and_save(file, show)
+
         return axs
 
     @clear_show_save
     def plot_interval_density(
             self,
             ax: plt.Axes,
             density: np.ndarray,
```

### Comparing `fastdfe-0.1.3b0/pyproject.toml` & `fastdfe-0.1.4b0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastdfe"
-version = "0.1.3-beta"
+version = "0.1.4-beta"
 description = "Fast, flexible, and hierarchical inference of the distribution of fitness effects"
 authors = ["Sendrowski <sendrowski.janek@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
```

### Comparing `fastdfe-0.1.3b0/PKG-INFO` & `fastdfe-0.1.4b0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastdfe
-Version: 0.1.3b0
+Version: 0.1.4b0
 Summary: Fast, flexible, and hierarchical inference of the distribution of fitness effects
 License: MIT
 Author: Sendrowski
 Author-email: sendrowski.janek@gmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

