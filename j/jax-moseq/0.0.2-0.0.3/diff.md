# Comparing `tmp/jax-moseq-0.0.2.tar.gz` & `tmp/jax-moseq-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jax-moseq-0.0.2.tar", last modified: Sun Apr 23 11:41:17 2023, max compression
+gzip compressed data, was "jax-moseq-0.0.3.tar", last modified: Thu May  4 15:12:12 2023, max compression
```

## Comparing `jax-moseq-0.0.2.tar` & `jax-moseq-0.0.3.tar`

### file list

```diff
@@ -1,40 +1,43 @@
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-04-23 11:41:17.314046 jax-moseq-0.0.2/
--rw-r--r--   0 calebweinreb   (501) staff       (20)     8384 2023-04-19 14:03:05.000000 jax-moseq-0.0.2/LICENSE.md
--rw-r--r--   0 calebweinreb   (501) staff       (20)      393 2023-04-23 11:41:17.314255 jax-moseq-0.0.2/PKG-INFO
--rw-r--r--   0 calebweinreb   (501) staff       (20)     1689 2023-04-19 14:03:05.000000 jax-moseq-0.0.2/README.md
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-04-23 11:41:17.267315 jax-moseq-0.0.2/jax_moseq/
--rw-r--r--   0 calebweinreb   (501) staff       (20)       51 2023-04-19 14:03:05.000000 jax-moseq-0.0.2/jax_moseq/__init__.py
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-04-23 11:41:17.274356 jax-moseq-0.0.2/jax_moseq/models/
--rw-r--r--   0 calebweinreb   (501) staff       (20)       67 2023-04-19 14:03:05.000000 jax-moseq-0.0.2/jax_moseq/models/__init__.py
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-04-23 11:41:17.278501 jax-moseq-0.0.2/jax_moseq/models/arhmm/
--rw-r--r--   0 calebweinreb   (501) staff       (20)      182 2023-04-19 14:03:05.000000 jax-moseq-0.0.2/jax_moseq/models/arhmm/__init__.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     6584 2023-04-19 14:03:05.000000 jax-moseq-0.0.2/jax_moseq/models/arhmm/generate.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     6677 2023-04-22 07:30:26.000000 jax-moseq-0.0.2/jax_moseq/models/arhmm/gibbs.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     8064 2023-04-19 14:03:05.000000 jax-moseq-0.0.2/jax_moseq/models/arhmm/initialize.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     3422 2023-04-19 14:03:05.000000 jax-moseq-0.0.2/jax_moseq/models/arhmm/log_prob.py
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-04-23 11:41:17.283383 jax-moseq-0.0.2/jax_moseq/models/keypoint_slds/
--rw-r--r--   0 calebweinreb   (501) staff       (20)      215 2023-04-19 14:03:05.000000 jax-moseq-0.0.2/jax_moseq/models/keypoint_slds/__init__.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    13504 2023-04-19 14:03:05.000000 jax-moseq-0.0.2/jax_moseq/models/keypoint_slds/alignment.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    11127 2023-04-19 14:03:05.000000 jax-moseq-0.0.2/jax_moseq/models/keypoint_slds/gibbs.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    14485 2023-04-19 14:03:05.000000 jax-moseq-0.0.2/jax_moseq/models/keypoint_slds/initialize.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     4833 2023-04-19 14:03:05.000000 jax-moseq-0.0.2/jax_moseq/models/keypoint_slds/log_prob.py
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-04-23 11:41:17.307825 jax-moseq-0.0.2/jax_moseq/models/slds/
--rw-r--r--   0 calebweinreb   (501) staff       (20)      133 2023-04-19 14:03:05.000000 jax-moseq-0.0.2/jax_moseq/models/slds/__init__.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     9776 2023-04-19 14:03:05.000000 jax-moseq-0.0.2/jax_moseq/models/slds/gibbs.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    10217 2023-04-19 14:03:05.000000 jax-moseq-0.0.2/jax_moseq/models/slds/initialize.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     4081 2023-04-19 14:03:05.000000 jax-moseq-0.0.2/jax_moseq/models/slds/log_prob.py
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-04-23 11:41:17.313097 jax-moseq-0.0.2/jax_moseq/utils/
--rw-r--r--   0 calebweinreb   (501) staff       (20)       35 2023-04-19 14:03:05.000000 jax-moseq-0.0.2/jax_moseq/utils/__init__.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     1148 2023-04-19 14:03:05.000000 jax-moseq-0.0.2/jax_moseq/utils/autoregression.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     2584 2023-04-19 14:03:05.000000 jax-moseq-0.0.2/jax_moseq/utils/distributions.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     4287 2023-04-19 14:03:05.000000 jax-moseq-0.0.2/jax_moseq/utils/kalman.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    11693 2023-04-19 14:03:05.000000 jax-moseq-0.0.2/jax_moseq/utils/transitions.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    11079 2023-04-21 10:38:44.000000 jax-moseq-0.0.2/jax_moseq/utils/utils.py
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-04-23 11:41:17.272970 jax-moseq-0.0.2/jax_moseq.egg-info/
--rw-r--r--   0 calebweinreb   (501) staff       (20)      393 2023-04-23 11:41:17.000000 jax-moseq-0.0.2/jax_moseq.egg-info/PKG-INFO
--rw-r--r--   0 calebweinreb   (501) staff       (20)      955 2023-04-23 11:41:17.000000 jax-moseq-0.0.2/jax_moseq.egg-info/SOURCES.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)        1 2023-04-23 11:41:17.000000 jax-moseq-0.0.2/jax_moseq.egg-info/dependency_links.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)       38 2023-04-23 11:41:17.000000 jax-moseq-0.0.2/jax_moseq.egg-info/requires.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)       10 2023-04-23 11:41:17.000000 jax-moseq-0.0.2/jax_moseq.egg-info/top_level.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)       79 2023-04-23 11:41:17.315075 jax-moseq-0.0.2/setup.cfg
--rw-r--r--   0 calebweinreb   (501) staff       (20)      840 2023-04-23 11:39:38.000000 jax-moseq-0.0.2/setup.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-05-04 15:12:12.870587 jax-moseq-0.0.3/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     8384 2023-04-19 14:03:05.000000 jax-moseq-0.0.3/LICENSE.md
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      300 2023-05-04 15:12:12.870790 jax-moseq-0.0.3/PKG-INFO
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      615 2023-05-04 15:11:20.000000 jax-moseq-0.0.3/README.md
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-05-04 15:12:12.872514 jax-moseq-0.0.3/jax_moseq/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      124 2023-05-04 15:11:20.000000 jax-moseq-0.0.3/jax_moseq/__init__.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      497 2023-05-04 15:12:12.872650 jax-moseq-0.0.3/jax_moseq/_version.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-05-04 15:12:12.854637 jax-moseq-0.0.3/jax_moseq/models/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)       67 2023-04-19 14:03:05.000000 jax-moseq-0.0.3/jax_moseq/models/__init__.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-05-04 15:12:12.857861 jax-moseq-0.0.3/jax_moseq/models/arhmm/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      182 2023-04-19 14:03:05.000000 jax-moseq-0.0.3/jax_moseq/models/arhmm/__init__.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     6584 2023-04-19 14:03:05.000000 jax-moseq-0.0.3/jax_moseq/models/arhmm/generate.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     6789 2023-05-04 15:11:20.000000 jax-moseq-0.0.3/jax_moseq/models/arhmm/gibbs.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     8064 2023-04-19 14:03:05.000000 jax-moseq-0.0.3/jax_moseq/models/arhmm/initialize.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     3422 2023-04-19 14:03:05.000000 jax-moseq-0.0.3/jax_moseq/models/arhmm/log_prob.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-05-04 15:12:12.861379 jax-moseq-0.0.3/jax_moseq/models/keypoint_slds/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      215 2023-04-19 14:03:05.000000 jax-moseq-0.0.3/jax_moseq/models/keypoint_slds/__init__.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    13504 2023-04-19 14:03:05.000000 jax-moseq-0.0.3/jax_moseq/models/keypoint_slds/alignment.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    11141 2023-05-04 15:11:20.000000 jax-moseq-0.0.3/jax_moseq/models/keypoint_slds/gibbs.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    14485 2023-04-30 19:00:54.000000 jax-moseq-0.0.3/jax_moseq/models/keypoint_slds/initialize.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     4833 2023-04-19 14:03:05.000000 jax-moseq-0.0.3/jax_moseq/models/keypoint_slds/log_prob.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-05-04 15:12:12.864908 jax-moseq-0.0.3/jax_moseq/models/slds/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      133 2023-04-19 14:03:05.000000 jax-moseq-0.0.3/jax_moseq/models/slds/__init__.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     9811 2023-05-04 15:11:20.000000 jax-moseq-0.0.3/jax_moseq/models/slds/gibbs.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    10217 2023-04-19 14:03:05.000000 jax-moseq-0.0.3/jax_moseq/models/slds/initialize.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     4081 2023-04-19 14:03:05.000000 jax-moseq-0.0.3/jax_moseq/models/slds/log_prob.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-05-04 15:12:12.870060 jax-moseq-0.0.3/jax_moseq/utils/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)       45 2023-05-04 15:11:20.000000 jax-moseq-0.0.3/jax_moseq/utils/__init__.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     1148 2023-04-19 14:03:05.000000 jax-moseq-0.0.3/jax_moseq/utils/autoregression.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     9385 2023-05-04 15:11:20.000000 jax-moseq-0.0.3/jax_moseq/utils/debugging.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     2644 2023-05-04 15:11:20.000000 jax-moseq-0.0.3/jax_moseq/utils/distributions.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     4343 2023-05-04 15:11:20.000000 jax-moseq-0.0.3/jax_moseq/utils/kalman.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    11715 2023-05-04 15:11:20.000000 jax-moseq-0.0.3/jax_moseq/utils/transitions.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     6471 2023-05-04 15:11:20.000000 jax-moseq-0.0.3/jax_moseq/utils/utils.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-05-04 15:12:12.854139 jax-moseq-0.0.3/jax_moseq.egg-info/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      300 2023-05-04 15:12:12.000000 jax-moseq-0.0.3/jax_moseq.egg-info/PKG-INFO
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     1020 2023-05-04 15:12:12.000000 jax-moseq-0.0.3/jax_moseq.egg-info/SOURCES.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)        1 2023-05-04 15:12:12.000000 jax-moseq-0.0.3/jax_moseq.egg-info/dependency_links.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)       38 2023-05-04 15:12:12.000000 jax-moseq-0.0.3/jax_moseq.egg-info/requires.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)       10 2023-05-04 15:12:12.000000 jax-moseq-0.0.3/jax_moseq.egg-info/top_level.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      590 2023-05-04 15:12:12.872005 jax-moseq-0.0.3/setup.cfg
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      241 2023-05-04 15:11:20.000000 jax-moseq-0.0.3/setup.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    83607 2023-05-04 15:11:20.000000 jax-moseq-0.0.3/versioneer.py
```

### Comparing `jax-moseq-0.0.2/LICENSE.md` & `jax-moseq-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `jax-moseq-0.0.2/jax_moseq/models/arhmm/generate.py` & `jax-moseq-0.0.3/jax_moseq/models/arhmm/generate.py`

 * *Files identical despite different names*

