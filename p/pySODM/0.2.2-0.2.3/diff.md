# Comparing `tmp/pySODM-0.2.2.tar.gz` & `tmp/pySODM-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pySODM-0.2.2.tar", last modified: Fri Jan 27 13:03:54 2023, max compression
+gzip compressed data, was "pySODM-0.2.3.tar", last modified: Thu May  4 13:55:03 2023, max compression
```

## Comparing `pySODM-0.2.2.tar` & `pySODM-0.2.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 twallema  (1001) twallema  (1001)        0 2023-01-27 13:03:54.506983 pySODM-0.2.2/
--rw-rw-r--   0 twallema  (1001) twallema  (1001)     1091 2022-11-17 15:58:03.000000 pySODM-0.2.2/LICENSE.txt
--rw-rw-r--   0 twallema  (1001) twallema  (1001)     6919 2023-01-27 13:03:54.506983 pySODM-0.2.2/PKG-INFO
--rw-rw-r--   0 twallema  (1001) twallema  (1001)     6500 2023-01-27 12:01:33.000000 pySODM-0.2.2/README.md
--rw-rw-r--   0 twallema  (1001) twallema  (1001)      107 2023-01-27 13:03:54.506983 pySODM-0.2.2/setup.cfg
--rw-r--r--   0 twallema  (1001) twallema  (1001)      947 2023-01-27 13:03:24.000000 pySODM-0.2.2/setup.py
-drwxrwxr-x   0 twallema  (1001) twallema  (1001)        0 2023-01-27 13:03:54.502983 pySODM-0.2.2/src/
-drwxrwxr-x   0 twallema  (1001) twallema  (1001)        0 2023-01-27 13:03:54.502983 pySODM-0.2.2/src/pySODM/
--rw-r--r--   0 twallema  (1001) twallema  (1001)        0 2022-11-17 15:58:03.000000 pySODM-0.2.2/src/pySODM/__init__.py
-drwxrwxr-x   0 twallema  (1001) twallema  (1001)        0 2023-01-27 13:03:54.506983 pySODM-0.2.2/src/pySODM/models/
--rw-r--r--   0 twallema  (1001) twallema  (1001)        0 2022-11-17 15:58:03.000000 pySODM-0.2.2/src/pySODM/models/__init__.py
--rw-r--r--   0 twallema  (1001) twallema  (1001)    34056 2023-01-25 18:44:03.000000 pySODM-0.2.2/src/pySODM/models/base.py
--rw-r--r--   0 twallema  (1001) twallema  (1001)     1207 2023-01-25 18:44:03.000000 pySODM-0.2.2/src/pySODM/models/utils.py
--rw-r--r--   0 twallema  (1001) twallema  (1001)    28087 2023-01-25 18:44:03.000000 pySODM-0.2.2/src/pySODM/models/validation.py
-drwxrwxr-x   0 twallema  (1001) twallema  (1001)        0 2023-01-27 13:03:54.506983 pySODM-0.2.2/src/pySODM/optimization/
--rw-r--r--   0 twallema  (1001) twallema  (1001)        0 2022-11-17 15:58:03.000000 pySODM-0.2.2/src/pySODM/optimization/__init__.py
--rw-r--r--   0 twallema  (1001) twallema  (1001)    12466 2023-01-19 20:36:31.000000 pySODM-0.2.2/src/pySODM/optimization/mcmc.py
--rw-r--r--   0 twallema  (1001) twallema  (1001)     7502 2023-01-27 12:01:33.000000 pySODM-0.2.2/src/pySODM/optimization/nelder_mead.py
--rw-r--r--   0 twallema  (1001) twallema  (1001)    53384 2023-01-27 12:01:33.000000 pySODM-0.2.2/src/pySODM/optimization/objective_functions.py
--rw-r--r--   0 twallema  (1001) twallema  (1001)     9879 2023-01-27 12:01:33.000000 pySODM-0.2.2/src/pySODM/optimization/pso.py
--rw-r--r--   0 twallema  (1001) twallema  (1001)    14915 2022-12-22 15:15:26.000000 pySODM-0.2.2/src/pySODM/optimization/utils.py
--rw-r--r--   0 twallema  (1001) twallema  (1001)     3979 2022-11-17 15:58:03.000000 pySODM-0.2.2/src/pySODM/optimization/visualization.py
-drwxrwxr-x   0 twallema  (1001) twallema  (1001)        0 2023-01-27 13:03:54.502983 pySODM-0.2.2/src/pySODM.egg-info/
--rw-rw-r--   0 twallema  (1001) twallema  (1001)     6919 2023-01-27 13:03:54.000000 pySODM-0.2.2/src/pySODM.egg-info/PKG-INFO
--rw-rw-r--   0 twallema  (1001) twallema  (1001)      606 2023-01-27 13:03:54.000000 pySODM-0.2.2/src/pySODM.egg-info/SOURCES.txt
--rw-rw-r--   0 twallema  (1001) twallema  (1001)        1 2023-01-27 13:03:54.000000 pySODM-0.2.2/src/pySODM.egg-info/dependency_links.txt
--rw-rw-r--   0 twallema  (1001) twallema  (1001)      125 2023-01-27 13:03:54.000000 pySODM-0.2.2/src/pySODM.egg-info/requires.txt
--rw-rw-r--   0 twallema  (1001) twallema  (1001)        7 2023-01-27 13:03:54.000000 pySODM-0.2.2/src/pySODM.egg-info/top_level.txt
+drwxrwxr-x   0 twallema  (1001) twallema  (1001)        0 2023-05-04 13:55:03.282010 pySODM-0.2.3/
+-rw-r--r--   0 twallema  (1001) twallema  (1001)     1091 2023-01-27 13:41:47.000000 pySODM-0.2.3/LICENSE.txt
+-rw-rw-r--   0 twallema  (1001) twallema  (1001)     7062 2023-05-04 13:55:03.282010 pySODM-0.2.3/PKG-INFO
+-rw-rw-r--   0 twallema  (1001) twallema  (1001)     6662 2023-05-04 13:54:54.000000 pySODM-0.2.3/README.md
+-rw-r--r--   0 twallema  (1001) twallema  (1001)      107 2023-05-04 13:55:03.282010 pySODM-0.2.3/setup.cfg
+-rw-r--r--   0 twallema  (1001) twallema  (1001)      947 2023-05-04 13:54:54.000000 pySODM-0.2.3/setup.py
+drwxrwxr-x   0 twallema  (1001) twallema  (1001)        0 2023-05-04 13:55:03.282010 pySODM-0.2.3/src/
+drwxrwxr-x   0 twallema  (1001) twallema  (1001)        0 2023-05-04 13:55:03.282010 pySODM-0.2.3/src/pySODM/
+-rw-r--r--   0 twallema  (1001) twallema  (1001)        0 2023-01-27 13:41:47.000000 pySODM-0.2.3/src/pySODM/__init__.py
+drwxrwxr-x   0 twallema  (1001) twallema  (1001)        0 2023-05-04 13:55:03.282010 pySODM-0.2.3/src/pySODM/models/
+-rw-r--r--   0 twallema  (1001) twallema  (1001)        0 2022-11-17 15:58:03.000000 pySODM-0.2.3/src/pySODM/models/__init__.py
+-rw-r--r--   0 twallema  (1001) twallema  (1001)    36410 2023-05-04 13:39:37.000000 pySODM-0.2.3/src/pySODM/models/base.py
+-rw-r--r--   0 twallema  (1001) twallema  (1001)     1206 2023-04-05 14:11:59.000000 pySODM-0.2.3/src/pySODM/models/utils.py
+-rw-r--r--   0 twallema  (1001) twallema  (1001)    28480 2023-05-04 13:39:37.000000 pySODM-0.2.3/src/pySODM/models/validation.py
+drwxrwxr-x   0 twallema  (1001) twallema  (1001)        0 2023-05-04 13:55:03.282010 pySODM-0.2.3/src/pySODM/optimization/
+-rw-r--r--   0 twallema  (1001) twallema  (1001)        0 2022-11-17 15:58:03.000000 pySODM-0.2.3/src/pySODM/optimization/__init__.py
+-rw-r--r--   0 twallema  (1001) twallema  (1001)    12481 2023-03-26 10:32:10.000000 pySODM-0.2.3/src/pySODM/optimization/mcmc.py
+-rw-r--r--   0 twallema  (1001) twallema  (1001)     7510 2023-03-22 16:27:18.000000 pySODM-0.2.3/src/pySODM/optimization/nelder_mead.py
+-rw-r--r--   0 twallema  (1001) twallema  (1001)    53814 2023-04-11 11:02:41.000000 pySODM-0.2.3/src/pySODM/optimization/objective_functions.py
+-rw-r--r--   0 twallema  (1001) twallema  (1001)     9879 2023-01-27 12:01:33.000000 pySODM-0.2.3/src/pySODM/optimization/pso.py
+-rw-r--r--   0 twallema  (1001) twallema  (1001)    14915 2022-12-22 15:15:26.000000 pySODM-0.2.3/src/pySODM/optimization/utils.py
+-rw-r--r--   0 twallema  (1001) twallema  (1001)     3979 2023-03-28 15:17:24.000000 pySODM-0.2.3/src/pySODM/optimization/visualization.py
+drwxrwxr-x   0 twallema  (1001) twallema  (1001)        0 2023-05-04 13:55:03.282010 pySODM-0.2.3/src/pySODM.egg-info/
+-rw-rw-r--   0 twallema  (1001) twallema  (1001)     7062 2023-05-04 13:55:03.000000 pySODM-0.2.3/src/pySODM.egg-info/PKG-INFO
+-rw-rw-r--   0 twallema  (1001) twallema  (1001)      606 2023-05-04 13:55:03.000000 pySODM-0.2.3/src/pySODM.egg-info/SOURCES.txt
+-rw-rw-r--   0 twallema  (1001) twallema  (1001)        1 2023-05-04 13:55:03.000000 pySODM-0.2.3/src/pySODM.egg-info/dependency_links.txt
+-rw-rw-r--   0 twallema  (1001) twallema  (1001)      125 2023-05-04 13:55:03.000000 pySODM-0.2.3/src/pySODM.egg-info/requires.txt
+-rw-rw-r--   0 twallema  (1001) twallema  (1001)        7 2023-05-04 13:55:03.000000 pySODM-0.2.3/src/pySODM.egg-info/top_level.txt
```

### Comparing `pySODM-0.2.2/LICENSE.txt` & `pySODM-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pySODM-0.2.2/PKG-INFO` & `pySODM-0.2.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,83 +1,88 @@
 Metadata-Version: 2.1
 Name: pySODM
