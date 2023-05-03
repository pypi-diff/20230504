# Comparing `tmp/estival-0.2.2.tar.gz` & `tmp/estival-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "estival-0.2.2.tar", max compression
+gzip compressed data, was "estival-0.2.3.tar", max compression
```

## Comparing `estival-0.2.2.tar` & `estival-0.2.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     3010 2023-04-04 20:46:52.692604 estival-0.2.2/estival/calibration/__pycache__/pymc.cpython-310.pyc
--rw-r--r--   0        0        0    14860 2023-02-20 23:46:02.295570 estival-0.2.2/estival/calibration/mcmc/__pycache__/adaptive.cpython-39.pyc
--rw-r--r--   0        0        0     2328 2023-02-21 00:23:32.275795 estival-0.2.2/estival/calibration/mcmc/__pycache__/covariance.cpython-39.pyc
--rw-r--r--   0        0        0     3288 2022-11-22 23:17:43.763620 estival-0.2.2/estival/calibration/mcmc/__pycache__/transformations.cpython-39.pyc
--rw-r--r--   0        0        0    23292 2023-03-09 20:46:38.954745 estival-0.2.2/estival/calibration/mcmc/adaptive.py
--rw-r--r--   0        0        0     1916 2023-02-21 00:23:01.508628 estival-0.2.2/estival/calibration/mcmc/covariance.py
--rw-r--r--   0        0        0     3408 2023-03-27 20:16:03.557131 estival-0.2.2/estival/calibration/mcmc/transformations.py
--rw-r--r--   0        0        0     2665 2023-04-04 20:12:53.083034 estival-0.2.2/estival/calibration/pymc.py
--rw-r--r--   0        0        0     2607 2023-05-03 04:10:46.170333 estival-0.2.2/estival/model.py
--rw-r--r--   0        0        0     2194 2023-04-04 00:33:00.496685 estival-0.2.2/estival/optimization/__pycache__/nevergrad.cpython-310.pyc
--rw-r--r--   0        0        0     4492 2023-05-03 03:19:27.593270 estival-0.2.2/estival/optimization/__pycache__/nevergrad.cpython-311.pyc
--rw-r--r--   0        0        0     2627 2023-05-03 04:11:25.401575 estival-0.2.2/estival/optimization/nevergrad.py
--rw-r--r--   0        0        0     3801 2023-04-04 20:15:44.189728 estival-0.2.2/estival/priors.py
--rw-r--r--   0        0        0    10505 2023-05-03 04:13:24.998335 estival-0.2.2/estival/targets.py
--rw-r--r--   0        0        0     2806 2023-03-29 04:09:12.012193 estival-0.2.2/estival/utils.py
--rw-r--r--   0        0        0     1320 2022-11-20 23:56:33.173670 estival-0.2.2/LICENSE
--rw-r--r--   0        0        0      967 2023-05-03 04:15:13.046878 estival-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      236 2022-11-20 23:56:33.174170 estival-0.2.2/README.md
--rw-r--r--   0        0        0     1274 1970-01-01 00:00:00.000000 estival-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     3010 2023-04-04 20:46:52.692604 estival-0.2.3/estival/calibration/__pycache__/pymc.cpython-310.pyc
+-rw-r--r--   0        0        0    14860 2023-02-20 23:46:02.295570 estival-0.2.3/estival/calibration/mcmc/__pycache__/adaptive.cpython-39.pyc
+-rw-r--r--   0        0        0     2328 2023-02-21 00:23:32.275795 estival-0.2.3/estival/calibration/mcmc/__pycache__/covariance.cpython-39.pyc
+-rw-r--r--   0        0        0     3288 2022-11-22 23:17:43.763620 estival-0.2.3/estival/calibration/mcmc/__pycache__/transformations.cpython-39.pyc
+-rw-r--r--   0        0        0    23290 2023-05-03 06:12:36.018586 estival-0.2.3/estival/calibration/mcmc/adaptive.py
+-rw-r--r--   0        0        0     1916 2023-02-21 00:23:01.508628 estival-0.2.3/estival/calibration/mcmc/covariance.py
+-rw-r--r--   0        0        0     3408 2023-03-27 20:16:03.557131 estival-0.2.3/estival/calibration/mcmc/transformations.py
+-rw-r--r--   0        0        0     2665 2023-04-04 20:12:53.083034 estival-0.2.3/estival/calibration/pymc.py
+-rw-r--r--   0        0        0     2659 2023-05-03 20:42:06.724911 estival-0.2.3/estival/model.py
+-rw-r--r--   0        0        0     2666 2023-05-03 21:37:51.092087 estival-0.2.3/estival/optimization/__pycache__/nevergrad.cpython-310.pyc
+-rw-r--r--   0        0        0     4492 2023-05-03 03:19:27.593270 estival-0.2.3/estival/optimization/__pycache__/nevergrad.cpython-311.pyc
+-rw-r--r--   0        0        0     2635 2023-05-03 21:00:19.800964 estival-0.2.3/estival/optimization/nevergrad.py
+-rw-r--r--   0        0        0     3801 2023-04-04 20:15:44.189728 estival-0.2.3/estival/priors.py
+-rw-r--r--   0        0        0    10790 2023-05-03 21:34:29.524110 estival-0.2.3/estival/targets.py
+-rw-r--r--   0        0        0     2806 2023-03-29 04:09:12.012193 estival-0.2.3/estival/utils.py
+-rw-r--r--   0        0        0     1320 2022-11-20 23:56:33.173670 estival-0.2.3/LICENSE
+-rw-r--r--   0        0        0     1002 2023-05-03 23:14:40.994446 estival-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      406 2023-05-03 23:21:51.163726 estival-0.2.3/README.md
+-rw-r--r--   0        0        0     1492 1970-01-01 00:00:00.000000 estival-0.2.3/PKG-INFO
```

### Comparing `estival-0.2.2/estival/calibration/__pycache__/pymc.cpython-310.pyc` & `estival-0.2.3/estival/calibration/__pycache__/pymc.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `estival-0.2.2/estival/calibration/mcmc/__pycache__/adaptive.cpython-39.pyc` & `estival-0.2.3/estival/calibration/mcmc/__pycache__/adaptive.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `estival-0.2.2/estival/calibration/mcmc/__pycache__/covariance.cpython-39.pyc` & `estival-0.2.3/estival/calibration/mcmc/__pycache__/covariance.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `estival-0.2.2/estival/calibration/mcmc/__pycache__/transformations.cpython-39.pyc` & `estival-0.2.3/estival/calibration/mcmc/__pycache__/transformations.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `estival-0.2.2/estival/calibration/mcmc/adaptive.py` & `estival-0.2.3/estival/calibration/mcmc/adaptive.py`

 * *Files 0% similar despite different names*

```diff
@@ -174,15 +174,14 @@
         self.target_evaluators = {t.name: t.get_evaluator(model_times_dti) for t in self.targets}
 
     def run(
         self,
         available_time: str = None,
         max_iter: int = None,
     ):