### Comparing `jax-moseq-0.0.2/jax_moseq/models/arhmm/gibbs.py` & `jax-moseq-0.0.3/jax_moseq/models/arhmm/gibbs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 import jax
 import jax.numpy as jnp
 import jax.random as jr
 
-from jax_moseq.utils import pad_affine, psd_solve, psd_inv, convert_data_precision
+from jax_moseq.utils import (
+    pad_affine, 
+    psd_solve, 
+    psd_inv, 
+    nan_check,
+    convert_data_precision
+)
 
 from jax_moseq.utils.distributions import (
     sample_mniw,
     sample_hmm_stateseq
 )
 from jax_moseq.utils.autoregression import (
     get_lags,
@@ -53,15 +59,15 @@
     _, z = jax.vmap(sample_hmm_stateseq, in_axes=(0,na,0,0))(
         jr.split(seed, num_samples),
         pi,
         jnp.moveaxis(log_likelihoods,0,-1),
         mask.astype(float)[:,nlags:])
     return convert_data_precision(z)
 
-
+@nan_check
 @partial(jax.jit, static_argnames=('num_states','nlags'))
 def resample_ar_params(seed, *, nlags, num_states, mask, x, z,
                        nu_0, S_0, M_0, K_0, **kwargs):
     """
     Resamples the AR parameters ``Ab`` and ``Q``.
 
     Parameters
@@ -102,15 +108,15 @@
     x_in = pad_affine(get_lags(x, nlags)).reshape(-1, nlags * x.shape[-1] + 1)
     x_out = x[..., nlags:, :].reshape(-1, x.shape[-1])
     
     map_fun = partial(_resample_regression_params, x_in, x_out, nu_0, S_0, M_0, K_0)
     Ab, Q = jax.lax.map(map_fun, (seeds, masks))
     return Ab, Q
 
-
+@nan_check
 @jax.jit
 def _resample_regression_params(x_in, x_out, nu_0, S_0, M_0, K_0, args):
     """
     Resamples regression parameters from a Matrix normal
     inverse-Wishart distribution.
 
     Parameters
@@ -183,14 +189,16 @@
     Returns
     ------
     model : dict
         Dictionary containing the hyperparameters and
         updated seed, states, and parameters of the model.
     """
     seed = jr.split(seed)[1]
+    params = params.copy()
+    states = states.copy()
 
     if not states_only: 
         if verbose: print('Resampling pi (transition matrix)')
         params['betas'], params['pi'] = resample_hdp_transitions(
             seed, **data, **states, **params, 
             **hypparams['trans_hypparams'])
```

### Comparing `jax-moseq-0.0.2/jax_moseq/models/arhmm/initialize.py` & `jax-moseq-0.0.3/jax_moseq/models/arhmm/initialize.py`

 * *Files identical despite different names*

### Comparing `jax-moseq-0.0.2/jax_moseq/models/arhmm/log_prob.py` & `jax-moseq-0.0.3/jax_moseq/models/arhmm/log_prob.py`

 * *Files identical despite different names*

### Comparing `jax-moseq-0.0.2/jax_moseq/models/keypoint_slds/alignment.py` & `jax-moseq-0.0.3/jax_moseq/models/keypoint_slds/alignment.py`

 * *Files identical despite different names*

### Comparing `jax-moseq-0.0.2/jax_moseq/models/keypoint_slds/gibbs.py` & `jax-moseq-0.0.3/jax_moseq/models/keypoint_slds/gibbs.py`

 * *Files 1% similar despite different names*

```diff
@@ -330,16 +330,16 @@
     model = arhmm.resample_model(data, seed, states, params,
                                  hypparams, states_only, verbose=verbose)
     if ar_only:
         model['noise_prior'] = noise_prior
         return model
     
     seed = model['seed']
-    params = model['params']
-    states = model['states']
+    params = model['params'].copy()
+    states = model['states'].copy()
 
     if not (states_only or skip_noise):
         if verbose: print('Resampling sigmasq (global noise scales)')
         params['sigmasq'] = resample_obs_variance(
             seed, **data, **states, **params, 
             s_0=noise_prior, **hypparams['obs_hypparams'])
```

### Comparing `jax-moseq-0.0.2/jax_moseq/models/keypoint_slds/initialize.py` & `jax-moseq-0.0.3/jax_moseq/models/keypoint_slds/initialize.py`

 * *Files identical despite different names*

### Comparing `jax-moseq-0.0.2/jax_moseq/models/keypoint_slds/log_prob.py` & `jax-moseq-0.0.3/jax_moseq/models/keypoint_slds/log_prob.py`

 * *Files identical despite different names*

### Comparing `jax-moseq-0.0.2/jax_moseq/models/slds/gibbs.py` & `jax-moseq-0.0.3/jax_moseq/models/slds/gibbs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import jax
 import jax.numpy as jnp
 import jax.random as jr
 
-from jax_moseq.utils import apply_affine
+from jax_moseq.utils import apply_affine, nan_check
 from jax_moseq.utils.distributions import sample_scaled_inv_chi2
 from jax_moseq.utils.kalman import kalman_sample, ar_to_lds
 
 from jax_moseq.models import arhmm
 
 na = jnp.newaxis
 
-
+@nan_check
 @jax.jit
 def resample_continuous_stateseqs(seed, Y, mask, z, s, Ab,
                                   Q, Cd, sigmasq, **kwargs):
     """
     Resamples the latent trajectories `x`.
 
     Parameters
@@ -307,16 +307,16 @@
     """
     model = arhmm.resample_model(data, seed, states, params,
                                  hypparams, states_only)
     if ar_only:
         return model
     
     seed = model['seed']
-    params = model['params']
-    states = model['states']
+    params = model['params'].copy()
+    states = model['states'].copy()
     
     if not (states_only or skip_noise):
         params['sigmasq'] = resample_obs_variance(
             seed, **data, **states, **params, 
             **hypparams['obs_hypparams'])
         
     states['x'] = resample_continuous_stateseqs(
```

### Comparing `jax-moseq-0.0.2/jax_moseq/models/slds/initialize.py` & `jax-moseq-0.0.3/jax_moseq/models/slds/initialize.py`

 * *Files identical despite different names*

### Comparing `jax-moseq-0.0.2/jax_moseq/models/slds/log_prob.py` & `jax-moseq-0.0.3/jax_moseq/models/slds/log_prob.py`

 * *Files identical despite different names*

### Comparing `jax-moseq-0.0.2/jax_moseq/utils/autoregression.py` & `jax-moseq-0.0.3/jax_moseq/utils/autoregression.py`

 * *Files identical despite different names*

### Comparing `jax-moseq-0.0.2/jax_moseq/utils/distributions.py` & `jax-moseq-0.0.3/jax_moseq/utils/distributions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import jax, jax.numpy as jnp, jax.random as jr
 import tensorflow_probability.substrates.jax.distributions as tfd
 from dynamax.hidden_markov_model.inference import hmm_posterior_sample
+from jax_moseq.utils import nan_check
 na = jnp.newaxis
 
 def sample_vonmises(seed, theta, kappa):
     return tfd.VonMises(theta, kappa).sample(seed=seed)
 
 def sample_vonmises_fisher(seed, direction):
     kappa = jnp.sqrt((direction**2).sum(-1))
@@ -25,27 +26,29 @@
 
 def sample_mn(seed, M, U, V):
     G = jr.normal(seed,M.shape)
     G = jnp.dot(jnp.linalg.cholesky(U),G)
     G = jnp.dot(G,jnp.linalg.cholesky(V).T)
     return M + G
 
+@nan_check
 def sample_invwishart(seed,S,nu):
     n = S.shape[0]
     
     chi2_seed, norm_seed = jr.split(seed)
     x = jnp.diag(jnp.sqrt(sample_chi2(chi2_seed, nu - jnp.arange(n))))
     x = x.at[jnp.triu_indices_from(x,1)].set(jr.normal(norm_seed, (n*(n-1)//2,)))
     R = jnp.linalg.qr(x,'r')
     
     chol = jnp.linalg.cholesky(S)
     
     T = jax.scipy.linalg.solve_triangular(R.T,chol.T,lower=True).T
     return jnp.dot(T,T.T)
 
+@nan_check
 def sample_mniw(seed, nu, S, M, K):
     sigma = sample_invwishart(seed, S, nu)
     A = sample_mn(seed, M, sigma, K)
     return A, sigma
 
 def sample_hmm_stateseq(seed, transition_matrix, log_likelihoods, mask):
     """Sample state sequences in a Markov chain.
```

### Comparing `jax-moseq-0.0.2/jax_moseq/utils/kalman.py` & `jax-moseq-0.0.3/jax_moseq/utils/kalman.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import jax
 import jax.numpy as jnp
 import jax.random as jr
-
 from jax_moseq.utils.autoregression import get_nlags
-
+from jax_moseq.utils import nan_check
 na = jnp.newaxis
 
-
+@nan_check
 def kalman_filter(ys, mask, zs, m0, S0, A, B, Q, C, D, Rs):
     """
     Run a Kalman filter to produce the marginal likelihood and filtered state 
     estimates. 
     """
 
     def _predict(m, S, A, B, Q):
@@ -49,15 +48,15 @@
         m_pred, S_pred, C, D, Rs[-1], ys[-1])
     
     filtered_ms = jnp.concatenate((filtered_ms,m_cond[na]),axis=0)
     filtered_Ss = jnp.concatenate((filtered_Ss,S_cond[na]),axis=0)
     return filtered_ms, filtered_Ss
 
 
