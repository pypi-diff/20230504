# Comparing `tmp/xopt-1.3.1.tar.gz` & `tmp/xopt-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/Xopt/Xopt/dist/.tmp-roqjaqyi/xopt-1.3.1.tar", last modified: Wed Apr 19 17:57:55 2023, max compression
+gzip compressed data, was "/home/runner/work/Xopt/Xopt/dist/.tmp-p569cmsx/xopt-1.4.0.tar", last modified: Wed May  3 22:33:53 2023, max compression
```

## Comparing `xopt-1.3.1.tar` & `xopt-1.4.0.tar`

### file list

```diff
@@ -1,115 +1,117 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:57:55.000000 xopt-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-19 17:57:46.000000 xopt-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-19 17:57:46.000000 xopt-1.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-04-19 17:57:55.000000 xopt-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-04-19 17:57:46.000000 xopt-1.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-19 17:57:46.000000 xopt-1.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-19 17:57:55.000000 xopt-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-19 17:57:46.000000 xopt-1.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:57:55.000000 xopt-1.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:57:46.000000 xopt-1.3.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:57:55.000000 xopt-1.3.1/tests/generators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:57:46.000000 xopt-1.3.1/tests/generators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:57:55.000000 xopt-1.3.1/tests/generators/bayesian/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:57:46.000000 xopt-1.3.1/tests/generators/bayesian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-04-19 17:57:46.000000 xopt-1.3.1/tests/generators/bayesian/test_bayesian_exploration.py
--rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-04-19 17:57:46.000000 xopt-1.3.1/tests/generators/bayesian/test_bayesian_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-04-19 17:57:46.000000 xopt-1.3.1/tests/generators/bayesian/test_bayesian_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-04-19 17:57:46.000000 xopt-1.3.1/tests/generators/bayesian/test_custom_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-04-19 17:57:46.000000 xopt-1.3.1/tests/generators/bayesian/test_expected_improvement.py
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-04-19 17:57:46.000000 xopt-1.3.1/tests/generators/bayesian/test_high_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-04-19 17:57:46.000000 xopt-1.3.1/tests/generators/bayesian/test_mggpo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-04-19 17:57:46.000000 xopt-1.3.1/tests/generators/bayesian/test_mobo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-04-19 17:57:46.000000 xopt-1.3.1/tests/generators/bayesian/test_multi_fidelity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-04-19 17:57:46.000000 xopt-1.3.1/tests/generators/bayesian/test_time_dependent_bo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-04-19 17:57:46.000000 xopt-1.3.1/tests/generators/bayesian/test_turbo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-04-19 17:57:46.000000 xopt-1.3.1/tests/generators/bayesian/test_upper_confidence_bound.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-19 17:57:46.000000 xopt-1.3.1/tests/generators/bayesian/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-04-19 17:57:46.000000 xopt-1.3.1/tests/generators/test_extremum_seeking.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-19 17:57:46.000000 xopt-1.3.1/tests/generators/test_generator_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-19 17:57:46.000000 xopt-1.3.1/tests/generators/test_random.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-19 17:57:46.000000 xopt-1.3.1/tests/generators/test_rcds.py
--rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-04-19 17:57:46.000000 xopt-1.3.1/tests/test_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-19 17:57:46.000000 xopt-1.3.1/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     9240 2023-04-19 17:57:46.000000 xopt-1.3.1/tests/test_pydantic.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-19 17:57:46.000000 xopt-1.3.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-04-19 17:57:46.000000 xopt-1.3.1/tests/test_vocs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-04-19 17:57:46.000000 xopt-1.3.1/tests/test_xopt.py
--rw-r--r--   0 runner    (1001) docker     (123)    78325 2023-04-19 17:57:46.000000 xopt-1.3.1/versioneer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:57:55.000000 xopt-1.3.1/xopt/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-19 17:57:55.000000 xopt-1.3.1/xopt/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    15472 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:57:55.000000 xopt-1.3.1/xopt/generators/
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:57:55.000000 xopt-1.3.1/xopt/generators/bayesian/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/bayesian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/bayesian/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/bayesian/bayesian_exploration.py
--rw-r--r--   0 runner    (1001) docker     (123)    11464 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/bayesian/bayesian_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:57:55.000000 xopt-1.3.1/xopt/generators/bayesian/custom_botorch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/bayesian/custom_botorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/bayesian/custom_botorch/constrained_acqusition.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/bayesian/custom_botorch/identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/bayesian/custom_botorch/multi_fidelity.py
--rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/bayesian/custom_botorch/proximal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/bayesian/expected_improvement.py
--rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/bayesian/mggpo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/bayesian/mobo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:57:55.000000 xopt-1.3.1/xopt/generators/bayesian/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/bayesian/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/bayesian/models/prior_mean.py
--rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/bayesian/models/standard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/bayesian/models/time_dependent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/bayesian/models/transformed_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/bayesian/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/bayesian/multi_fidelity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/bayesian/objectives.py
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/bayesian/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/bayesian/time_dependent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/bayesian/turbo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/bayesian/upper_confidence_bound.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/bayesian/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:57:55.000000 xopt-1.3.1/xopt/generators/es/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/es/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/es/extremumseeking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:57:55.000000 xopt-1.3.1/xopt/generators/ga/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/ga/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11706 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/ga/cnsga.py
--rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/ga/deap_creator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3137 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/ga/deap_fitness_with_constraints.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3138 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/ga/fitness_with_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:57:55.000000 xopt-1.3.1/xopt/generators/rcds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/rcds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14509 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/rcds/rcds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:57:55.000000 xopt-1.3.1/xopt/generators/scipy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/scipy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12355 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/generators/scipy/neldermead.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:57:55.000000 xopt-1.3.1/xopt/mpi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/mpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/mpi/run.py
--rw-r--r--   0 runner    (1001) docker     (123)    18604 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/pydantic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:57:55.000000 xopt-1.3.1/xopt/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:57:55.000000 xopt-1.3.1/xopt/resources/test_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/resources/test_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/resources/test_functions/ackley_20.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/resources/test_functions/modified_tnk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/resources/test_functions/rosenbrock.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/resources/test_functions/sinusoid_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/resources/test_functions/sphere_20.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/resources/test_functions/tnk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/resources/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13546 2023-04-19 17:57:46.000000 xopt-1.3.1/xopt/vocs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:57:55.000000 xopt-1.3.1/xopt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-04-19 17:57:55.000000 xopt-1.3.1/xopt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-04-19 17:57:55.000000 xopt-1.3.1/xopt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 17:57:55.000000 xopt-1.3.1/xopt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-19 17:57:55.000000 xopt-1.3.1/xopt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-19 17:57:55.000000 xopt-1.3.1/xopt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:53.000000 xopt-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-03 22:33:42.000000 xopt-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-03 22:33:42.000000 xopt-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-05-03 22:33:53.000000 xopt-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-05-03 22:33:42.000000 xopt-1.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-03 22:33:42.000000 xopt-1.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-03 22:33:53.000000 xopt-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-03 22:33:42.000000 xopt-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:53.000000 xopt-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:42.000000 xopt-1.4.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:53.000000 xopt-1.4.0/tests/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:42.000000 xopt-1.4.0/tests/generators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:53.000000 xopt-1.4.0/tests/generators/bayesian/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:42.000000 xopt-1.4.0/tests/generators/bayesian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-05-03 22:33:42.000000 xopt-1.4.0/tests/generators/bayesian/test_bayesian_exploration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-05-03 22:33:42.000000 xopt-1.4.0/tests/generators/bayesian/test_bayesian_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-05-03 22:33:42.000000 xopt-1.4.0/tests/generators/bayesian/test_bayesian_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-03 22:33:42.000000 xopt-1.4.0/tests/generators/bayesian/test_custom_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-05-03 22:33:42.000000 xopt-1.4.0/tests/generators/bayesian/test_expected_improvement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-05-03 22:33:42.000000 xopt-1.4.0/tests/generators/bayesian/test_high_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-03 22:33:42.000000 xopt-1.4.0/tests/generators/bayesian/test_mggpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-05-03 22:33:42.000000 xopt-1.4.0/tests/generators/bayesian/test_mobo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-03 22:33:42.000000 xopt-1.4.0/tests/generators/bayesian/test_model_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-05-03 22:33:42.000000 xopt-1.4.0/tests/generators/bayesian/test_multi_fidelity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-05-03 22:33:42.000000 xopt-1.4.0/tests/generators/bayesian/test_time_dependent_bo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-03 22:33:42.000000 xopt-1.4.0/tests/generators/bayesian/test_turbo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-05-03 22:33:42.000000 xopt-1.4.0/tests/generators/bayesian/test_upper_confidence_bound.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-03 22:33:42.000000 xopt-1.4.0/tests/generators/bayesian/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-05-03 22:33:42.000000 xopt-1.4.0/tests/generators/test_extremum_seeking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-03 22:33:42.000000 xopt-1.4.0/tests/generators/test_generator_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-03 22:33:42.000000 xopt-1.4.0/tests/generators/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-03 22:33:42.000000 xopt-1.4.0/tests/generators/test_rcds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-05-03 22:33:42.000000 xopt-1.4.0/tests/test_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-03 22:33:42.000000 xopt-1.4.0/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9240 2023-05-03 22:33:42.000000 xopt-1.4.0/tests/test_pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-03 22:33:42.000000 xopt-1.4.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-05-03 22:33:42.000000 xopt-1.4.0/tests/test_vocs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-05-03 22:33:42.000000 xopt-1.4.0/tests/test_xopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78325 2023-05-03 22:33:42.000000 xopt-1.4.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:53.000000 xopt-1.4.0/xopt/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-03 22:33:53.000000 xopt-1.4.0/xopt/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15621 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:53.000000 xopt-1.4.0/xopt/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:53.000000 xopt-1.4.0/xopt/generators/bayesian/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/bayesian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/bayesian/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/bayesian/bayesian_exploration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11464 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/bayesian/bayesian_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:53.000000 xopt-1.4.0/xopt/generators/bayesian/custom_botorch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/bayesian/custom_botorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/bayesian/custom_botorch/constrained_acqusition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/bayesian/custom_botorch/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/bayesian/custom_botorch/multi_fidelity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/bayesian/custom_botorch/proximal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/bayesian/expected_improvement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/bayesian/mggpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/bayesian/mobo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:53.000000 xopt-1.4.0/xopt/generators/bayesian/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/bayesian/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/bayesian/models/prior_mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/bayesian/models/standard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/bayesian/models/time_dependent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/bayesian/models/trainable_mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/bayesian/models/transformed_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/bayesian/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/bayesian/multi_fidelity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/bayesian/objectives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/bayesian/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/bayesian/time_dependent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/bayesian/turbo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/bayesian/upper_confidence_bound.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/bayesian/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:53.000000 xopt-1.4.0/xopt/generators/es/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/es/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/es/extremumseeking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:53.000000 xopt-1.4.0/xopt/generators/ga/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/ga/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11706 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/ga/cnsga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/ga/deap_creator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3137 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/ga/deap_fitness_with_constraints.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3138 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/ga/fitness_with_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:53.000000 xopt-1.4.0/xopt/generators/rcds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/rcds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14509 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/rcds/rcds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:53.000000 xopt-1.4.0/xopt/generators/scipy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/scipy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12355 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/generators/scipy/neldermead.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:53.000000 xopt-1.4.0/xopt/mpi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/mpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/mpi/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18604 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/pydantic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:53.000000 xopt-1.4.0/xopt/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:53.000000 xopt-1.4.0/xopt/resources/test_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/resources/test_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/resources/test_functions/ackley_20.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/resources/test_functions/modified_tnk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/resources/test_functions/rosenbrock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/resources/test_functions/sinusoid_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/resources/test_functions/sphere_20.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/resources/test_functions/tnk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/resources/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13823 2023-05-03 22:33:42.000000 xopt-1.4.0/xopt/vocs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:33:53.000000 xopt-1.4.0/xopt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-05-03 22:33:53.000000 xopt-1.4.0/xopt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-05-03 22:33:53.000000 xopt-1.4.0/xopt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 22:33:53.000000 xopt-1.4.0/xopt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-03 22:33:53.000000 xopt-1.4.0/xopt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-03 22:33:53.000000 xopt-1.4.0/xopt.egg-info/top_level.txt
```

### Comparing `xopt-1.3.1/LICENSE` & `xopt-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xopt-1.3.1/PKG-INFO` & `xopt-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xopt
-Version: 1.3.1
+Version: 1.4.0
 Home-page: https://github.com/ChristopherMayes/xopt
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
   <img src="docs/assets/Xopt-logo.png", width="200">