-
         if not self._has_run:
             self.starting_point = self.get_transformed_start(self.initial_priors)
 
             # Set chain specific seed
             # Chain 0 will have seed equal to that set in the calibration initialisation
             self.seed_chain = ((self.chain_id * 2**22) + self.seed) % (2**32)
 
@@ -207,15 +206,15 @@
     def loglikelihood(self, all_params_dict):
         """
         Calculate the loglikelihood for a set of parameters
         """
 
         modelled = self.run_model_with_params(all_params_dict)
 
-        ll = 0  # loglikelihood if using bayesian approach.
+        ll = 0.0  # loglikelihood if using bayesian approach.
 
         for k, te in self.target_evaluators.items():
             mdata = modelled[k]
             ll += te.evaluate(mdata, all_params_dict)
 
         return ll
 
@@ -233,15 +232,14 @@
                 s = sum(target.time_weights)
                 target.time_weights = target.time_weights / s
 
     def workout_unspecified_jumping_stdevs(self):
         self.jumping_sds = {}
 
         for i, prior in enumerate(self.priors):
-
             prior_low, prior_high = prior.bounds(0.95)
             prior_width = prior_high - prior_low
 
             #  95% of the sampled values within [mu - 2*sd, mu + 2*sd], i.e. interval of witdth 4*sd
             relative_prior_width = (
                 self.metropolis_init_rel_step_size  # fraction of prior_width in which 95% of samples should fall
             )
@@ -325,15 +323,14 @@
 
             # transform the density
             proposed_acceptance_quantity = proposed_log_posterior
 
             for i, prior in enumerate(
                 self.priors
             ):  # multiply the density with the determinant of the Jacobian
-
                 inv_derivative = self.transform[prior.name].inverse_derivative(
                     proposed_iterative_params_trans[i]
                 )
                 if inv_derivative > 0:
                     proposed_acceptance_quantity += np.log(inv_derivative)
                 else:
                     proposed_acceptance_quantity += np.log(1.0e-100)
@@ -420,15 +417,15 @@
         cov_matrix = self.covariance.cov_t
         adaptive_cov_matrix = scaling_factor * cov_matrix + scaling_factor * ADAPTIVE_METROPOLIS[
             "EPSILON"
         ] * np.eye(len(self.priors))
         return adaptive_cov_matrix
 
     def build_transformations(self):