-
+@nan_check
 def kalman_sample(seed, ys, mask, zs, m0, S0, A, B, Q, C, D, Rs):
     
     # run the kalman filter
     filtered_ms, filtered_Ss = kalman_filter(ys, mask, zs, m0, S0, A, B, Q, C, D, Rs)
     
     def _condition_on(m, S, A, B, Qinv, x):
         Sinv = jnp.linalg.inv(S)
```

### Comparing `jax-moseq-0.0.2/jax_moseq/utils/transitions.py` & `jax-moseq-0.0.3/jax_moseq/utils/transitions.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     
     transition_counts = jnp.zeros((num_states, num_states))
     transition_counts = transition_counts.at[start_states, end_states].add(mask)
     return transition_counts
 
 
 @njit
-def _sample_loyal_crf_table_counts(seed, customer_counts, dish_ratings, loyalty):
+def _sample_loyal_crf_table_counts(rng, customer_counts, dish_ratings, loyalty):
     """
     In a Chinese restaurant franchise (CRF) process with loyal customers,
     ``table_counts[i, j]`` represents the number of tables in restaurant ``i``
     that were served dish ``j``, which is a random variable that depends on:
 
         (1) the observed number of patrons in the restaurant eating
             the dish (``customer_counts[i, j]``),
@@ -68,16 +68,16 @@
     of the franchise-wide ``dish_ratings`` (analogous to ``betas`` scaled by ``alpha``).
     For a more thorough overview of the analogy and its relevance to the HDP-HMM
     Gibbs sampling algorithm, see the reference (where `table_counts` corresponds
     to the auxillary parameter m).
 
     Parameters
     ----------
-    seed : int
-        Value for random seed.
+    rng : instance of numpy.random.Generator
+        Seeded random number generator
     customer_counts : numpy array of shape (N, N)
         Number of customers for each restaurant/dish pair.
     dish_ratings : numpy array of shape N
         Parameter representing franchise-wide popularity of each dish.
     loyalty : scalar
         Non-negative scalar representing customers' bias for their
         restaurant's specialty dish.
@@ -88,30 +88,30 @@
         Number of tables in each restaurant served each dish.
 
     References
     ----------
     See the supplement to Fox et al. 2011 at
     <http://dx.doi.org/10.1214/10-AOAS395SUPP>.
     """