```

### Comparing `xopt-1.3.1/README.md` & `xopt-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `xopt-1.3.1/setup.py` & `xopt-1.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.1/tests/generators/bayesian/test_bayesian_exploration.py` & `xopt-1.4.0/tests/generators/bayesian/test_bayesian_exploration.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.1/tests/generators/bayesian/test_bayesian_generator.py` & `xopt-1.4.0/tests/generators/bayesian/test_bayesian_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,16 +28,17 @@
         model = gen.train_model(test_data)
         assert isinstance(model, GPyTorchModel)
 
         # test evaluating the model
         test_pts = torch.tensor(
             pd.DataFrame(TEST_VOCS_BASE.random_inputs(5, False, False)).to_numpy()
         )
+
         with torch.no_grad():
-            model(test_pts)
+            model.posterior(test_pts)
 
         # test with maximize and minimize
         test_vocs = deepcopy(TEST_VOCS_BASE)
         test_vocs.objectives["y1"] = "MINIMIZE"
         test_data = deepcopy(TEST_VOCS_DATA)
         gen = BayesianGenerator(test_vocs)
         model = gen.train_model(test_data)
```

### Comparing `xopt-1.3.1/tests/generators/bayesian/test_bayesian_options.py` & `xopt-1.4.0/tests/generators/bayesian/test_bayesian_options.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.1/tests/generators/bayesian/test_custom_model.py` & `xopt-1.4.0/tests/generators/bayesian/test_custom_model.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.1/tests/generators/bayesian/test_expected_improvement.py` & `xopt-1.4.0/tests/generators/bayesian/test_expected_improvement.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,18 @@
+import torch
+import pandas as pd
 from copy import deepcopy