-Version: 0.2.2
+Version: 0.2.3
 Summary: Simulating and Optimising Dynamical Models
 Home-page: https://github.com/twallema/pySODM
 Author: Tijs Alleman, KERMIT, Ghent University
 Author-email: tijs.alleman@ugent.be
 License: MIT
 Keywords: ODE PDE simulation calibration gillespie xarray emcee
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: develop
 License-File: LICENSE.txt
 
 ## pySODM
 *Simulating and Optimising Dynamical Models in Python 3*
 
-![build](https://github.com/twallema/pySODM/actions/workflows/tests.yml/badge.svg) ![docs](https://github.com/twallema/pySODM/actions/workflows/deploy.yml/badge.svg)
+![build](https://github.com/twallema/pySODM/actions/workflows/tests.yml/badge.svg) ![docs](https://github.com/twallema/pySODM/actions/workflows/deploy.yml/badge.svg) [![HitCount](https://hits.dwyl.com/twallema/pySODM.svg)](https://hits.dwyl.com/twallema/pySODM)
 
-### Links
+### Quick installation 
+```
+pip install pySODM
+```
+### Resources
 
 Documentation: https://twallema.github.io/pySODM
 
 Manuscript: https://arxiv.org/abs/2301.10664
 
+pyPI: https://pypi.org/project/pySODM/ 
+
 ### Aim & Scope
 
 A modeling and simulation workflow will typically constitute the following steps (see [Villaverde et. al](https://doi.org/10.1093/bib/bbab387)),
 1. Build a system dynamical model to describe some real-world phenomenon. Assess structural identifiability.
 2. Calibrate the model to a set of experimental data.
 3. Extract knowledge from the calibrated parameter values (assess practical identifiability).
 4. Use the model to make projections outside the calibrated range.
 
-The aim of pySODM is to reduce the time it takes to step through this workflow. pySODM is a template to construct, simulate and calibrate dynamical systems governed by differential equations. Models can have n-dimensional labeled states of different sizes and can be simulated deterministically and stochastically. Model parameters can be time-dependent by means of complex functions
+The aim of pySODM is to reduce the time it takes to step through this workflow. pySODM provides a *template* to construct, simulate and calibrate dynamical systems governed by differential equations. Models can have n-dimensional labeled states of different sizes and can be simulated deterministically and stochastically. Model parameters can be time-dependent by means of complex functions
 with arbitrary inputs. The labeled n-dimensional model states can be aligned with n-dimensional
 data to compute the posterior probability function, which can subsequently be optimised.
 
 ### Overview of features
 
 | Workflow                     | Features                                                                                                                        |
 |------------------------------|---------------------------------------------------------------------------------------------------------------------------------|
-| Building a model     | Solve coupled systems of equations deterministically (integration) or stochastically (Gillespie's SSA and Tau-Leaping)                  |
-|                              | n-Dimensional model states with coordinates. Different states can have different sizes.                                         |
-|                              | Easy indexing, manipulating, saving, and piping to third-party software of model output by formatting simulation output as `xarray.Dataset` |
-| Simulating a model   | Vary model parameters during the simulation in accordance with an arbitrarily complex function containing any input                     |
-|                              | Use *draw functions* to perform repeated simulations for sensitivity analysis. With multiprocessing support                     |
-| Calibrating a model  | Calibration of n-dimensional model parameters                                                                                           |
-|                              | Construct a posterior probability function                                                                                      |
-|                              | Automatic alignment of data and model prediction over timesteps and dimensions                                                  |
-|                              | Nelder-Mead Simplex and Particle Swarm Optimization for frequentist optimization                                                |
-|                              | Pipeline to and backend for `emcee.EnsembleSampler` to perform Bayesian inference of model parameters                           |
-|                              | Analysis of the mean-variance ratio in count-based datasets to aid in the choice of an appropriate likelihood function          |
+| Construct a dynamical model     | Implement coupled systems of differential equations            |
+|                                 | States can be n-dimensional and of different sizes, allowing users to build models with subprocesses                                       |
+|                                 | Allows n-dimensional model states to be labelled with coordinates and dimensions by using `xarray.Dataset}` to store simulation output |
+|                                 | Easy indexing, manipulating, saving, and piping to third-party software of model output by formatting simulation output as `xarray.Dataset` |
+| Simulating the model            | Continuous and discrete deterministic simulation or discrete stochastic simulation (Gillespie's Stochastic Simulation Algorithm or Tau-Leaping) |
+|                                 | Vary model parameters during the simulation generically using a complex function |
+|                                 | Use *draw functions* to perform repeated simulations for sensitivity analysis. With multiprocessing support |
+| Calibrate the model             | Construct and maximize a posterior probability function  |
+|                                 | Automatic alignment of data and model forecast over timesteps and coordinates  |
+|                                 | Nelder-Mead Simplex and Particle Swarm Optimization for point estimation of model parameters |
+|                                 | Pipeline to and backend for `emcee.EnsembleSampler` to perform Bayesian inference of model parameters                           |
 
 ### Getting started
 
 The [quistart tutorial](quickstart.md) will teach you the basics of building and simulating models with n-dimensional labeled states in pySODM. It will demonstrate how to vary model parameters over the course of a simulation and how to perform repeated simulations with sampling of model parameters.
 
 The [workflow](worfklow.md) tutorial provides a step-by-step introduction to a modeling and simulation workflow by inferring the distributions of the model parameters of a simple compartmental disease model using a synthetic dataset. 
 
 The [enzyme kinetics](enzyme_kinetics.md) and [influenza 17-18](influenza_1718.md) case studies apply the modeling and simulation workflow to more advanced, real-world problems. In the enzyme kinetics case study, a 1D packed-bed reactor model is implemented in pySODM by reducing the two PDEs to a set of coupled ODEs by using the method-of-lines. In the Influenza 17-18 case study, a stochastic, age-structured model for influenza is developped and calibrated to the Influenza incidence data reported by the Belgian Federal Institute of Public Health. These case studies mainly serve to demonstrate pySODM's capabilities across scientific disciplines and highlight the arbitrarily complex nature of the models that can be built with pySODM. For an academic description of pySODM and on the Enzyme Kinetics and Influenza 17-18 case studies, checkout our [manuscript](https://arxiv.org/abs/2301.10664).
 
 ### Versions
 
 - Version 0.2.0 (2023-01-19, PR #25)
     > Introduction of `state_dimensions` in model declaration, allowing the user to define models where states can have different sizes.
     - Version 0.2.1 (2023-01-27, PR #30)
-        > Fixed bugs when using pySODM for the COVID-19 related models. More thorough checks on `bounds` in the log posterior probability function. Finished manuscript.
+        > Fixed bugs encountered when incorporating pySODM into the SARS-CoV-2 Dynamic Transmission Models. More thorough checks on `bounds` in the log posterior probability function. Finished manuscript.
+    - Version 0.2.2 (2023-01-27, PR #31)
+        > Published to pyPI.
+    - Version 0.2.3 (2023-05-04, PR #46)
+        > Fixed minor bugs encountered when using pySODM for a dynamic input-output model of the Belgian economy. Published to pyPI.
 - Version 0.1 (2022-12-23, PR #14)
     > Application pySODM to three use cases. Documentation website. Unit tests for ODEModel, SDEModel and calibration. 
     - Version 0.1.1 (2023-01-09, PR #20)
         > Start of semantic versions: Major.Minor.Patch
     - Version 0.1.2 (2023-01-11, PR #23)
         > Calibration of 1-D model parameters generalized to n-dimensions.
         > Added 'aggregation functions' to the `log_posterior_probability` class to perform custom aggregations of model output before matching with data.
         > `xarray.DataArray`/`xarray.Dataset` can be used as datasets during calibration. Internally converted to `pd.DataFrame`.
 - Version 0.0 (2022-11-14)
     - First pySODM version. Obtained by splitting the generally applicable parts from the ad-hoc parts in UGentBiomath/COVID19-Model. Without documentation website. 
 - Pre-development (2020-05-01 - 2022-11-24)
     - Code developped to model the spread of SARS-CoV-2 in Belgium (UGentBiomath/COVID19-Model).
-
-[![HitCount](https://hits.dwyl.com/twallema/pySODM.svg)](https://hits.dwyl.com/twallema/pySODM)
-
-
```

### Comparing `pySODM-0.2.2/README.md` & `pySODM-0.2.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,67 +1,75 @@
 ## pySODM
 *Simulating and Optimising Dynamical Models in Python 3*
 
-![build](https://github.com/twallema/pySODM/actions/workflows/tests.yml/badge.svg) ![docs](https://github.com/twallema/pySODM/actions/workflows/deploy.yml/badge.svg)
+![build](https://github.com/twallema/pySODM/actions/workflows/tests.yml/badge.svg) ![docs](https://github.com/twallema/pySODM/actions/workflows/deploy.yml/badge.svg) [![HitCount](https://hits.dwyl.com/twallema/pySODM.svg)](https://hits.dwyl.com/twallema/pySODM)
 
-### Links
+### Quick installation 
+```
+pip install pySODM
+```
+### Resources
 
 Documentation: https://twallema.github.io/pySODM
 
 Manuscript: https://arxiv.org/abs/2301.10664
 
+pyPI: https://pypi.org/project/pySODM/ 
+
 ### Aim & Scope
 
 A modeling and simulation workflow will typically constitute the following steps (see [Villaverde et. al](https://doi.org/10.1093/bib/bbab387)),
 1. Build a system dynamical model to describe some real-world phenomenon. Assess structural identifiability.
 2. Calibrate the model to a set of experimental data.
 3. Extract knowledge from the calibrated parameter values (assess practical identifiability).
 4. Use the model to make projections outside the calibrated range.
 
-The aim of pySODM is to reduce the time it takes to step through this workflow. pySODM is a template to construct, simulate and calibrate dynamical systems governed by differential equations. Models can have n-dimensional labeled states of different sizes and can be simulated deterministically and stochastically. Model parameters can be time-dependent by means of complex functions
+The aim of pySODM is to reduce the time it takes to step through this workflow. pySODM provides a *template* to construct, simulate and calibrate dynamical systems governed by differential equations. Models can have n-dimensional labeled states of different sizes and can be simulated deterministically and stochastically. Model parameters can be time-dependent by means of complex functions
 with arbitrary inputs. The labeled n-dimensional model states can be aligned with n-dimensional
 data to compute the posterior probability function, which can subsequently be optimised.
 
 ### Overview of features
 
 | Workflow                     | Features                                                                                                                        |
 |------------------------------|---------------------------------------------------------------------------------------------------------------------------------|
-| Building a model     | Solve coupled systems of equations deterministically (integration) or stochastically (Gillespie's SSA and Tau-Leaping)                  |
-|                              | n-Dimensional model states with coordinates. Different states can have different sizes.                                         |
-|                              | Easy indexing, manipulating, saving, and piping to third-party software of model output by formatting simulation output as `xarray.Dataset` |
-| Simulating a model   | Vary model parameters during the simulation in accordance with an arbitrarily complex function containing any input                     |
-|                              | Use *draw functions* to perform repeated simulations for sensitivity analysis. With multiprocessing support                     |
-| Calibrating a model  | Calibration of n-dimensional model parameters                                                                                           |
-|                              | Construct a posterior probability function                                                                                      |
-|                              | Automatic alignment of data and model prediction over timesteps and dimensions                                                  |
-|                              | Nelder-Mead Simplex and Particle Swarm Optimization for frequentist optimization                                                |
-|                              | Pipeline to and backend for `emcee.EnsembleSampler` to perform Bayesian inference of model parameters                           |
-|                              | Analysis of the mean-variance ratio in count-based datasets to aid in the choice of an appropriate likelihood function          |
+| Construct a dynamical model     | Implement coupled systems of differential equations            |
+|                                 | States can be n-dimensional and of different sizes, allowing users to build models with subprocesses                                       |
+|                                 | Allows n-dimensional model states to be labelled with coordinates and dimensions by using `xarray.Dataset}` to store simulation output |
+|                                 | Easy indexing, manipulating, saving, and piping to third-party software of model output by formatting simulation output as `xarray.Dataset` |
+| Simulating the model            | Continuous and discrete deterministic simulation or discrete stochastic simulation (Gillespie's Stochastic Simulation Algorithm or Tau-Leaping) |
+|                                 | Vary model parameters during the simulation generically using a complex function |
+|                                 | Use *draw functions* to perform repeated simulations for sensitivity analysis. With multiprocessing support |
+| Calibrate the model             | Construct and maximize a posterior probability function  |
+|                                 | Automatic alignment of data and model forecast over timesteps and coordinates  |
+|                                 | Nelder-Mead Simplex and Particle Swarm Optimization for point estimation of model parameters |
+|                                 | Pipeline to and backend for `emcee.EnsembleSampler` to perform Bayesian inference of model parameters                           |
 
 ### Getting started
 
 The [quistart tutorial](quickstart.md) will teach you the basics of building and simulating models with n-dimensional labeled states in pySODM. It will demonstrate how to vary model parameters over the course of a simulation and how to perform repeated simulations with sampling of model parameters.
 
 The [workflow](worfklow.md) tutorial provides a step-by-step introduction to a modeling and simulation workflow by inferring the distributions of the model parameters of a simple compartmental disease model using a synthetic dataset. 
 
 The [enzyme kinetics](enzyme_kinetics.md) and [influenza 17-18](influenza_1718.md) case studies apply the modeling and simulation workflow to more advanced, real-world problems. In the enzyme kinetics case study, a 1D packed-bed reactor model is implemented in pySODM by reducing the two PDEs to a set of coupled ODEs by using the method-of-lines. In the Influenza 17-18 case study, a stochastic, age-structured model for influenza is developped and calibrated to the Influenza incidence data reported by the Belgian Federal Institute of Public Health. These case studies mainly serve to demonstrate pySODM's capabilities across scientific disciplines and highlight the arbitrarily complex nature of the models that can be built with pySODM. For an academic description of pySODM and on the Enzyme Kinetics and Influenza 17-18 case studies, checkout our [manuscript](https://arxiv.org/abs/2301.10664).
 
 ### Versions
 
 - Version 0.2.0 (2023-01-19, PR #25)
     > Introduction of `state_dimensions` in model declaration, allowing the user to define models where states can have different sizes.
     - Version 0.2.1 (2023-01-27, PR #30)
-        > Fixed bugs when using pySODM for the COVID-19 related models. More thorough checks on `bounds` in the log posterior probability function. Finished manuscript.
+        > Fixed bugs encountered when incorporating pySODM into the SARS-CoV-2 Dynamic Transmission Models. More thorough checks on `bounds` in the log posterior probability function. Finished manuscript.
+    - Version 0.2.2 (2023-01-27, PR #31)
+        > Published to pyPI.
+    - Version 0.2.3 (2023-05-04, PR #46)
+        > Fixed minor bugs encountered when using pySODM for a dynamic input-output model of the Belgian economy. Published to pyPI.
 - Version 0.1 (2022-12-23, PR #14)
     > Application pySODM to three use cases. Documentation website. Unit tests for ODEModel, SDEModel and calibration. 
     - Version 0.1.1 (2023-01-09, PR #20)
         > Start of semantic versions: Major.Minor.Patch
     - Version 0.1.2 (2023-01-11, PR #23)
         > Calibration of 1-D model parameters generalized to n-dimensions.
         > Added 'aggregation functions' to the `log_posterior_probability` class to perform custom aggregations of model output before matching with data.
         > `xarray.DataArray`/`xarray.Dataset` can be used as datasets during calibration. Internally converted to `pd.DataFrame`.
 - Version 0.0 (2022-11-14)
     - First pySODM version. Obtained by splitting the generally applicable parts from the ad-hoc parts in UGentBiomath/COVID19-Model. Without documentation website. 
 - Pre-development (2020-05-01 - 2022-11-24)
-    - Code developped to model the spread of SARS-CoV-2 in Belgium (UGentBiomath/COVID19-Model).
-
-[![HitCount](https://hits.dwyl.com/twallema/pySODM.svg)](https://hits.dwyl.com/twallema/pySODM)
+    - Code developped to model the spread of SARS-CoV-2 in Belgium (UGentBiomath/COVID19-Model).
```

### Comparing `pySODM-0.2.2/setup.py` & `pySODM-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages, setup
 
 setup(
     name='pySODM',
     packages=find_packages("src", exclude=["*.tests"]),
     package_dir={'': 'src'},
-    version='0.2.2',
+    version='0.2.3',
     description='Simulating and Optimising Dynamical Models',
     author='Tijs Alleman, KERMIT, Ghent University',
     author_email='tijs.alleman@ugent.be',
     keywords='ODE PDE simulation calibration gillespie xarray emcee',
     url='https://github.com/twallema/pySODM',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

### Comparing `pySODM-0.2.2/src/pySODM/models/base.py` & `pySODM-0.2.3/src/pySODM/models/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,86 +14,14 @@
 from scipy.integrate import solve_ivp
 from pySODM.models.utils import int_to_date, list_to_dict
 from pySODM.models.validation import merge_parameter_names_parameter_stratified_names, validate_draw_function, validate_simulation_time, validate_dimensions, \
                                         validate_time_dependent_parameters, validate_integrate, check_duplicates, build_state_sizes_dimensions, validate_state_dimensions, \
                                             validate_initial_states, validate_integrate_or_compute_rates_signature, validate_provided_parameters, validate_parameter_stratified_sizes, \
                                                 validate_apply_transitionings_signature, validate_compute_rates, validate_apply_transitionings
 
-def _output_to_xarray_dataset(output, state_shapes, state_dimensions, state_coordinates, actual_start_date=None):
-    """
-    Convert array (returned by scipy) to an xarray Dataset with the right coordinates and variable names
-
-    Parameters
-    ----------
-
-    output: dict
-        Keys: "y" (states) and "t" (timesteps)
-        Size of `y`: (total number of states, number of timesteps)
-        Size of `t`: number of timesteps
-
-    state_shapes: dict
-        Keys: state names. Values: tuples with state shape
-
-    state_dimensions: dict
-        Keys: state names. Values: list containing dimensions associated with state
-
-    state_coordinates: dict
-        Keys: state names. Values: list containing coordinates of every dimension the state is associated with
-
-    actual_start_date: datetime
-        Used to determine if the time output should be returned as dates
-
-    Returns
-    -------
-
-    output: xarray.Dataset
-        Simulation results
-    """
-
-    # Convert scipy's output to a dictionary of states with the correct sizes
-    new_state_shapes={}
-    for k,v in state_shapes.items():
-        v=list(v)
-        v.append(len(output["t"]))
-        new_state_shapes.update({k: tuple(v)})
-    output_flat = np.ravel(output["y"])
-    data_variables = list_to_dict(output_flat, new_state_shapes)
-
-    # Append the time dimension
-    new_state_dimensions={}
-    for k,v in state_dimensions.items():
-        v_acc = v.copy()
-        if actual_start_date is not None:
-            v_acc.append('date')
-            new_state_dimensions.update({k: v_acc})
-        else:
-            v_acc.append('time')
-            new_state_dimensions.update({k: v_acc})
-
-    # Append the time coordinates
-    new_state_coordinates={}
-    for k,v in state_coordinates.items():
-        v_acc=v.copy()
-        if actual_start_date is not None:
-            v_acc.append(actual_start_date + pd.to_timedelta(output["t"], unit='D'))
-            new_state_coordinates.update({k: v_acc})
-        else:
-            v_acc.append(output["t"])
-            new_state_coordinates.update({k: v_acc})
-
-    # Build the xarray dataset
-    data = {}
-    for var, arr in data_variables.items():
-        if len(new_state_dimensions[var]) == 1:
-            arr = np.ravel(arr)
-        xarr = xarray.DataArray(arr, dims=new_state_dimensions[var], coords=new_state_coordinates[var])
-        data[var] = xarr
-
-    return xarray.Dataset(data)
-
 class SDEModel:
     """
     Initialise a stochastic differential equations model
 
     Parameters
     ----------
     To initialise the model, provide following inputs:
@@ -410,23 +338,23 @@
 
                 return np.asarray(out), tau
 
         return func
 
     def _solve_discrete(self, fun, t_eval, y, args):
         # Preparations
-        y = np.reshape(y, [y.size,1])
+        y = np.reshape(y, [len(y),1])
         y_prev=y
         # Simulation loop
         t_lst=[t_eval[0]]
         t = t_eval[0]
         while t < t_eval[-1]:
             out, tau = fun(t, y_prev, args)
             y_prev = out
-            out = np.reshape(out,[out.size,1])
+            out = np.reshape(out,[len(out),1])
             y = np.append(y,out,axis=1)
             t = t + tau
             t_lst.append(t)
         # Interpolate output y to times t_eval
         y_eval = np.zeros([y.shape[0], len(t_eval)])
         for row_idx in range(y.shape[0]):
             y_eval[row_idx,:] = np.interp(t_eval, t_lst, y[row_idx,:])
@@ -455,61 +383,73 @@
     def _mp_sim_single(self, drawn_parameters, time, actual_start_date, method, tau, output_timestep):
         """
         A Multiprocessing-compatible wrapper for _sim_single, assigns the drawn dictionary and runs _sim_single
         """
         self.parameters.update(drawn_parameters)
         return self._sim_single(time, actual_start_date, method, tau, output_timestep)
 
-    def sim(self, time, warmup=0, N=1, draw_function=None, samples=None, method='tau_leap', tau=0.5, output_timestep=1, processes=None):
+    def sim(self, time, warmup=0, N=1, draw_function=None, samples=None, processes=None, method='tau_leap', tau=0.5, output_timestep=1):
 
         """
         Run a model simulation for the given time period. Can optionally perform N repeated simulations of time days.
         Can change the values of model parameters at every repeated simulation by drawing samples from a dictionary `samples` using a function `draw_function`
 
-
         Parameters
         ----------
+
         time : 1) int/float, 2) list of int/float of type '[start_time, stop_time]', 3) list of pd.Timestamp or str of type '[start_date, stop_date]',
             The start and stop "time" for the simulation run.
             1) Input is converted to [0, time]. Floats are automatically rounded.
             2) Input is interpreted as [start_time, stop_time]. Time axis in xarray output is named 'time'. Floats are automatically rounded.
             3) Input is interpreted as [start_date, stop_date]. Time axis in xarray output is named 'date'. Floats are automatically rounded.
 
         warmup : int
             Number of days to simulate prior to start time or date
 
         N : int
-            Number of repeated simulations (useful for stochastic models). One by default.
+            Number of repeated simulations (default: 1)
 
         draw_function : function
-            A function which takes as its input the dictionary of model parameters and a samples dictionary
-            and the dictionary of sampled parameter values and assings these samples to the model parameter dictionary ad random.
+            A function with as obligatory inputs the dictionary of model parameters and a dictionary of samples
+            The function can alter parameters in the model parameters dictionary between repeated simulations `N`.
+            Usefull to propagate uncertainty, perform sensitivity analysis.
 
         samples : dictionary
-            Sample dictionary used by draw_function. Does not need to be supplied if samples_dict is not used in draw_function.
+            Sample dictionary used by `draw_function`.
+
+        processes: int
+            Number of cores to distribute the `N` draws over
 
         method: str
-            Stochastic simulation method. Either 'Stochastic Simulation Algorithm' (SSA), or its tau-leaping approximation (tau_leap).
-        
+            Stochastic simulation method. Either 'Stochastic Simulation Algorithm' ('SSA'), or its tau-leaping approximation ('tau_leap').
+    
         tau: int/float
-            Timestep used by the tau-leaping algorithm
+            Timestep used by the tau-leaping algorithm (default: 0.5)
 
         output_timestep: int/flat
             Interpolate model output to every `output_timestep` time
             For datetimes: expressed in days
 
-        processes: int
-            Number of cores to distribute the N draws over.
-
         Returns
         -------
-        xarray.Dataset
 
+        output: xarray.Dataset
+            Simulation output
         """
 
+        # Input checks on solution method and timestep
+        if not isinstance(method, str):
+            raise TypeError(
+                "solver method 'method' must be of type string"
+                )
+        if not isinstance(tau, (int,float)):
+            raise TypeError(
+                "discrete timestep 'tau' must be of type int or float"
+                )
+
         # Input checks on supplied simulation time
         time, actual_start_date = validate_simulation_time(time, warmup)
 
         # Input check on draw function
         if draw_function:
             validate_draw_function(draw_function, self.parameters, samples)
 
@@ -683,105 +623,145 @@
             for d in dstates:
                 out.extend(list(np.ravel(d)))
 
             return out
 
         return func
 
-    def _sim_single(self, time, actual_start_date=None, method='RK23', rtol=5e-3, output_timestep=1):
-        """"""
+    def _solve_discrete(self, fun, tau, t_eval, y, args):
+        # Preparations
+        y = np.reshape(y, [len(y),1])
+        y_prev=y
+        # Simulation loop
+        t_lst=[t_eval[0]]
+        t = t_eval[0]
+        while t < t_eval[-1]:
+            out = fun(t, y_prev, args)
+            out = np.reshape(out,[len(out),1])*tau
+            y = np.append(y,y_prev+out,axis=1)
+            y_prev += out
+            t = t + tau
+            t_lst.append(t)
+        # Interpolate output y to times t_eval
+        y_eval = np.zeros([y.shape[0], len(t_eval)])
+        for row_idx in range(y.shape[0]):
+            y_eval[row_idx,:] = np.interp(t_eval, t_lst, y[row_idx,:])
+            
+        return {'y': y_eval, 't': t_eval}
+
+    def _sim_single(self, time, actual_start_date=None, method='RK23', rtol=5e-3, output_timestep=1, tau=None):
+        """
+        Integrates the model over the interval time = [t0, t1] and builds the xarray output. Integration is either continuous (default) or discrete (tau != None).
+        """
 
         # Create scipy-compatible wrapper
         fun = self._create_fun(actual_start_date)
 
         # Construct vector of timesteps
         t0, t1 = time
         t_eval = np.arange(start=t0, stop=t1 + output_timestep, step=output_timestep)
 
         # Flatten initial states
         y0=[]
         for v in self.initial_states.values():
             y0.extend(list(np.ravel(v)))
 
-        # Get output
-        output = solve_ivp(fun, time, y0, args=[self.parameters], t_eval=t_eval, method=method, rtol=rtol)
+        if tau:
+            output = self._solve_discrete(fun, tau, t_eval, y0, args=self.parameters)
+        else:
+            output = solve_ivp(fun, time, y0, args=[self.parameters], t_eval=t_eval, method=method, rtol=rtol)
 
         # Map to variable names
         return _output_to_xarray_dataset(output, self.state_shapes, self.state_dimensions, self.state_coordinates, actual_start_date)
 
-    def _mp_sim_single(self, drawn_parameters, time, actual_start_date, method, rtol, output_timestep):
+    def _mp_sim_single(self, drawn_parameters, time, actual_start_date, method, rtol, output_timestep, tau):
         """
         A `multiprocessing`-compatible wrapper for `_sim_single`, assigns the drawn dictionary and runs `_sim_single`
         """
         self.parameters.update(drawn_parameters)
-        out = self._sim_single(time, actual_start_date, method, rtol, output_timestep)
+        out = self._sim_single(time, actual_start_date, method, rtol, output_timestep, tau)
         return out
 
-    def sim(self, time, warmup=0, N=1, draw_function=None, samples=None, method='RK23', output_timestep=1, rtol=1e-3, processes=None):
+    def sim(self, time, warmup=0, N=1, draw_function=None, samples=None, processes=None, method='RK23', rtol=1e-3, tau=None, output_timestep=1):
         """
-        Run a model simulation for the given time period. Can optionally perform `N` repeated simulations of time days.
-        Can change the values of model parameters at every repeated simulation by drawing samples from a dictionary `samples` using a function `draw_function`
+        Run a model simulation for a given time period. Can optionally perform `N` repeated simulations with sampling of model parameters from a dictionary `samples` using a function `draw_function`. Can perform discrete timestepping if `tau != None`.
 
         Parameters
         ----------
+
         time : 1) int/float, 2) list of int/float of type '[start_time, stop_time]', 3) list of pd.Timestamp or str of type '[start_date, stop_date]',
             The start and stop "time" for the simulation run.
             1) Input is converted to [0, time]. Floats are automatically rounded.
             2) Input is interpreted as [start_time, stop_time]. Time axis in xarray output is named 'time'. Floats are automatically rounded.
             3) Input is interpreted as [start_date, stop_date]. Time axis in xarray output is named 'date'. Floats are automatically rounded.
 
         warmup : int
             Number of days to simulate prior to start time or date
 
         N : int
-            Number of repeated simulations (useful for stochastic models). One by default.
+            Number of repeated simulations (default: 1)
 
         draw_function : function
-            A function which takes as its input the dictionary of model parameters and a samples dictionary
-            and the dictionary of sampled parameter values and assings these samples to the model parameter dictionary ad random.
+            A function with as obligatory inputs the dictionary of model parameters and a dictionary of samples
+            The function can alter parameters in the model parameters dictionary between repeated simulations `N`.
+            Usefull to propagate uncertainty, perform sensitivity analysis.
 
         samples : dictionary
-            Sample dictionary used by draw_function. Does not need to be supplied if samples_dict is not used in draw_function.
+            Sample dictionary used by `draw_function`.
 
         processes: int
-            Number of cores to distribute the N draws over.
+            Number of cores to distribute the `N` draws over.
 
         method: str
             Method used by Scipy `solve_ivp` for integration of differential equations. Default: 'RK23'.
+
+        rtol: float
+            Relative tolerance of Scipy `solve_ivp`. Default: 1e-3.
         
+        tau: int/float
+            If `tau != None`, the integrator (`scipy.solve_ivp()`) is overwritten and a discrete timestepper with timestep `tau` is used. (default:None)
+
         output_timestep: int/flat
             Interpolate model output to every `output_timestep` time
             For datetimes: expressed in days
 
-        rtol: float
-            Relative tolerance of Scipy `solve_ivp`. Default: 1e-3. Quick and dirty: 5e-3.
-
         Returns
         -------
-        xarray.Dataset
 
+        output: xarray.Dataset
+            Simulation output
         """
 
         # Input checks on solver settings
         if not isinstance(rtol, float):
             raise TypeError(
-                "Relative solver tolerance 'rtol' must be of type float"
-            )
+                "relative solver tolerance 'rtol' must be of type float"
+                )
         if not isinstance(method, str):
             raise TypeError(
-                "Solver method 'method' must be of type string"
-            )
+                "solver method 'method' must be of type string"
+                )
+        if tau != None:
+            if not isinstance(tau, (int,float)):
+                raise TypeError(
+                    "discrete timestep 'tau' must be of type int or float"
+                )
+            print(f"performing discrete timestepping with tau = {tau}\n")
 
         # Input checks on supplied simulation time
         time, actual_start_date = validate_simulation_time(time, warmup)
 
         # Input check on draw function
         if draw_function:
             validate_draw_function(draw_function, self.parameters, samples)
-           
+        
+        # Provinding 'N' but no draw function: wastefull
+        if ((N != 1) & (draw_function==None)):
+            raise ValueError('performing N={0} repeated simulations without a `draw_function` is mighty wastefull of computational resources'.format(N))
+
         # Copy parameter dictionary --> dict is global
         cp = copy.deepcopy(self.parameters)
         # Construct list of drawn dictionaries
         drawn_dictionaries=[]
         for n in range(N):
             cp_draws=copy.deepcopy(self.parameters)
             if draw_function:
@@ -791,22 +771,98 @@
             else:
                 drawn_dictionaries.append({})
             self.parameters=cp_draws
 
         # Run simulations
         if processes: # Needed 
             with mp.Pool(processes) as p:
-                output = p.map(partial(self._mp_sim_single, time=time, actual_start_date=actual_start_date, method=method, rtol=rtol, output_timestep=output_timestep), drawn_dictionaries)
+                output = p.map(partial(self._mp_sim_single, time=time, actual_start_date=actual_start_date, method=method, rtol=rtol, output_timestep=output_timestep, tau=tau), drawn_dictionaries)
         else:
             output=[]
             for dictionary in drawn_dictionaries:
-                output.append(self._mp_sim_single(dictionary, time, actual_start_date, method=method, rtol=rtol, output_timestep=output_timestep))
+                output.append(self._mp_sim_single(dictionary, time, actual_start_date, method=method, rtol=rtol, output_timestep=output_timestep, tau=tau))
 
         # Append results
         out = output[0]
         for xarr in output[1:]:
             out = xarray.concat([out, xarr], "draws")
 
         # Reset parameter dictionary
         self.parameters = cp
 
-        return out
+        return out
+
+
+def _output_to_xarray_dataset(output, state_shapes, state_dimensions, state_coordinates, actual_start_date=None):
+    """
+    Convert array (returned by scipy) to an xarray Dataset with the right coordinates and variable names
+
+    Parameters
+    ----------
+
+    output: dict
+        Keys: "y" (states) and "t" (timesteps)
+        Size of `y`: (total number of states, number of timesteps)
+        Size of `t`: number of timesteps
+
+    state_shapes: dict
+        Keys: state names. Values: tuples with state shape
+
+    state_dimensions: dict
+        Keys: state names. Values: list containing dimensions associated with state
+
+    state_coordinates: dict
+        Keys: state names. Values: list containing coordinates of every dimension the state is associated with
+
+    actual_start_date: datetime
+        Used to determine if the time output should be returned as dates
+
+    Returns
+    -------
+
+    output: xarray.Dataset
+        Simulation results
+    """
+
+    # Convert scipy's output to a dictionary of states with the correct sizes
+    new_state_shapes={}
+    for k,v in state_shapes.items():
+        v=list(v)
+        v.append(len(output["t"]))
+        new_state_shapes.update({k: tuple(v)})
+    output_flat = np.ravel(output["y"])
+    data_variables = list_to_dict(output_flat, new_state_shapes)
+    # Move time axis to first position (yes, obviously I have tried this  with np.reshape in `list_to_dict` but this didn't work for n-D states)
+    for k,v in data_variables.items():
+        data_variables.update({k: np.moveaxis(v, [-1,], [0,])})
+
+    # Append the time dimension
+    new_state_dimensions={}
+    for k,v in state_dimensions.items():
+        v_acc = v.copy()
+        if actual_start_date is not None:
+            v_acc = ['date',] + v_acc
+            new_state_dimensions.update({k: v_acc})
+        else:
+            v_acc = ['time',] + v_acc
+            new_state_dimensions.update({k: v_acc})
+
+    # Append the time coordinates
+    new_state_coordinates={}
+    for k,v in state_coordinates.items():
+        v_acc=v.copy()
+        if actual_start_date is not None:
+            v_acc = [actual_start_date + pd.to_timedelta(output["t"], unit='D'),] + v_acc
+            new_state_coordinates.update({k: v_acc})
+        else:
+            v_acc = [output["t"],] + v_acc
+            new_state_coordinates.update({k: v_acc})
+
+    # Build the xarray dataset
+    data = {}
+    for var, arr in data_variables.items():
+        if len(new_state_dimensions[var]) == 1:
+            arr = np.ravel(arr)
+        xarr = xarray.DataArray(arr, dims=new_state_dimensions[var], coords=new_state_coordinates[var])
+        data[var] = xarr
+
+    return xarray.Dataset(data)
```

### Comparing `pySODM-0.2.2/src/pySODM/models/utils.py` & `pySODM-0.2.3/src/pySODM/models/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,9 +36,8 @@
         n = np.prod(s)
         # Reshape changes type of floats to np.ndarray which is not desirable
         if ((n == 1) & (retain_floats==True)):
             restoredArray.append(y[offset])
         else:
             restoredArray.append(y[offset:(offset+n)].reshape(s))
         offset+=n
-
     return dict(zip(shape_dictionary.keys(), restoredArray))
```

### Comparing `pySODM-0.2.2/src/pySODM/models/validation.py` & `pySODM-0.2.3/src/pySODM/models/validation.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,14 +51,19 @@
                 "Input argument 'time' must be a single number (int or float), a list of format: time=[start, stop], a string representing of a timestamp, or a timestamp"
             )
 
     if time[1] < time[0]:
         raise ValueError(
             "Start of simulation is chronologically after end of simulation"
         )
+    elif time[0] == time[1]:
+        # TODO: Might be usefull to just return the initial condition in this case?
+        raise ValueError(
+            "Start of simulation is the same as the end of simulation"
+        )
     return time, actual_start_date
 
 def validate_draw_function(draw_function, parameters, samples):
     """Validates the draw functions input and output. For use in the sim() function. """
 
     sig = inspect.signature(draw_function)
     keywords = list(sig.parameters.keys())
@@ -234,14 +239,15 @@
 
     return extra_params
 
 def validate_initial_states(state_shapes, initial_states):
     """
     A function to check the types and sizes of the model's initial states provided by the user.
     Automatically assumes non-specified states are equal to zero.
+    All allowed input types converted to np.float64.
 
     Parameters
     ----------
 
     state_shapes: dict
         Contains the shape of every model state.
     
@@ -260,52 +266,53 @@
         if state_name in initial_states:
             # if present, verify the length
             initial_states[state_name] = check_initial_states_shape(
                                         initial_states[state_name], state_shape, state_name, "initial state",
                                         )
         else:
             # Fill with zeros
-            initial_states[state_name] = np.zeros(state_shape)
+            initial_states[state_name] = np.zeros(state_shape, dtype=np.float64)
 
     # validate the states (using `set` to ignore order)
     if set(initial_states.keys()) != set(state_shapes.keys()):
         raise ValueError(
             f"The specified initial states don't exactly match the predefined states. Redundant states: {set(initial_states.keys()).difference(set(state_shapes.keys()))}"
         )
 
     # sort the initial states to match the state_names
     initial_states = {state: initial_states[state] for state in state_shapes}
 
     return initial_states
 
 def check_initial_states_shape(values, desired_shape, name, object_name):
-    """A function checking if the provided initial states have the correct shape
+    """ A function checking if the provided initial states have the correct shape
+        Converts all values of initial states to type np.float64
     """
 
     # If the model doesn't have dimensions, initial states can be defined as: np.array([int/float]), [int/float], int or float
     # However these still need to converted to a np.array internally
     if list(desired_shape) == [1]:
         if not isinstance(values, (list,int,float,np.int32,np.int64,np.float32,np.float64,np.ndarray)):
             raise TypeError(
                 f"{object_name} {name} must be of type int, float, or list. found {type(values)}"
             )
         else:
             if isinstance(values,(int,float)):
                 values = np.asarray([values,])
-        values = np.asarray(values)
+        values = np.asarray(values, dtype=np.float64)
 
         if values.shape != desired_shape:
             raise ValueError(
                 "The desired shape of model state '{name}' is {desired_shape}, but provided {obj} '{name}' "
                 "has length {val}".format(
                     desired_shape=desired_shape, obj=object_name, name=name, val=values.shape
                 )
             )
     else:
-        values = np.asarray(values)
+        values = np.asarray(values, dtype=np.float64)
         if values.shape != desired_shape:
             raise ValueError(
                 "The desired shape of model state '{name}' is {desired_shape}, but provided {obj} '{name}' "
                 "has length {val}".format(
                     desired_shape=desired_shape, obj=object_name, name=name, val=values.shape
                 )
             )
```

### Comparing `pySODM-0.2.2/src/pySODM/optimization/mcmc.py` & `pySODM-0.2.3/src/pySODM/optimization/mcmc.py`

 * *Files 1% similar despite different names*

```diff
@@ -237,14 +237,15 @@
 
     try:
         autocorr = sampler.get_autocorr_time()
         thin = max(1, round(0.5 * np.max(autocorr)))
         print(f'Convergence: the chain is longer than 50 times the intergrated autocorrelation time.\nPreparing to save samples with thinning value {thin}.')
         sys.stdout.flush()
     except:
+        thin=1
         print('Warning: The chain is shorter than 50 times the integrated autocorrelation time.\nUse this estimate with caution and run a longer chain! Setting thinning to 1.\n')
         sys.stdout.flush()
 
     #####################################
     # Construct a dictionary of samples #
     #####################################
```

### Comparing `pySODM-0.2.2/src/pySODM/optimization/nelder_mead.py` & `pySODM-0.2.3/src/pySODM/optimization/nelder_mead.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     ##################
 
     if not bounds:
         try:
             bounds = func.expanded_bounds
         except:
             raise Exception(
-                "'func' does not appear to be a pySODM model: 'expanded_bounds' not found. Provide bounds directly to `pso.optimize()`"
+                "'func' does not appear to be a pySODM model: 'expanded_bounds' not found. Provide bounds directly to `nelder_mead.optimize()`"
             )
 
     # Input check bounds
     lb, ub = [], []
     for variable_bounds in bounds:
         lb.append(variable_bounds[0])
         ub.append(variable_bounds[1])
```

### Comparing `pySODM-0.2.2/src/pySODM/optimization/objective_functions.py` & `pySODM-0.2.3/src/pySODM/optimization/objective_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,19 @@
     ll: float
         Loglikelihood belonging to the comparison of the data points and the model prediction for its particular parameter values
     """
 
     if not sigma.shape == ymodel.shape:
         # Expand first dimensions on 'alpha' to match the axes
         sigma = np.array(sigma)[np.newaxis, ...]   
-
+    # Check for zeros (TODO: move to a higher layer)
+    if len(sigma[sigma<=0]) != 0:
+        raise ValueError(
+            'argument `sigma` of `ll_gaussian` contains values smaller than or equal to zero'
+        )
     return - 1/2 * np.sum((ydata - ymodel) ** 2 / sigma**2 + np.log(2*np.pi*sigma**2))
 
 def ll_poisson(ymodel, ydata):
     """Loglikelihood of Poisson distribution
     
     Parameters
     ----------
@@ -126,15 +130,15 @@
 
     Returns
     -------
     Log probability of sample x in light of a uniform prior distribution.
 
     """
     prob = 1/(bounds[1]-bounds[0])
-    condition = bounds[0] < x < bounds[1]
+    condition = bounds[0] <= x <= bounds[1]
     if condition == True:
         # Can also be set to zero: value doesn't matter much because its constant
         return np.log(prob)
     else:
         return -np.inf
 
 def log_prior_custom(x, args):
@@ -437,14 +441,17 @@
         return total_ll
 
     def __call__(self, thetas, simulation_kwargs={}):
         """
         This function manages the internal bookkeeping (assignment of model parameters, model simulation) and then computes and sums the log prior probabilities and log likelihoods to compute the log posterior probability.
         """
 
+        # Compute log prior probability 
+        lp = self.compute_log_prior_probability(thetas, self.log_prior_prob_fnc, self.log_prior_prob_fnc_args)
+
         # Restrict thetas to user-provided bounds
         for i,theta in enumerate(thetas):
             if theta > self.expanded_bounds[i][1]:
                 thetas[i] = self.expanded_bounds[i][1]
             elif theta < self.expanded_bounds[i][0]:
                 thetas[i] = self.expanded_bounds[i][0]
 
@@ -455,17 +462,14 @@
         if 'warmup' in thetas_dict.keys():
             simulation_kwargs.update({'warmup': float(thetas_dict['warmup'])})
             del thetas_dict['warmup']
 
         # Assign model parameters
         self.model.parameters.update(thetas_dict)
 
-        # Compute log prior probability 
-        lp = self.compute_log_prior_probability(thetas, self.log_prior_prob_fnc, self.log_prior_prob_fnc_args)
-
         if not self.initial_states:
             # Perform simulation only once
             out = self.model.sim([self.start_sim,self.end_sim], **simulation_kwargs)
             # Loop over dataframes
             for idx,df in enumerate(self.data):
                 # Get aggregation function
                 if self.aggregation_function:
@@ -884,30 +888,33 @@
         Model "output" 
     """
 
     # Append the time dimension
     new_state_dimensions={}
     for k,v in state_dimensions.items():
         v_acc = v.copy()
-        v_acc.append(time_index)
+        v_acc = [time_index,] + v_acc
         new_state_dimensions.update({k: v_acc})
 
     # Append the time coordinates
     new_state_coordinates={}
     for k,v in state_coordinates.items():
         v_acc=v.copy()
-        v_acc.append([0,])
+        if time_index == 'time':
+            v_acc = [[0,],] + v_acc
+        elif time_index == 'date':
+            v_acc = [[pd.Timestamp('2000-01-01'),],] + v_acc
         new_state_coordinates.update({k: v_acc})
 
     # Build the xarray dataset
     data = {}
     for var, arr in initial_states.items():
         if arr.ndim >= 1:
             if state_dimensions[var]:
-                arr = arr[..., np.newaxis]
+                arr = arr[np.newaxis, ...]
         xarr = xr.DataArray(arr, dims=new_state_dimensions[var], coords=new_state_coordinates[var])
         data[var] = xarr
 
     return xr.Dataset(data)
 
 
 def compare_data_model_coordinates(output, data, calibration_state_names, aggregation_function, additional_axes_data):
@@ -943,15 +950,14 @@
     # Validate
     coordinates_data_also_in_model=[]
     aggregate_over=[]
     # Loop over states/datasets we'd like to match
     for i, (state_name, df) in enumerate(zip(calibration_state_names, data)):
         # Call the aggregation function
         if aggregation_function:
-            
             new_output = aggregation_function[i](output[state_name])
         else:
             new_output = output[state_name]
         # Create a dictionary containing, for every dimensions that is not 'time'/'date'
         # key: list of dimensions, value: list of corresponding coordinates
         dimensions = list(new_output.dims)
         dimensions = [d for d in dimensions if ((d != 'time')&(d!='date'))]
@@ -1076,15 +1082,16 @@
                         if not log_likelihood_fnc_args[idx].index.equals(df.index):
                             raise ValueError(
                                 f"index of pd.Series containing arguments of the {idx}th log likelihood function must match the index of the {idx}th dataset"
                             )
                         else:
                             # Make sure time index is in first position
                             val = log_likelihood_fnc_args[idx].to_xarray()
-                            val = val.transpose([time_index,]+additional_axes_data[idx])
+                            dims = [time_index,]+additional_axes_data[idx]
+                            val = val.transpose(*dims)
                             log_likelihood_fnc_args[idx] = val.to_numpy()         
             else:
                 # Compute desired shape in case of one parameter per stratfication
                 desired_shape=[]
                 for lst in coordinates_data_also_in_model[idx]:
                     desired_shape.append(len(lst))
                 # Input checks
@@ -1104,11 +1111,12 @@
                         if not log_likelihood_fnc_args[idx].index.equals(df.index):
                             raise ValueError(
                                 f"index of pd.Series containing arguments of the {idx}th log likelihood function must match the index of the {idx}th dataset"
                             )
                         else:
                             # Make sure time index is in first position
                             val = log_likelihood_fnc_args[idx].to_xarray()
-                            val = val.transpose([time_index,]+additional_axes_data[idx])
+                            dims = [time_index,]+additional_axes_data[idx]
+                            val = val.transpose(*dims)
                             log_likelihood_fnc_args[idx] = val.to_numpy()
     
     return log_likelihood_fnc_args
```

### Comparing `pySODM-0.2.2/src/pySODM/optimization/pso.py` & `pySODM-0.2.3/src/pySODM/optimization/pso.py`

 * *Files identical despite different names*

### Comparing `pySODM-0.2.2/src/pySODM/optimization/utils.py` & `pySODM-0.2.3/src/pySODM/optimization/utils.py`

 * *Files identical despite different names*

### Comparing `pySODM-0.2.2/src/pySODM/optimization/visualization.py` & `pySODM-0.2.3/src/pySODM/optimization/visualization.py`

 * *Files identical despite different names*

### Comparing `pySODM-0.2.2/src/pySODM.egg-info/PKG-INFO` & `pySODM-0.2.3/src/pySODM.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,83 +1,88 @@
 Metadata-Version: 2.1
 Name: pySODM
-Version: 0.2.2
+Version: 0.2.3
 Summary: Simulating and Optimising Dynamical Models
 Home-page: https://github.com/twallema/pySODM
 Author: Tijs Alleman, KERMIT, Ghent University
 Author-email: tijs.alleman@ugent.be
 License: MIT
 Keywords: ODE PDE simulation calibration gillespie xarray emcee
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: develop
 License-File: LICENSE.txt
 
 ## pySODM
 *Simulating and Optimising Dynamical Models in Python 3*
 
-![build](https://github.com/twallema/pySODM/actions/workflows/tests.yml/badge.svg) ![docs](https://github.com/twallema/pySODM/actions/workflows/deploy.yml/badge.svg)
+![build](https://github.com/twallema/pySODM/actions/workflows/tests.yml/badge.svg) ![docs](https://github.com/twallema/pySODM/actions/workflows/deploy.yml/badge.svg) [![HitCount](https://hits.dwyl.com/twallema/pySODM.svg)](https://hits.dwyl.com/twallema/pySODM)
 
-### Links
+### Quick installation 
+```
+pip install pySODM
+```
+### Resources
 
 Documentation: https://twallema.github.io/pySODM
 
 Manuscript: https://arxiv.org/abs/2301.10664
 
+pyPI: https://pypi.org/project/pySODM/ 
+
 ### Aim & Scope
 
 A modeling and simulation workflow will typically constitute the following steps (see [Villaverde et. al](https://doi.org/10.1093/bib/bbab387)),
 1. Build a system dynamical model to describe some real-world phenomenon. Assess structural identifiability.
 2. Calibrate the model to a set of experimental data.
 3. Extract knowledge from the calibrated parameter values (assess practical identifiability).
 4. Use the model to make projections outside the calibrated range.
 
-The aim of pySODM is to reduce the time it takes to step through this workflow. pySODM is a template to construct, simulate and calibrate dynamical systems governed by differential equations. Models can have n-dimensional labeled states of different sizes and can be simulated deterministically and stochastically. Model parameters can be time-dependent by means of complex functions
+The aim of pySODM is to reduce the time it takes to step through this workflow. pySODM provides a *template* to construct, simulate and calibrate dynamical systems governed by differential equations. Models can have n-dimensional labeled states of different sizes and can be simulated deterministically and stochastically. Model parameters can be time-dependent by means of complex functions
 with arbitrary inputs. The labeled n-dimensional model states can be aligned with n-dimensional
 data to compute the posterior probability function, which can subsequently be optimised.
 
 ### Overview of features
 
 | Workflow                     | Features                                                                                                                        |
 |------------------------------|---------------------------------------------------------------------------------------------------------------------------------|
-| Building a model     | Solve coupled systems of equations deterministically (integration) or stochastically (Gillespie's SSA and Tau-Leaping)                  |
-|                              | n-Dimensional model states with coordinates. Different states can have different sizes.                                         |
-|                              | Easy indexing, manipulating, saving, and piping to third-party software of model output by formatting simulation output as `xarray.Dataset` |
-| Simulating a model   | Vary model parameters during the simulation in accordance with an arbitrarily complex function containing any input                     |
-|                              | Use *draw functions* to perform repeated simulations for sensitivity analysis. With multiprocessing support                     |
-| Calibrating a model  | Calibration of n-dimensional model parameters                                                                                           |
-|                              | Construct a posterior probability function                                                                                      |
-|                              | Automatic alignment of data and model prediction over timesteps and dimensions                                                  |
-|                              | Nelder-Mead Simplex and Particle Swarm Optimization for frequentist optimization                                                |
-|                              | Pipeline to and backend for `emcee.EnsembleSampler` to perform Bayesian inference of model parameters                           |
-|                              | Analysis of the mean-variance ratio in count-based datasets to aid in the choice of an appropriate likelihood function          |
+| Construct a dynamical model     | Implement coupled systems of differential equations            |
+|                                 | States can be n-dimensional and of different sizes, allowing users to build models with subprocesses                                       |
+|                                 | Allows n-dimensional model states to be labelled with coordinates and dimensions by using `xarray.Dataset}` to store simulation output |
+|                                 | Easy indexing, manipulating, saving, and piping to third-party software of model output by formatting simulation output as `xarray.Dataset` |
+| Simulating the model            | Continuous and discrete deterministic simulation or discrete stochastic simulation (Gillespie's Stochastic Simulation Algorithm or Tau-Leaping) |
+|                                 | Vary model parameters during the simulation generically using a complex function |
+|                                 | Use *draw functions* to perform repeated simulations for sensitivity analysis. With multiprocessing support |
+| Calibrate the model             | Construct and maximize a posterior probability function  |
+|                                 | Automatic alignment of data and model forecast over timesteps and coordinates  |
+|                                 | Nelder-Mead Simplex and Particle Swarm Optimization for point estimation of model parameters |
+|                                 | Pipeline to and backend for `emcee.EnsembleSampler` to perform Bayesian inference of model parameters                           |
 
 ### Getting started
 
 The [quistart tutorial](quickstart.md) will teach you the basics of building and simulating models with n-dimensional labeled states in pySODM. It will demonstrate how to vary model parameters over the course of a simulation and how to perform repeated simulations with sampling of model parameters.
 
 The [workflow](worfklow.md) tutorial provides a step-by-step introduction to a modeling and simulation workflow by inferring the distributions of the model parameters of a simple compartmental disease model using a synthetic dataset. 
 
 The [enzyme kinetics](enzyme_kinetics.md) and [influenza 17-18](influenza_1718.md) case studies apply the modeling and simulation workflow to more advanced, real-world problems. In the enzyme kinetics case study, a 1D packed-bed reactor model is implemented in pySODM by reducing the two PDEs to a set of coupled ODEs by using the method-of-lines. In the Influenza 17-18 case study, a stochastic, age-structured model for influenza is developped and calibrated to the Influenza incidence data reported by the Belgian Federal Institute of Public Health. These case studies mainly serve to demonstrate pySODM's capabilities across scientific disciplines and highlight the arbitrarily complex nature of the models that can be built with pySODM. For an academic description of pySODM and on the Enzyme Kinetics and Influenza 17-18 case studies, checkout our [manuscript](https://arxiv.org/abs/2301.10664).
 
 ### Versions
 
 - Version 0.2.0 (2023-01-19, PR #25)
     > Introduction of `state_dimensions` in model declaration, allowing the user to define models where states can have different sizes.
     - Version 0.2.1 (2023-01-27, PR #30)
-        > Fixed bugs when using pySODM for the COVID-19 related models. More thorough checks on `bounds` in the log posterior probability function. Finished manuscript.
+        > Fixed bugs encountered when incorporating pySODM into the SARS-CoV-2 Dynamic Transmission Models. More thorough checks on `bounds` in the log posterior probability function. Finished manuscript.
+    - Version 0.2.2 (2023-01-27, PR #31)
+        > Published to pyPI.
+    - Version 0.2.3 (2023-05-04, PR #46)
+        > Fixed minor bugs encountered when using pySODM for a dynamic input-output model of the Belgian economy. Published to pyPI.
 - Version 0.1 (2022-12-23, PR #14)
     > Application pySODM to three use cases. Documentation website. Unit tests for ODEModel, SDEModel and calibration. 
     - Version 0.1.1 (2023-01-09, PR #20)
         > Start of semantic versions: Major.Minor.Patch
     - Version 0.1.2 (2023-01-11, PR #23)
         > Calibration of 1-D model parameters generalized to n-dimensions.
         > Added 'aggregation functions' to the `log_posterior_probability` class to perform custom aggregations of model output before matching with data.
         > `xarray.DataArray`/`xarray.Dataset` can be used as datasets during calibration. Internally converted to `pd.DataFrame`.
 - Version 0.0 (2022-11-14)
     - First pySODM version. Obtained by splitting the generally applicable parts from the ad-hoc parts in UGentBiomath/COVID19-Model. Without documentation website. 
 - Pre-development (2020-05-01 - 2022-11-24)
     - Code developped to model the spread of SARS-CoV-2 in Belgium (UGentBiomath/COVID19-Model).
-
-[![HitCount](https://hits.dwyl.com/twallema/pySODM.svg)](https://hits.dwyl.com/twallema/pySODM)
-
-
```

### Comparing `pySODM-0.2.2/src/pySODM.egg-info/SOURCES.txt` & `pySODM-0.2.3/src/pySODM.egg-info/SOURCES.txt`

 * *Files identical despite different names*