-    np.random.seed(seed)
+
     N = len(dish_ratings)    # num restaurants/dishes
 
     # Sample counts without considering loyalty factor
     table_counts = np.zeros_like(customer_counts)
     for i in prange(N):
         for j in range(N):
             # Sample counts by simulating table dish
             # assignment process.
             for k in range(customer_counts[i, j]):
                 dish_rating = dish_ratings[j]
                 if i == j:
                     # Account for loyalty factor
                     dish_rating += loyalty
                 p = dish_rating / (k + dish_rating)
-                bernoulli_sample = np.random.random() < p
+                bernoulli_sample = rng.random() < p
                 table_counts[i, j] += bernoulli_sample
     return table_counts
 
 
 def _sample_beta_suffient_stats(seed, transition_counts,
                                 betas, alpha, kappa, gamma):
     """
@@ -138,27 +138,27 @@
     -------
     sufficient_stats : jax array of shape num_states
         Sufficient statistics for resampling `betas`.
     """
     num_states = len(betas)
     
     # Sample table counts (uses numpy/numba)
-    seed = seed[0].item()
+    rng = np.random.default_rng(seed[0].item())
     concentrations = np.array(alpha * betas)
     transition_counts = np.array(transition_counts, dtype=np.int32)
     # m in Fox et al.