-
 import pytest
+from botorch.acquisition import ExpectedImprovement
 
 from xopt.base import Xopt
-
+from xopt.vocs import VOCS, ObjectiveEnum
 from xopt.evaluator import Evaluator
 from xopt.generators.bayesian.expected_improvement import ExpectedImprovementGenerator
 from xopt.generators.bayesian.upper_confidence_bound import UCBOptions
-
 from xopt.resources.testing import TEST_VOCS_BASE, TEST_VOCS_DATA, xtest_callable
 
 
 class TestExpectedImprovement:
     def test_init(self):
         ei_gen = ExpectedImprovementGenerator(TEST_VOCS_BASE)
         ei_gen.options.dict()
@@ -78,7 +79,42 @@
 
         # initialize with single initial candidate
         xopt.step()
 
         # now use bayes opt
         for _ in range(1):
             xopt.step()
+
+    def test_acquisition_accuracy(self):
+        train_x = torch.tensor([0.01, 0.3, 0.6, 0.99]).double()
+        train_y = torch.sin(2 * torch.pi * train_x)
+        train_data = pd.DataFrame(
+            {"x1": train_x.numpy(), "y1": train_y.numpy()})
+        test_x = torch.linspace(0.0, 1.0, 1000)
+
+        for objective in ObjectiveEnum:
+            vocs = VOCS(**{"variables": {"x1": [0.0, 1.0]},
+                           "objectives": {"y1": objective}})
+            generator = ExpectedImprovementGenerator(vocs)
+            generator.add_data(train_data)
+            model = generator.train_model().models[0]
+
+            # xopt acquisition function
+            acq = generator.get_acquisition(model)
+
+            # analytical acquisition function
+            if objective == "MAXIMIZE":
+                an_acq = ExpectedImprovement(model, best_f=train_y.max(),
+                                             maximize=True)
+            else:
+                an_acq = ExpectedImprovement(model, best_f=train_y.min(),
+                                             maximize=False)
+
+            # compare candidates (maximum in test data)
+            with torch.no_grad():
+                acq_v = acq(test_x.reshape(-1, 1, 1))
+                candidate = test_x[torch.argmax(acq_v)]
+                an_acq_v = an_acq(test_x.reshape(-1, 1, 1))
+                an_candidate = test_x[torch.argmax(an_acq_v)]
+
+            # difference should be small
+            assert torch.abs(an_candidate - candidate) < 0.01
```

### Comparing `xopt-1.3.1/tests/generators/bayesian/test_high_level.py` & `xopt-1.4.0/tests/generators/bayesian/test_high_level.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.1/tests/generators/bayesian/test_mggpo.py` & `xopt-1.4.0/tests/generators/bayesian/test_mggpo.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.1/tests/generators/bayesian/test_mobo.py` & `xopt-1.4.0/tests/generators/bayesian/test_mobo.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.1/tests/generators/bayesian/test_multi_fidelity.py` & `xopt-1.4.0/tests/generators/bayesian/test_multi_fidelity.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.1/tests/generators/bayesian/test_time_dependent_bo.py` & `xopt-1.4.0/tests/generators/bayesian/test_time_dependent_bo.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.1/tests/generators/bayesian/test_turbo.py` & `xopt-1.4.0/tests/generators/bayesian/test_turbo.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.1/tests/generators/bayesian/test_upper_confidence_bound.py` & `xopt-1.4.0/tests/generators/bayesian/test_upper_confidence_bound.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.1/tests/generators/bayesian/test_utils.py` & `xopt-1.4.0/tests/generators/bayesian/test_utils.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.1/tests/generators/test_extremum_seeking.py` & `xopt-1.4.0/tests/generators/test_extremum_seeking.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.1/tests/generators/test_rcds.py` & `xopt-1.4.0/tests/generators/test_rcds.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.1/tests/test_evaluator.py` & `xopt-1.4.0/tests/test_evaluator.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.1/tests/test_io.py` & `xopt-1.4.0/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.1/tests/test_pydantic.py` & `xopt-1.4.0/tests/test_pydantic.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.1/tests/test_vocs.py` & `xopt-1.4.0/tests/test_vocs.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.1/tests/test_xopt.py` & `xopt-1.4.0/tests/test_xopt.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.1/versioneer.py` & `xopt-1.4.0/versioneer.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.1/xopt/base.py` & `xopt-1.4.0/xopt/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -331,15 +331,18 @@
         """
         Concatenate new data to internal dataframe,
         and also adds this data to the generator if it exists.
         """
         logger.debug(f"Adding {len(new_data)} new data to internal dataframes")
 
         # Set internal dataframe. Don't use self.data =