-        self.transform : Dict[str, TransformedPrior] = {}
+        self.transform: Dict[str, TransformedPrior] = {}
 
         for prior in self.priors:
             param_name = prior.name
             self.transform[param_name] = TransformedPrior(prior)
 
     def get_transformed_start(self, starting_point: dict):
         """
```

### Comparing `estival-0.2.2/estival/calibration/mcmc/covariance.py` & `estival-0.2.3/estival/calibration/mcmc/covariance.py`

 * *Files identical despite different names*

### Comparing `estival-0.2.2/estival/calibration/mcmc/transformations.py` & `estival-0.2.3/estival/calibration/mcmc/transformations.py`

 * *Files identical despite different names*

### Comparing `estival-0.2.2/estival/calibration/pymc.py` & `estival-0.2.3/estival/calibration/pymc.py`

 * *Files identical despite different names*

### Comparing `estival-0.2.2/estival/model.py` & `estival-0.2.3/estival/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,34 +30,35 @@
         self._ref_idx = self.model._get_ref_idx()
 
     def _build_logll_func(self, extra_ll=None):
         model_params = self.model.get_input_parameters()
         dyn_params = list(model_params.intersection(set(self.priors)))
         self.model.set_derived_outputs_whitelist(list(self.targets))
 
-        ll_runner = self.model.get_runner(self.parameters, dyn_params)
+        self._ll_runner = self.model.get_runner(self.parameters, dyn_params)
 
         self.model.set_derived_outputs_whitelist([])
         self._full_runner = self.model.get_runner(self.parameters, dyn_params)
 
         tidx = pd.Index(self.model.times)
 
-        evaluators = {}
+        self._evaluators = {}
         for k, t in self.targets.items():
-            evaluators[k] = t.get_evaluator(tidx)
+            tev = t.get_evaluator(tidx)
+            self._evaluators[k] = tev.evaluate
 
         @jit
         def logll(**kwargs):
             dict_args = capture_model_kwargs(self.model, **kwargs)
-            res = ll_runner._run_func(dict_args)["derived_outputs"]
+            res = self._ll_runner._run_func(dict_args)["derived_outputs"]
 
             logdens = 0.0
-            for tk, te in evaluators.items():
+            for tk, te in self._evaluators.items():
                 modelled = res[tk]
-                logdens += te.evaluate(modelled, kwargs)
+                logdens += te(modelled, kwargs)
 
             if extra_ll:
                 logdens += extra_ll(kwargs)
 
             return logdens
 
         return logll
```

### Comparing `estival-0.2.2/estival/optimization/__pycache__/nevergrad.cpython-310.pyc` & `estival-0.2.3/estival/optimization/__pycache__/nevergrad.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr  4 00:32:27 2023 UTC, .py size: 2401 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,138 +1,167 @@
-00000000: 6f0d 0d0a 0000 0000 1b70 2b64 6109 0000  o........p+da...
+00000000: 6f0d 0d0a 0000 0000 63cb 5264 4b0a 0000  o.......c.RdK...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 000b 0000 0040 0000 0073 9800 0000 6400  .....@...s....d.
+00000020: 000d 0000 0040 0000 0073 ac00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
-00000040: 6d03 5a03 0100 6400 6403 6c04 5a05 6400  m.Z...d.d.l.Z.d.
-00000050: 6404 6c06 6d07 5a07 0100 6400 6405 6c08  d.l.m.Z...d.d.l.
-00000060: 6d09 5a09 0100 7a06 6400 6403 6c0a 5a0b  m.Z...z.d.d.l.Z.
-00000070: 5700 6e04 0100 0100 0100 5900 6413 6407  W.n.......Y.d.d.
-00000080: 6408 8401 5a0c 4700 6409 640a 8400 640a  d...Z.G.d.d...d.
-00000090: 8302 5a0d 640b 650b 6a0e 6a0f 6403 6403  ..Z.d.e.j.j.d.d.
-000000a0: 6406 6605 640c 6507 640d 6510 640e 6510  d.f.d.e.d.e.d.e.
-000000b0: 640f 6511 6410 6512 660a 6411 6412 8405  d.e.d.e.f.d.d...
-000000c0: 5a13 6403 5300 2914 e900 0000 0029 01da  Z.d.S.)......)..
-000000d0: 0766 7574 7572 6573 2901 da09 6370 755f  .futures)...cpu_
-000000e0: 636f 756e 744e 2901 da1a 4261 7965 7369  countN)...Bayesi
-000000f0: 616e 436f 6d70 6172 746d 656e 7461 6c4d  anCompartmentalM
-00000100: 6f64 656c 2901 da08 6e65 6761 7469 7665  odel)...negative
-00000110: da08 6d69 6470 6f69 6e74 6303 0000 0000  ..midpointc.....
-00000120: 0000 0000 0000 000b 0000 0006 0000 0043  ...............C
-00000130: 0000 0073 f400 0000 6900 7d03 7c01 7005  ...s....i.}.|.p.
-00000140: 6900 7d01 6900 7d04 7c00 a000 a100 4400  i.}.i.}.|.....D.
-00000150: 5d35 5c02 7d05 7d06 7c01 a001 7c05 a101  ]5\.}.}.|...|...
-00000160: 0400 7d07 721c 7c07 7c04 7c05 3c00 710c  ..}.r.|.|.|.<.q.
-00000170: 7c02 6401 6b02 7228 7402 a003 6402 7c06  |.d.k.r(t...d.|.
-00000180: 6a04 a102 7d08 6e12 7c02 6403 6b02 7235  j...}.n.|.d.k.r5
-00000190: 7402 6a05 6a06 7c06 6a04 6404 8d01 7d08  t.j.j.|.j.d...}.
-000001a0: 6e05 7407 6405 7c02 8302 8201 7c06 a008  n.t.d.|.....|...
-000001b0: 7c08 a101 7c04 7c05 3c00 710c 7c00 a000  |...|.|.<.q.|...
-000001c0: a100 4400 5d2a 5c02 7d05 7d06 7c06 a009  ..D.]*\.}.}.|...
-000001d0: a100 5c02 7d09 7d0a 7c06 6a04 6406 6b02  ..\.}.}.|.j.d.k.
-000001e0: 7263 740a 6a0b 6a0c 7c04 7c05 1900 7c09  rct.j.j.|.|...|.
-000001f0: 7c0a 6407 8d03 7c03 7c05 3c00 7146 740a  |.d...|.|.<.qFt.
-00000200: 6a0b 6a0d 7c04 7c05 1900 7c09 7c0a 6407  j.j.|.|...|.|.d.
-00000210: 8d03 7c03 7c05 3c00 7146 740a 6a0b 6a0e  ..|.|.<.qFt.j.j.
-00000220: 6408 6900 7c03 a401 8e01 5300 2909 4e72  d.i.|.....S.).Nr
-00000230: 0600 0000 6700 0000 0000 00e0 3fda 0775  ....g.......?..u
-00000240: 6e69 666f 726d 2901 da04 7369 7a65 7a13  niform)...sizez.
-00000250: 496e 7661 6c69 6420 696e 6974 206d 6574  Invalid init met
-00000260: 686f 64e9 0100 0000 2903 da04 696e 6974  hod.....)...init
-00000270: da05 6c6f 7765 72da 0575 7070 6572 a900  ..lower..upper..
-00000280: 290f da05 6974 656d 73da 0367 6574 da02  )...items..get..
-00000290: 6e70 da06 7265 7065 6174 7208 0000 00da  np..repeatr.....
-000002a0: 0672 616e 646f 6d72 0700 0000 da0a 5661  .randomr......Va
-000002b0: 6c75 6545 7272 6f72 da03 7070 66da 0662  lueError..ppf..b
-000002c0: 6f75 6e64 73da 026e 67da 0170 da06 5363  ounds..ng..p..Sc
-000002d0: 616c 6172 da05 4172 7261 795a 0f49 6e73  alar..ArrayZ.Ins
-000002e0: 7472 756d 656e 7461 7469 6f6e 290b da06  trumentation)...
-000002f0: 7072 696f 7273 da09 7375 6767 6573 7465  priors..suggeste
-00000300: 64da 0b69 6e69 745f 6d65 7468 6f64 5a05  d..init_methodZ.
-00000310: 6964 6963 745a 0f73 7461 7274 696e 675f  idictZ.starting_
-00000320: 706f 696e 7473 da02 706b 7217 0000 005a  points..pkr....Z
-00000330: 0673 7567 5f70 74da 0270 7072 0b00 0000  .sug_pt..ppr....
-00000340: 720c 0000 0072 0d00 0000 720d 0000 00fa  r....r....r.....
-00000350: 382f 6d6e 742f 632f 6465 762f 454d 552f  8/mnt/c/dev/EMU/
-00000360: 6573 7469 7661 6c2f 6573 7469 7661 6c2f  estival/estival/
-00000370: 6f70 7469 6d69 7a61 7469 6f6e 2f6e 6576  optimization/nev
-00000380: 6572 6772 6164 2e70 79da 1367 6574 5f69  ergrad.py..get_i
-00000390: 6e73 7472 756d 656e 7461 7469 6f6e 1000  nstrumentation..
-000003a0: 0000 7324 0000 0004 0108 0204 0110 010e  ..s$............
-000003b0: 010a 0108 0210 0108 0112 010a 0210 0110  ................
-000003c0: 020c 010a 011c 011c 0212 0272 2000 0000  ...........r ...
-000003d0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-000003e0: 0002 0000 0040 0000 0073 1c00 0000 6500  .....@...s....e.
-000003f0: 5a01 6400 5a02 6401 6402 8400 5a03 6403  Z.d.Z.d.d...Z.d.
-00000400: 6404 8400 5a04 6405 5300 2906 da09 4f70  d...Z.d.S.)...Op
-00000410: 7452 756e 6e65 7263 0400 0000 0000 0000  tRunnerc........
-00000420: 0000 0000 0400 0000 0200 0000 4300 0000  ............C...
-00000430: 7316 0000 007c 017c 005f 007c 027c 005f  s....|.|._.|.|._
-00000440: 017c 037c 005f 0264 0053 0029 014e 2903  .|.|._.d.S.).N).
-00000450: da09 6f70 7469 6d69 7a65 72da 086d 696e  ..optimizer..min
-00000460: 5f66 756e 63da 0b6e 756d 5f77 6f72 6b65  _func..num_worke
-00000470: 7273 2904 da04 7365 6c66 7222 0000 0072  rs)...selfr"...r
-00000480: 2300 0000 7224 0000 0072 0d00 0000 720d  #...r$...r....r.
-00000490: 0000 0072 1f00 0000 da08 5f5f 696e 6974  ...r......__init
-000004a0: 5f5f 2b00 0000 7306 0000 0006 0106 010a  __+...s.........
-000004b0: 017a 124f 7074 5275 6e6e 6572 2e5f 5f69  .z.OptRunner.__i
-000004c0: 6e69 745f 5f63 0200 0000 0000 0000 0000  nit__c..........
-000004d0: 0000 0500 0000 0800 0000 4300 0000 735a  ..........C...sZ
-000004e0: 0000 007c 006a 006a 017d 027c 027c 0117  ...|.j.j.}.|.|..
-000004f0: 007c 006a 005f 0274 036a 047c 006a 0564  .|.j._.t.j.|.j.d
-00000500: 018d 018f 127d 037c 006a 006a 067c 006a  .....}.|.j.j.|.j
-00000510: 077c 0364 028d 027d 0457 0064 0004 0004  .|.d...}.W.d....
-00000520: 0083 0301 007c 0453 0031 0073 2677 0101  .....|.S.1.s&w..
-00000530: 0001 0001 0059 0001 007c 0453 0029 034e  .....Y...|.S.).N
-00000540: 2901 da0b 6d61 785f 776f 726b 6572 7329  )...max_workers)
-00000550: 01da 0865 7865 6375 746f 7229 0872 2200  ...executor).r".
-00000560: 0000 5a07 6e75 6d5f 6173 6bda 0662 7564  ..Z.num_ask..bud
-00000570: 6765 7472 0200 0000 da12 5468 7265 6164  getr......Thread
-00000580: 506f 6f6c 4578 6563 7574 6f72 7224 0000  PoolExecutorr$..
-00000590: 00da 086d 696e 696d 697a 6572 2300 0000  ...minimizer#...
-000005a0: 2905 7225 0000 0072 2900 0000 5a07 6375  ).r%...r)...Z.cu
-000005b0: 725f 6173 6b72 2800 0000 da03 7265 6372  r_askr(.....recr
-000005c0: 0d00 0000 720d 0000 0072 1f00 0000 722b  ....r....r....r+
-000005d0: 0000 0030 0000 0073 1000 0000 0801 0c01  ...0...s........
-000005e0: 1001 1401 0aff 0402 10fe 0402 7a12 4f70  ............z.Op
-000005f0: 7452 756e 6e65 722e 6d69 6e69 6d69 7a65  tRunner.minimize
-00000600: 4e29 05da 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
-00000610: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
-00000620: 6c6e 616d 655f 5f72 2600 0000 722b 0000  lname__r&...r+..
-00000630: 0072 0d00 0000 720d 0000 0072 0d00 0000  .r....r....r....
-00000640: 721f 0000 0072 2100 0000 2a00 0000 7306  r....r!...*...s.
-00000650: 0000 0008 0008 010c 0572 2100 0000 69e8  .........r!...i.
-00000660: 0300 00da 0362 636d 7229 0000 0072 2400  .....bcmr)...r$.
-00000670: 0000 721b 0000 0072 1c00 0000 6306 0000  ..r....r....c...
-00000680: 0000 0000 0000 0000 0009 0000 0005 0000  ................
-00000690: 0043 0000 0073 3c00 0000 7c03 7305 7400  .C...s<...|.s.t.
-000006a0: 8300 7d03 7401 7c00 6a02 7c04 7c05 8303  ..}.t.|.j.|.|...
-000006b0: 7d06 7403 7c00 6a04 8301 7d07 7c02 7c06  }.t.|.j...}.|.|.
-000006c0: 7c01 7c03 6401 8d03 7d08 7405 7c08 7c07  |.|.d...}.t.|.|.
-000006d0: 7c03 8303 5300 2902 4e29 035a 0f70 6172  |...S.).N).Z.par
-000006e0: 616d 6574 7269 7a61 7469 6f6e 7229 0000  ametrizationr)..
-000006f0: 0072 2400 0000 2906 7203 0000 0072 2000  .r$...).r....r .
-00000700: 0000 721a 0000 0072 0500 0000 da0d 6c6f  ..r....r......lo
-00000710: 676c 696b 656c 6968 6f6f 6472 2100 0000  glikelihoodr!...
-00000720: 2909 7230 0000 0072 2900 0000 5a09 6f70  ).r0...r)...Z.op
-00000730: 745f 636c 6173 7372 2400 0000 721b 0000  t_classr$...r...
-00000740: 0072 1c00 0000 5a07 696e 7374 7275 6d72  .r....Z.instrumr
-00000750: 2300 0000 7222 0000 0072 0d00 0000 720d  #...r"...r....r.
-00000760: 0000 0072 1f00 0000 da0e 6f70 7469 6d69  ...r......optimi
-00000770: 7a65 5f6d 6f64 656c 3700 0000 730c 0000  ze_model7...s...
-00000780: 0004 0706 010e 020a 010e 010c 0172 3200  .............r2.
-00000790: 0000 2902 4e72 0600 0000 2914 da0a 636f  ..).Nr....)...co
-000007a0: 6e63 7572 7265 6e74 7202 0000 00da 0f6d  ncurrentr......m
-000007b0: 756c 7469 7072 6f63 6573 7369 6e67 7203  ultiprocessingr.
-000007c0: 0000 00da 056e 756d 7079 7210 0000 00da  .....numpyr.....
-000007d0: 0d65 7374 6976 616c 2e6d 6f64 656c 7204  .estival.modelr.
-000007e0: 0000 005a 0d65 7374 6976 616c 2e75 7469  ...Z.estival.uti
-000007f0: 6c73 7205 0000 005a 096e 6576 6572 6772  lsr....Z.nevergr
-00000800: 6164 7216 0000 0072 2000 0000 7221 0000  adr....r ...r!..
-00000810: 005a 0a6f 7074 696d 697a 6572 735a 054e  .Z.optimizersZ.N
-00000820: 474f 7074 da03 696e 74da 0464 6963 74da  GOpt..int..dict.
-00000830: 0373 7472 7232 0000 0072 0d00 0000 720d  .strr2...r....r.
-00000840: 0000 0072 0d00 0000 721f 0000 00da 083c  ...r....r......<
-00000850: 6d6f 6475 6c65 3e01 0000 0073 3200 0000  module>....s2...
-00000860: 0c00 0c01 0801 0c02 0c01 0205 0c01 0601  ................
-00000870: 0201 0a02 0e1a 020e 0601 0201 0201 0201  ................
-00000880: 08fb 0201 02ff 0203 02fd 0204 02fc 0205  ................
-00000890: 0efb                                     ..
+00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
+00000050: 0100 6400 6404 6c06 5a07 6400 6405 6c08  ..d.d.l.Z.d.d.l.
+00000060: 6d09 5a09 0100 6400 6406 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
+00000070: 0100 7a06 6400 6404 6c0c 5a0d 5700 6e04  ..z.d.d.l.Z.W.n.
+00000080: 0100 0100 0100 5900 6416 6408 6409 8401  ......Y.d.d.d...
+00000090: 5a0e 4700 640a 640b 8400 640b 8302 5a0f  Z.G.d.d...d...Z.
+000000a0: 640c 650d 6a10 6a11 6404 6404 6407 6404  d.e.j.j.d.d.d.d.
+000000b0: 640d 6607 640e 6509 640f 6512 6410 6512  d.f.d.e.d.e.d.e.
+000000c0: 6411 6513 6412 6514 6413 6501 660c 6414  d.e.d.e.d.e.f.d.
+000000d0: 6415 8405 5a15 6404 5300 2917 e900 0000  d...Z.d.S.).....
+000000e0: 0029 01da 0843 616c 6c61 626c 6529 01da  .)...Callable)..
+000000f0: 0766 7574 7572 6573 2901 da09 6370 755f  .futures)...cpu_
+00000100: 636f 756e 744e 2901 da1a 4261 7965 7369  countN)...Bayesi
+00000110: 616e 436f 6d70 6172 746d 656e 7461 6c4d  anCompartmentalM
+00000120: 6f64 656c 2901 da08 6e65 6761 7469 7665  odel)...negative
+00000130: da08 6d69 6470 6f69 6e74 6303 0000 0000  ..midpointc.....
+00000140: 0000 0000 0000 000b 0000 0006 0000 0043  ...............C
+00000150: 0000 0073 f400 0000 6900 7d03 7c01 7005  ...s....i.}.|.p.
+00000160: 6900 7d01 6900 7d04 7c00 a000 a100 4400  i.}.i.}.|.....D.
+00000170: 5d35 5c02 7d05 7d06 7c01 a001 7c05 a101  ]5\.}.}.|...|...
+00000180: 0400 7d07 721c 7c07 7c04 7c05 3c00 710c  ..}.r.|.|.|.<.q.
+00000190: 7c02 6401 6b02 7228 7402 a003 6402 7c06  |.d.k.r(t...d.|.
+000001a0: 6a04 a102 7d08 6e12 7c02 6403 6b02 7235  j...}.n.|.d.k.r5
+000001b0: 7402 6a05 6a06 7c06 6a04 6404 8d01 7d08  t.j.j.|.j.d...}.
+000001c0: 6e05 7407 6405 7c02 8302 8201 7c06 a008  n.t.d.|.....|...
+000001d0: 7c08 a101 7c04 7c05 3c00 710c 7c00 a000  |...|.|.<.q.|...
+000001e0: a100 4400 5d2a 5c02 7d05 7d06 7c06 a009  ..D.]*\.}.}.|...
+000001f0: a100 5c02 7d09 7d0a 7c06 6a04 6406 6b02  ..\.}.}.|.j.d.k.
+00000200: 7263 740a 6a0b 6a0c 7c04 7c05 1900 7c09  rct.j.j.|.|...|.
+00000210: 7c0a 6407 8d03 7c03 7c05 3c00 7146 740a  |.d...|.|.<.qFt.
+00000220: 6a0b 6a0d 7c04 7c05 1900 7c09 7c0a 6407  j.j.|.|...|.|.d.
+00000230: 8d03 7c03 7c05 3c00 7146 740a 6a0b 6a0e  ..|.|.<.qFt.j.j.
+00000240: 6408 6900 7c03 a401 8e01 5300 2909 4e72  d.i.|.....S.).Nr
+00000250: 0700 0000 6700 0000 0000 00e0 3fda 0775  ....g.......?..u
+00000260: 6e69 666f 726d 2901 da04 7369 7a65 7a13  niform)...sizez.
+00000270: 496e 7661 6c69 6420 696e 6974 206d 6574  Invalid init met
+00000280: 686f 64e9 0100 0000 2903 da04 696e 6974  hod.....)...init
+00000290: da05 6c6f 7765 72da 0575 7070 6572 a900  ..lower..upper..
+000002a0: 290f da05 6974 656d 73da 0367 6574 da02  )...items..get..
+000002b0: 6e70 da06 7265 7065 6174 7209 0000 00da  np..repeatr.....
+000002c0: 0672 616e 646f 6d72 0800 0000 da0a 5661  .randomr......Va
+000002d0: 6c75 6545 7272 6f72 da03 7070 66da 0662  lueError..ppf..b
+000002e0: 6f75 6e64 73da 026e 67da 0170 da06 5363  ounds..ng..p..Sc
+000002f0: 616c 6172 da05 4172 7261 795a 0f49 6e73  alar..ArrayZ.Ins
+00000300: 7472 756d 656e 7461 7469 6f6e 290b da06  trumentation)...
+00000310: 7072 696f 7273 da09 7375 6767 6573 7465  priors..suggeste
+00000320: 64da 0b69 6e69 745f 6d65 7468 6f64 5a05  d..init_methodZ.
+00000330: 6964 6963 74da 0f73 7461 7274 696e 675f  idict..starting_
+00000340: 706f 696e 7473 da02 706b 7218 0000 005a  points..pkr....Z
+00000350: 0673 7567 5f70 74da 0270 7072 0c00 0000  .sug_pt..ppr....
+00000360: 720d 0000 0072 0e00 0000 720e 0000 00fa  r....r....r.....
+00000370: 382f 6d6e 742f 632f 6465 762f 454d 552f  8/mnt/c/dev/EMU/
+00000380: 6573 7469 7661 6c2f 6573 7469 7661 6c2f  estival/estival/
+00000390: 6f70 7469 6d69 7a61 7469 6f6e 2f6e 6576  optimization/nev
+000003a0: 6572 6772 6164 2e70 79da 1367 6574 5f69  ergrad.py..get_i
+000003b0: 6e73 7472 756d 656e 7461 7469 6f6e 1200  nstrumentation..
+000003c0: 0000 7324 0000 0004 0108 0204 0110 010e  ..s$............
+000003d0: 010a 0108 0210 0108 0112 010a 0210 0110  ................
+000003e0: 020c 010a 011c 011c 0212 0272 2200 0000  ...........r"...
+000003f0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00000400: 0002 0000 0040 0000 0073 1c00 0000 6500  .....@...s....e.
+00000410: 5a01 6400 5a02 6401 6402 8400 5a03 6403  Z.d.Z.d.d...Z.d.
+00000420: 6404 8400 5a04 6405 5300 2906 da09 4f70  d...Z.d.S.)...Op
+00000430: 7452 756e 6e65 7263 0400 0000 0000 0000  tRunnerc........
+00000440: 0000 0000 0400 0000 0200 0000 4300 0000  ............C...
+00000450: 7316 0000 007c 017c 005f 007c 027c 005f  s....|.|._.|.|._
+00000460: 017c 037c 005f 0264 0053 0029 014e 2903  .|.|._.d.S.).N).
+00000470: da09 6f70 7469 6d69 7a65 72da 086d 696e  ..optimizer..min
+00000480: 5f66 756e 63da 0b6e 756d 5f77 6f72 6b65  _func..num_worke
+00000490: 7273 2904 da04 7365 6c66 7224 0000 0072  rs)...selfr$...r
+000004a0: 2500 0000 7226 0000 0072 0e00 0000 720e  %...r&...r....r.
+000004b0: 0000 0072 2100 0000 da08 5f5f 696e 6974  ...r!.....__init
+000004c0: 5f5f 2e00 0000 7306 0000 0006 0106 010a  __....s.........
+000004d0: 017a 124f 7074 5275 6e6e 6572 2e5f 5f69  .z.OptRunner.__i
+000004e0: 6e69 745f 5f63 0200 0000 0000 0000 0000  nit__c..........
+000004f0: 0000 0500 0000 0800 0000 4300 0000 735a  ..........C...sZ
+00000500: 0000 007c 006a 006a 017d 027c 027c 0117  ...|.j.j.}.|.|..
+00000510: 007c 006a 005f 0274 036a 047c 006a 0564  .|.j._.t.j.|.j.d
+00000520: 018d 018f 127d 037c 006a 006a 067c 006a  .....}.|.j.j.|.j
+00000530: 077c 0364 028d 027d 0457 0064 0004 0004  .|.d...}.W.d....
+00000540: 0083 0301 007c 0453 0031 0073 2677 0101  .....|.S.1.s&w..
+00000550: 0001 0001 0059 0001 007c 0453 0029 034e  .....Y...|.S.).N
+00000560: 2901 da0b 6d61 785f 776f 726b 6572 7329  )...max_workers)
+00000570: 01da 0865 7865 6375 746f 7229 0872 2400  ...executor).r$.
+00000580: 0000 5a07 6e75 6d5f 6173 6bda 0662 7564  ..Z.num_ask..bud
+00000590: 6765 7472 0300 0000 da12 5468 7265 6164  getr......Thread
+000005a0: 506f 6f6c 4578 6563 7574 6f72 7226 0000  PoolExecutorr&..
+000005b0: 00da 086d 696e 696d 697a 6572 2500 0000  ...minimizer%...
+000005c0: 2905 7227 0000 0072 2b00 0000 5a07 6375  ).r'...r+...Z.cu
+000005d0: 725f 6173 6b72 2a00 0000 da03 7265 6372  r_askr*.....recr
+000005e0: 0e00 0000 720e 0000 0072 2100 0000 722d  ....r....r!...r-
+000005f0: 0000 0033 0000 0073 1000 0000 0801 0c01  ...3...s........
+00000600: 1001 1401 0aff 0402 10fe 0402 7a12 4f70  ............z.Op
+00000610: 7452 756e 6e65 722e 6d69 6e69 6d69 7a65  tRunner.minimize
+00000620: 4e29 05da 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
+00000630: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+00000640: 6c6e 616d 655f 5f72 2800 0000 722d 0000  lname__r(...r-..
+00000650: 0072 0e00 0000 720e 0000 0072 0e00 0000  .r....r....r....
+00000660: 7221 0000 0072 2300 0000 2d00 0000 7306  r!...r#...-...s.
+00000670: 0000 0008 0008 010c 0572 2300 0000 69e8  .........r#...i.
+00000680: 0300 0054 da03 6263 6d72 2b00 0000 7226  ...T..bcmr+...r&
+00000690: 0000 0072 1c00 0000 721d 0000 00da 0c6f  ...r....r......o
+000006a0: 626a 5f66 756e 6374 696f 6e63 0800 0000  bj_functionc....
+000006b0: 0000 0000 0000 0000 0c00 0000 0500 0000  ................
+000006c0: 4300 0000 7362 0000 007c 0373 0574 0083  C...sb...|.s.t..
+000006d0: 007d 0374 017c 006a 027c 047c 0583 037d  .}.t.|.j.|.|...}
+000006e0: 0864 0164 0284 007d 097c 0664 0075 0072  .d.d...}.|.d.u.r
+000006f0: 177c 006a 037d 067c 0772 1e74 047c 0683  .|.j.}.|.r.t.|..
+00000700: 017d 066e 047c 097c 0683 017d 067c 067d  .}.n.|.|...}.|.}
+00000710: 0a7c 027c 087c 017c 0364 038d 037d 0b74  .|.|.|.|.d...}.t
+00000720: 057c 0b7c 0a7c 0383 0353 0029 044e 6301  .|.|.|...S.).Nc.
+00000730: 0000 0000 0000 0000 0000 0002 0000 0003  ................
+00000740: 0000 0013 0000 0073 1000 0000 8700 6601  .......s......f.
+00000750: 6401 6402 8408 7d01 7c01 5300 2903 4e63  d.d...}.|.S.).Nc
+00000760: 0000 0000 0000 0000 0000 0000 0100 0000  ................
+00000770: 0500 0000 1b00 0000 7312 0000 0074 0088  ........s....t..
+00000780: 0064 0169 007c 00a4 018e 0183 0153 0029  .d.i.|.......S.)
+00000790: 024e 720e 0000 0029 01da 0566 6c6f 6174  .Nr....)...float
+000007a0: 2901 da0a 7061 7261 6d65 7465 7273 a901  )...parameters..
+000007b0: da07 7772 6170 7065 6472 0e00 0000 7221  ..wrappedr....r!
+000007c0: 0000 00da 0d66 6c6f 6174 5f77 7261 7070  .....float_wrapp
+000007d0: 6572 4b00 0000 7302 0000 0012 017a 376f  erK...s......z7o
+000007e0: 7074 696d 697a 655f 6d6f 6465 6c2e 3c6c  ptimize_model.<l
+000007f0: 6f63 616c 733e 2e61 735f 666c 6f61 742e  ocals>.as_float.
+00000800: 3c6c 6f63 616c 733e 2e66 6c6f 6174 5f77  <locals>.float_w
+00000810: 7261 7070 6572 720e 0000 0029 0272 3700  rapperr....).r7.
+00000820: 0000 7238 0000 0072 0e00 0000 7236 0000  ..r8...r....r6..
+00000830: 0072 2100 0000 da08 6173 5f66 6c6f 6174  .r!.....as_float
+00000840: 4a00 0000 7304 0000 000c 0104 037a 206f  J...s........z o
+00000850: 7074 696d 697a 655f 6d6f 6465 6c2e 3c6c  ptimize_model.<l
+00000860: 6f63 616c 733e 2e61 735f 666c 6f61 7429  ocals>.as_float)
+00000870: 035a 0f70 6172 616d 6574 7269 7a61 7469  .Z.parametrizati
+00000880: 6f6e 722b 0000 0072 2600 0000 2906 7204  onr+...r&...).r.
+00000890: 0000 0072 2200 0000 721b 0000 00da 0d6c  ...r"...r......l
+000008a0: 6f67 6c69 6b65 6c69 686f 6f64 7206 0000  oglikelihoodr...
+000008b0: 0072 2300 0000 290c 7232 0000 0072 2b00  .r#...).r2...r+.
+000008c0: 0000 5a09 6f70 745f 636c 6173 7372 2600  ..Z.opt_classr&.
+000008d0: 0000 721c 0000 0072 1d00 0000 7233 0000  ..r....r....r3..
+000008e0: 005a 0f69 6e76 6572 745f 6675 6e63 7469  .Z.invert_functi
+000008f0: 6f6e 5a07 696e 7374 7275 6d72 3900 0000  onZ.instrumr9...
+00000900: 7225 0000 0072 2400 0000 720e 0000 0072  r%...r$...r....r
+00000910: 0e00 0000 7221 0000 00da 0e6f 7074 696d  ....r!.....optim
+00000920: 697a 655f 6d6f 6465 6c3b 0000 0073 1800  ize_model;...s..
+00000930: 0000 040a 0601 0e02 0802 0806 0601 0401  ................
+00000940: 0a01 0802 0402 0e01 0c01 723b 0000 0029  ..........r;...)
+00000950: 024e 7207 0000 0029 16da 0674 7970 696e  .Nr....)...typin
+00000960: 6772 0200 0000 da0a 636f 6e63 7572 7265  gr......concurre
+00000970: 6e74 7203 0000 00da 0f6d 756c 7469 7072  ntr......multipr
+00000980: 6f63 6573 7369 6e67 7204 0000 00da 056e  ocessingr......n
+00000990: 756d 7079 7211 0000 00da 0d65 7374 6976  umpyr......estiv
+000009a0: 616c 2e6d 6f64 656c 7205 0000 005a 0d65  al.modelr....Z.e
+000009b0: 7374 6976 616c 2e75 7469 6c73 7206 0000  stival.utilsr...
+000009c0: 00da 096e 6576 6572 6772 6164 7217 0000  ...nevergradr...
+000009d0: 0072 2200 0000 7223 0000 00da 0a6f 7074  .r"...r#.....opt
+000009e0: 696d 697a 6572 735a 054e 474f 7074 da03  imizersZ.NGOpt..
+000009f0: 696e 74da 0464 6963 74da 0373 7472 723b  int..dict..strr;
+00000a00: 0000 0072 0e00 0000 720e 0000 0072 0e00  ...r....r....r..
+00000a10: 0000 7221 0000 00da 083c 6d6f 6475 6c65  ..r!.....<module
+00000a20: 3e01 0000 0073 4000 0000 0c00 0c02 0c01  >....s@.........
+00000a30: 0801 0c02 0c01 0204 0c01 0601 0201 0a03  ................
+00000a40: 0e1b 0210 0601 0201 0201 0201 0201 0201  ................
+00000a50: 04f8 0201 02ff 0202 02fe 0204 02fc 0205  ................
+00000a60: 02fb 0206 02fa 0207 0ef9                 ..........
```

### Comparing `estival-0.2.2/estival/optimization/__pycache__/nevergrad.cpython-311.pyc` & `estival-0.2.3/estival/optimization/__pycache__/nevergrad.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `estival-0.2.2/estival/optimization/nevergrad.py` & `estival-0.2.3/estival/optimization/nevergrad.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 def optimize_model(
     bcm: BayesianCompartmentalModel,
     budget: int = 1000,
     opt_class=ng.optimizers.NGOpt,
     num_workers: int = None,
     suggested: dict = None,
     init_method: str = "midpoint",
-    obj_function=Callable,
+    obj_function: Callable = None,
     invert_function=True,
 ):
     if not num_workers:
         num_workers = cpu_count()
 
     instrum = get_instrumentation(bcm.priors, suggested, init_method)
```

### Comparing `estival-0.2.2/estival/priors.py` & `estival-0.2.3/estival/priors.py`

 * *Files identical despite different names*

### Comparing `estival-0.2.2/estival/targets.py` & `estival-0.2.3/estival/targets.py`

 * *Files 8% similar despite different names*

```diff
@@ -82,15 +82,15 @@
             n = self.target.dispersion_param
 
         # We use the parameterisation based on mean and variance and assume define var=mean**delta
         mu = modelled[self.index]
         # work out parameter p to match the distribution mean with the model output
         p = mu / (mu + n)
         # Attempt to minimize -inf showing up
-        p = jnp.where(p == 0.0, 1e-16, p)
+        p = jnp.where(p < 1e-16, 1e-16, p)
         # ll = np.sum(stats.nbinom.logpmf(self.data, n, 1.0 - p) * self.time_weights)
         ll = jsp.stats.nbinom.logpmf(self.data, n, 1.0 - p)
 
         if self.time_weights is not None:
             ll = ll * self.time_weights
             return jnp.sum(ll) * self.target.weight
         else:
@@ -203,21 +203,29 @@
 
     def evaluate(self, modelled: np.array, parameters: dict) -> float:
         if isinstance(self.target.stdev, BasePrior):
             sd = parameters[self.target.stdev.name]
         else:
             sd = self.target.stdev
 
+        from tensorflow_probability.substrates.jax import distributions as tfpd
+
+        tdist = tfpd.TruncatedNormal(
+            loc=self.data, scale=sd, low=self.target.trunc_range[0], high=self.target.trunc_range[1]
+        )
+
         distri_params = {
             "scale": sd,
             "a": (self.target.trunc_range[0] - self.data) / sd,
             "b": (self.target.trunc_range[1] - self.data) / sd,
         }
 
-        ll = jsp.stats.truncnorm.logpdf(modelled[self.index], loc=self.data, **distri_params)
+        # ll = jsp.stats.truncnorm.logpdf(modelled[self.index], loc=self.data, **distri_params)
+
+        ll = tdist.log_prob(modelled[self.index])
 
         if self.time_weights is not None:
             ll = ll * self.time_weights
             return jnp.sum(ll) * self.target.weight
         else:
             return jnp.mean(ll) * self.target.weight
```

### Comparing `estival-0.2.2/estival/utils.py` & `estival-0.2.3/estival/utils.py`

 * *Files identical despite different names*

### Comparing `estival-0.2.2/LICENSE` & `estival-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `estival-0.2.2/pyproject.toml` & `estival-0.2.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "estival"
-version = "0.2.2"
+version = "0.2.3"
 readme = "README.md"
 license = "BSD-2-Clause"
 homepage = "https://github.com/monash-emu/estival"
 repository = "https://github.com/monash-emu/estival"
 documentation = "https://github.com/monash-emu/estival"
 keywords = [
     "calibration",
@@ -23,14 +23,15 @@
 python = ">=3.8.0"
 numpy = ">=1.20.3"
 scipy = ">=1.7.3"
 arviz = ">=0.12.1"
 nevergrad = ">=0.6.0"
 pymc = ">=5.2.0"
 summerepi2 = ">=1.2.1"
+tensorflow-probability = ">=0.9.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
 black = "^20.8b0"
 pytest-parallel = "^0.1.0"
 pre-commit = "^2.19.0"
```