-    table_counts = _sample_loyal_crf_table_counts(seed, transition_counts,
+    table_counts = _sample_loyal_crf_table_counts(rng, transition_counts,
                                                   concentrations, kappa)
     
     # Downweight the influence of self transitions,
     # which are less informative about state usages
     auxillary_param = table_counts    # corresponds to mbar in Fox et al.
     diagonal_counts = np.diag(auxillary_param)
     p = concentrations / (concentrations + kappa)
-    binomial_samples = np.random.binomial(diagonal_counts, p)
+    binomial_samples = rng.binomial(diagonal_counts, p)
     np.fill_diagonal(auxillary_param, binomial_samples)
     
     # Compute sufficient statistics
     sufficient_stats = auxillary_param.sum(0) + (gamma / num_states)
     sufficient_stats = jax.device_put(sufficient_stats)
     return sufficient_stats
```

### Comparing `jax-moseq-0.0.2/jax_moseq.egg-info/SOURCES.txt` & `jax-moseq-0.0.3/jax_moseq.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 LICENSE.md
 README.md
 setup.cfg
 setup.py
+versioneer.py
 jax_moseq/__init__.py
+jax_moseq/_version.py
 jax_moseq.egg-info/PKG-INFO
 jax_moseq.egg-info/SOURCES.txt
 jax_moseq.egg-info/dependency_links.txt
 jax_moseq.egg-info/requires.txt
 jax_moseq.egg-info/top_level.txt
 jax_moseq/models/__init__.py
 jax_moseq/models/arhmm/__init__.py
@@ -21,11 +23,12 @@
 jax_moseq/models/keypoint_slds/log_prob.py
 jax_moseq/models/slds/__init__.py
 jax_moseq/models/slds/gibbs.py
 jax_moseq/models/slds/initialize.py
 jax_moseq/models/slds/log_prob.py
 jax_moseq/utils/__init__.py
 jax_moseq/utils/autoregression.py
+jax_moseq/utils/debugging.py
 jax_moseq/utils/distributions.py
 jax_moseq/utils/kalman.py
 jax_moseq/utils/transitions.py
 jax_moseq/utils/utils.py
```