-        new_data = pd.DataFrame(new_data)
+        new_data = pd.DataFrame(new_data, copy=True)  # copy for reindexing
+        new_data.index = np.arange(
+            len(self._data) + 1, len(self._data) + len(new_data) + 1
+        )
         self._data = pd.concat([self._data, new_data], axis=0)
         self._new_data = new_data
 
         if self.generator is not None:
             self.generator.add_data(new_data)
 
     @property
```

### Comparing `xopt-1.3.1/xopt/evaluator.py` & `xopt-1.4.0/xopt/evaluator.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.1/xopt/generator.py` & `xopt-1.4.0/xopt/generator.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.1/xopt/generators/__init__.py` & `xopt-1.4.0/xopt/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.1/xopt/generators/bayesian/__init__.py` & `xopt-1.4.0/xopt/generators/bayesian/__init__.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.1/xopt/generators/bayesian/base_model.py` & `xopt-1.4.0/xopt/generators/bayesian/base_model.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.1/xopt/generators/bayesian/bayesian_exploration.py` & `xopt-1.4.0/xopt/generators/bayesian/bayesian_exploration.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.1/xopt/generators/bayesian/bayesian_generator.py` & `xopt-1.4.0/xopt/generators/bayesian/bayesian_generator.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.1/xopt/generators/bayesian/custom_botorch/constrained_acqusition.py` & `xopt-1.4.0/xopt/generators/bayesian/custom_botorch/constrained_acqusition.py`

 * *Files 8% similar despite different names*

```diff
@@ -68,16 +68,21 @@
             X_pending=X_pending,
         )
         self.base_acqusition = base_acqusition
 
     @concatenate_pending_points
     @t_batch_mode_transform()
     def forward(self, X: Tensor) -> Tensor:
-        posterior = self.model.posterior(
-            X=X, posterior_transform=self.posterior_transform
-        )
-        samples = self.get_posterior_samples(posterior)
-        obj = self.objective(samples, X=X)
+        if self.objective.constraints:
+            posterior = self.model.posterior(
+                X=X, posterior_transform=self.posterior_transform
+            )
+            samples = self.get_posterior_samples(posterior)
+            obj = self.objective(samples, X=X)
 
-        # multiply the output of the base acquisition function by the feasibility
-        base_val = torch.nn.functional.softplus(self.base_acqusition(X), beta=10)
-        return base_val * obj.max(dim=-1)[0].mean(dim=0)
+            # multiply the output of the base acquisition function by
+            # the feasibility
+            base_val = torch.nn.functional.softplus(
+                self.base_acqusition(X), beta=10)
+            return base_val * obj.max(dim=-1)[0].mean(dim=0)
+        else:
+            return self.base_acqusition(X)
```

### Comparing `xopt-1.3.1/xopt/generators/bayesian/custom_botorch/identity.py` & `xopt-1.4.0/xopt/generators/bayesian/custom_botorch/identity.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.1/xopt/generators/bayesian/custom_botorch/multi_fidelity.py` & `xopt-1.4.0/xopt/generators/bayesian/custom_botorch/multi_fidelity.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.1/xopt/generators/bayesian/custom_botorch/proximal.py` & `xopt-1.4.0/xopt/generators/bayesian/custom_botorch/proximal.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.1/xopt/generators/bayesian/expected_improvement.py` & `xopt-1.4.0/xopt/generators/bayesian/expected_improvement.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import pandas as pd
 import torch
 from botorch.acquisition import qExpectedImprovement
 
 from xopt.generators.bayesian.bayesian_generator import BayesianGenerator
 from xopt.generators.bayesian.custom_botorch.constrained_acqusition import (
     ConstrainedMCAcquisitionFunction,
 )
@@ -10,15 +9,15 @@
 from xopt.utils import format_option_descriptions
 from xopt.vocs import VOCS
 
 
 class ExpectedImprovementGenerator(BayesianGenerator):
     alias = "expected_improvement"
     __doc__ = (
-        """Implements Bayeisan Optimization using the Upper Confidence Bound
+        """Implements Bayeisan Optimization using the Expected Improvement
         acquisition function"""
         + f"{format_option_descriptions(BayesianOptions())}"
     )
 
     def __init__(self, vocs: VOCS, options: BayesianOptions = None):
         """
         Generator using Expected improvement acquisition function
@@ -41,28 +40,24 @@
         super().__init__(vocs, options)
 
     @staticmethod
     def default_options() -> BayesianOptions:
         return BayesianOptions()
 
     def _get_acquisition(self, model):
-        valid_data = self.data[
-            pd.unique(self.vocs.variable_names + self.vocs.output_names)
-        ].dropna()
-        objective_data = self.vocs.objective_data(valid_data, "")
-
-        best_f = torch.tensor(objective_data.max(), **self._tkwargs)
+        objective_data = self.vocs.objective_data(self.data, "").dropna()
+        best_f = -torch.tensor(objective_data.min(), **self._tkwargs)
 
         qEI = qExpectedImprovement(
             model,
             best_f=best_f,
             sampler=self.sampler,
             objective=self._get_objective(),
         )
 
-        cqUCB = ConstrainedMCAcquisitionFunction(
+        cqEI = ConstrainedMCAcquisitionFunction(
             model,
             qEI,
             self._get_constraint_callables(),
         )
 
-        return cqUCB
+        return cqEI
```

### Comparing `xopt-1.3.1/xopt/generators/bayesian/mggpo.py` & `xopt-1.4.0/xopt/generators/bayesian/mggpo.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.1/xopt/generators/bayesian/mobo.py` & `xopt-1.4.0/xopt/generators/bayesian/mobo.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.1/xopt/generators/bayesian/models/prior_mean.py` & `xopt-1.4.0/xopt/generators/bayesian/models/prior_mean.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,22 +8,26 @@
 
 class CustomMean(TransformedModel, Mean):
     def __init__(
         self,
         model: torch.nn.Module,
         gp_input_transform: InputTransform,
         gp_outcome_transform: OutcomeTransform,
+        fixed_model: bool = False
     ):
         """Custom prior mean for a GP based on an arbitrary model.
+
         Args:
             model: Representation of the model.
             gp_input_transform: Module used to transform inputs in the GP.
             gp_outcome_transform: Module used to transform outcomes in the GP.
+            fixed_model: Inherited from TransformedModel.
         """
-        super().__init__(model, gp_input_transform, gp_outcome_transform)
+        super().__init__(model, gp_input_transform, gp_outcome_transform,
+                         fixed_model=fixed_model)
 
     def forward(self, x):
         # set transformers to eval mode
         self.set_transformers(eval_mode=True)
 
         # transform inputs to model space
         x_model = self.input_transformer.untransform(x)
```

### Comparing `xopt-1.3.1/xopt/generators/bayesian/models/standard.py` & `xopt-1.4.0/xopt/generators/bayesian/models/standard.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import pandas as pd
 import torch
+from typing import Optional
 from botorch.models import ModelListGP
 from botorch.models.transforms import Normalize, Standardize
 from gpytorch import Module
 from gpytorch.likelihoods import GaussianLikelihood
 from gpytorch.priors import GammaPrior
 
 from xopt.generators.bayesian.base_model import ModelConstructor
@@ -23,31 +24,24 @@
         self.likelihood = None
         if self.options.use_low_noise_prior:
             self.likelihood = GaussianLikelihood(noise_prior=GammaPrior(1.0, 10.0))
 
         self.input_data = None
         self.objective_data = None
         self.constraint_data = None
-        self.train_X = None
         self.tkwargs = {"dtype": torch.double, "device": "cpu"}
 
     def collect_data(self, data: pd.DataFrame):
-        # drop nans
-        valid_data = data[
-            pd.unique(self.vocs.variable_names + self.vocs.output_names)
-        ].dropna()
-
         # get data
         (
             self.input_data,
             self.objective_data,
             self.constraint_data,
-        ) = self.vocs.extract_data(valid_data, return_raw=True)
+        ) = self.vocs.extract_data(data, return_raw=True)
 
-        self.train_X = torch.tensor(self.input_data.to_numpy(), **self.tkwargs)
         self.input_transform.to(**self.tkwargs)
         if self.likelihood is not None:
             self.likelihood.to(**self.tkwargs)
 
     def build_model(self, data: pd.DataFrame, tkwargs: dict = None) -> ModelListGP:
         """construct independent model for each objective and constraint"""
         # overwrite tkwargs if specified
@@ -55,61 +49,62 @@
 
         # collect data from dataframe
         self.collect_data(data)
 
         # build model
         return self.build_standard_model()
 
+    def build_mean_module(self, name, outcome_transform) -> Optional[CustomMean]:
+        """Builds the mean module for the output specified by name."""
+        mean_module = self._get_module(self.options.mean_modules, name)
+        if mean_module is not None:
+            mean_module = CustomMean(mean_module, self.input_transform,
+                                     outcome_transform)
+        return mean_module
+
+    def _get_training_data(self, name) -> (torch.Tensor, torch.Tensor):
+        """Returns (train_X, train_Y) for the output specified by name."""
+        # objective specifics
+        if name in self.vocs.objective_names:
+            target_data = self.objective_data
+        # constraint specifics
+        elif name in self.vocs.constraint_names:
+            target_data = self.constraint_data
+        else:
+            raise RuntimeError(
+                "Output '{}' is not found in either objectives or "
+                "constraints.".format(name)
+            )
+        train_X = torch.tensor(
+            self.input_data[~target_data[name].isnull()].to_numpy(),
+            **self.tkwargs)
+        train_Y = torch.tensor(
+            target_data[~target_data[name].isnull()][name].to_numpy(),
+            **self.tkwargs).unsqueeze(-1)
+        return train_X, train_Y
+
     def build_standard_model(self, **model_kwargs):
+        pd.options.mode.use_inf_as_na = True
         models = []
         for name in self.vocs.output_names:
             outcome_transform = Standardize(1)
             covar_module = self._get_module(self.options.covar_modules, name)
-            mean_module = self._get_module(self.options.mean_modules, name)
-
-            # objective specifics
-            if name in self.vocs.objective_names:
-                # if we are doing minimization add a negative sign to the prior model
-                # if self.vocs.objectives[name] == "MINIMIZE" and mean_module is not
-                # None:
-                #    mean_module = _NegativeModule(mean_module)
-
-                train_Y = torch.tensor(
-                    self.objective_data[name].to_numpy(), **self.tkwargs
-                ).unsqueeze(-1)
-
-            # constraint specific
-            elif name in self.vocs.constraint_names:
-                train_Y = torch.tensor(
-                    self.constraint_data[name].to_numpy(), **self.tkwargs
-                ).unsqueeze(-1)
-
-            else:
-                raise RuntimeError(
-                    "if you are recieving this message there is "
-                    "something wrong with vocs"
-                )
-
-            if mean_module is not None:
-                mean_module = CustomMean(
-                    mean_module, self.input_transform, outcome_transform
-                )
-
+            mean_module = self.build_mean_module(name, outcome_transform)
+            train_X, train_Y = self._get_training_data(name)
             models.append(
                 self.build_single_task_gp(
-                    self.train_X,
+                    train_X,
                     train_Y,
                     input_transform=self.input_transform,
                     outcome_transform=outcome_transform,
                     covar_module=covar_module,
                     mean_module=mean_module,
                     likelihood=self.likelihood,
                 )
             )
-
         return ModelListGP(*models)
 
     @staticmethod
     def _get_module(base, name):
         if isinstance(base, Module):
             return base
         elif isinstance(base, dict):
```

### Comparing `xopt-1.3.1/xopt/generators/bayesian/models/time_dependent.py` & `xopt-1.4.0/xopt/generators/bayesian/models/time_dependent.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,14 @@
     def build_model(self, data: pd.DataFrame, tkwargs: dict = None) -> ModelListGP:
         self.tkwargs = tkwargs or {"dtype": torch.double, "device": "cpu"}
 
         self.collect_data(data)
 
         # add time column to variable data
         self.input_data = pd.concat([self.input_data, data["time"]], axis=1)
-        self.train_X = torch.tensor(self.input_data.to_numpy(), **tkwargs)
 
         # add bounds for input transformation
         bounds = np.hstack(
             [
                 self.vocs.bounds,
                 np.array(
                     (
```

### Comparing `xopt-1.3.1/xopt/generators/bayesian/models/transformed_model.py` & `xopt-1.4.0/xopt/generators/bayesian/models/transformed_model.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,42 @@
 import torch
 
 
 class TransformedModel(torch.nn.Module):
-    """
-    Fixed model that requires an input and outcome transform to evaluate
-    Transformer objects must have a forward method that transforms tensors into input
-    coordinates for model and an untransform method that does the reverse.
-    """
-
-    def __init__(self, model, input_transformer, outcome_transformer):
-        """
-        model: torch.nn.Module object
-        input_transformer:
+    def __init__(
+            self,
+            model: torch.nn.Module,
+            input_transformer,
+            outcome_transformer,
+            fixed_model: bool = True
+    ):
+        """A model that requires an input and outcome transform to evaluate.
+
+        Transformer objects must have a forward method that transforms tensors
+        into input coordinates for model and an untransform method that does
+        the reverse.
+
+        model: Representation of the model.
+        input_transformer: Module used to transform inputs.
+        outcome_transformer: Module used to transform outcomes.
+        fixed_model: If true, the model is put in evaluation mode and
+          gradient computation is deactivated.
         """
         super().__init__()
-        self.model = model
-        self.model.eval()
-        self.model.requires_grad_(False)
+        self._model = model
+        if fixed_model:
+            self._model.eval()
+            self._model.requires_grad_(False)
         self.input_transformer = input_transformer
         self.outcome_transformer = outcome_transformer
 
+    @property
+    def model(self):
+        return self._model
+
     def set_transformers(self, eval_mode=True):
         """set transformers to eval mode if they are torch.nn.Module objects -
         prevents transformer training during evaluation
         if `eval_mode` is true set to eval, otherwise set to train
         """
         modules = [self.input_transformer, self.outcome_transformer]
         for m in modules:
@@ -31,15 +44,15 @@
                 if eval_mode:
                     m.eval()
                 else:
                     m.train()
 
     def evaluate_model(self, x):
         """Placeholder method which can be used to modify model calls."""
-        return self.model(x)
+        return self._model(x)
 
     def forward(self, x):
         # set transformers to eval mode
         self.set_transformers(eval_mode=True)
 
         # transform inputs to model space
         x_model = self.input_transformer(x)
```

### Comparing `xopt-1.3.1/xopt/generators/bayesian/models/utils.py` & `xopt-1.4.0/xopt/generators/bayesian/models/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from xopt.generators.bayesian.models.standard import StandardModelConstructor
 from xopt.generators.bayesian.models.time_dependent import TimeDependentModelConstructor
+from xopt.generators.bayesian.models.trainable_mean import TrainableMeanModelConstructor
 
 
 def get_model_constructor(model_options):
     if model_options.custom_constructor:
         constructor = model_options.custom_constructor
     else:
         name = model_options.name
         if name == "standard":
             constructor = StandardModelConstructor
         elif name == "time_dependent_standard":
             constructor = TimeDependentModelConstructor
+        elif name == "trainable_mean_standard":
+            constructor = TrainableMeanModelConstructor
         else:
             raise ValueError(f"{name} is not a vaild model name")
 
     return constructor
```

### Comparing `xopt-1.3.1/xopt/generators/bayesian/multi_fidelity.py` & `xopt-1.4.0/xopt/generators/bayesian/multi_fidelity.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.1/xopt/generators/bayesian/objectives.py` & `xopt-1.4.0/xopt/generators/bayesian/objectives.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.1/xopt/generators/bayesian/options.py` & `xopt-1.4.0/xopt/generators/bayesian/options.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.1/xopt/generators/bayesian/time_dependent.py` & `xopt-1.4.0/xopt/generators/bayesian/time_dependent.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.1/xopt/generators/bayesian/turbo.py` & `xopt-1.4.0/xopt/generators/bayesian/turbo.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.1/xopt/generators/bayesian/upper_confidence_bound.py` & `xopt-1.4.0/xopt/generators/bayesian/upper_confidence_bound.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.1/xopt/generators/bayesian/utils.py` & `xopt-1.4.0/xopt/generators/bayesian/utils.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.1/xopt/generators/es/extremumseeking.py` & `xopt-1.4.0/xopt/generators/es/extremumseeking.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.1/xopt/generators/ga/cnsga.py` & `xopt-1.4.0/xopt/generators/ga/cnsga.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.1/xopt/generators/ga/deap_creator.py` & `xopt-1.4.0/xopt/generators/ga/deap_creator.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.1/xopt/generators/ga/deap_fitness_with_constraints.py` & `xopt-1.4.0/xopt/generators/ga/deap_fitness_with_constraints.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.1/xopt/generators/ga/fitness_with_constraints.py` & `xopt-1.4.0/xopt/generators/ga/fitness_with_constraints.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.1/xopt/generators/random.py` & `xopt-1.4.0/xopt/generators/random.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.1/xopt/generators/rcds/rcds.py` & `xopt-1.4.0/xopt/generators/rcds/rcds.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.1/xopt/generators/scipy/neldermead.py` & `xopt-1.4.0/xopt/generators/scipy/neldermead.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.1/xopt/log.py` & `xopt-1.4.0/xopt/log.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.1/xopt/mpi/run.py` & `xopt-1.4.0/xopt/mpi/run.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.1/xopt/pydantic.py` & `xopt-1.4.0/xopt/pydantic.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.1/xopt/resources/test_functions/modified_tnk.py` & `xopt-1.4.0/xopt/resources/test_functions/modified_tnk.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.1/xopt/resources/test_functions/rosenbrock.py` & `xopt-1.4.0/xopt/resources/test_functions/rosenbrock.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.1/xopt/resources/test_functions/tnk.py` & `xopt-1.4.0/xopt/resources/test_functions/tnk.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.1/xopt/resources/testing.py` & `xopt-1.4.0/xopt/resources/testing.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.1/xopt/utils.py` & `xopt-1.4.0/xopt/utils.py`

 * *Files identical despite different names*

### Comparing `xopt-1.3.1/xopt/vocs.py` & `xopt-1.4.0/xopt/vocs.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,32 +136,37 @@
         return len(self.constraints)
 
     @property
     def n_outputs(self):
         """Returns the number of outputs (objectives and constraints)"""
         return self.n_objectives + self.n_constraints
 
-    def random_inputs(
-        self, n=None, include_constants=True, include_linked_variables=True
-    ):
+    def random_inputs(self, n=None, include_constants=True,
+                      include_linked_variables=True, seed=None):
         """
         Uniform sampling of the variables.
 
         Returns a dict of inputs.
 
         If include_constants, the vocs.constants are added to the dict.
 
         Optional:
             n (integer) to make arrays of inputs, of size n.
+            seed (integer) to initialize the random number generator
 
         """
         inputs = {}
+        if seed is None:
+            rng_sample_function = np.random.random
+        else:
+            rng = np.random.default_rng(seed=seed)
+            rng_sample_function = rng.random
         for key, val in self.variables.items():  # No need to sort here
             a, b = val
-            x = np.random.random(n)
+            x = rng_sample_function(n)
             inputs[key] = x * a + (1 - x) * b
 
         # Constants
         if include_constants and self.constants is not None:
             inputs.update(self.constants)
 
         # Handle linked variables
```

### Comparing `xopt-1.3.1/xopt.egg-info/PKG-INFO` & `xopt-1.4.0/xopt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xopt
-Version: 1.3.1
+Version: 1.4.0
 Home-page: https://github.com/ChristopherMayes/xopt
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
   <img src="docs/assets/Xopt-logo.png", width="200">
```

### Comparing `xopt-1.3.1/xopt.egg-info/SOURCES.txt` & `xopt-1.4.0/xopt.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 tests/generators/bayesian/test_bayesian_generator.py
 tests/generators/bayesian/test_bayesian_options.py
 tests/generators/bayesian/test_custom_model.py
 tests/generators/bayesian/test_expected_improvement.py
 tests/generators/bayesian/test_high_level.py
 tests/generators/bayesian/test_mggpo.py
 tests/generators/bayesian/test_mobo.py
+tests/generators/bayesian/test_model_constructor.py
 tests/generators/bayesian/test_multi_fidelity.py
 tests/generators/bayesian/test_time_dependent_bo.py
 tests/generators/bayesian/test_turbo.py
 tests/generators/bayesian/test_upper_confidence_bound.py
 tests/generators/bayesian/test_utils.py
 xopt/__init__.py
 xopt/_version.py
@@ -67,14 +68,15 @@
 xopt/generators/bayesian/custom_botorch/identity.py
 xopt/generators/bayesian/custom_botorch/multi_fidelity.py
 xopt/generators/bayesian/custom_botorch/proximal.py
 xopt/generators/bayesian/models/__init__.py
 xopt/generators/bayesian/models/prior_mean.py
 xopt/generators/bayesian/models/standard.py
 xopt/generators/bayesian/models/time_dependent.py
+xopt/generators/bayesian/models/trainable_mean.py
 xopt/generators/bayesian/models/transformed_model.py
 xopt/generators/bayesian/models/utils.py
 xopt/generators/es/__init__.py
 xopt/generators/es/extremumseeking.py
 xopt/generators/ga/__init__.py
 xopt/generators/ga/cnsga.py
 xopt/generators/ga/deap_creator.py
```

