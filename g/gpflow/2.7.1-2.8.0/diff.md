# Comparing `tmp/gpflow-2.7.1.tar.gz` & `tmp/gpflow-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gpflow-2.7.1.tar", last modified: Thu Mar 16 14:39:37 2023, max compression
+gzip compressed data, was "dist/gpflow-2.8.0.tar", last modified: Thu May  4 08:51:21 2023, max compression
```

## Comparing `gpflow-2.7.1.tar` & `gpflow-2.8.0.tar`

### file list

```diff
@@ -1,261 +1,262 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 14:39:37.000000 gpflow-2.7.1/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2023-03-16 14:39:23.000000 gpflow-2.7.1/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      182 2023-03-16 14:39:23.000000 gpflow-2.7.1/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12653 2023-03-16 14:39:37.000000 gpflow-2.7.1/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11316 2023-03-16 14:39:23.000000 gpflow-2.7.1/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20330 2023-03-16 14:39:23.000000 gpflow-2.7.1/RELEASE.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-03-16 14:39:23.000000 gpflow-2.7.1/VERSION
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 14:39:37.000000 gpflow-2.7.1/benchmark/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-03-16 14:39:23.000000 gpflow-2.7.1/benchmark/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9767 2023-03-16 14:39:23.000000 gpflow-2.7.1/benchmark/benchmark_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3524 2023-03-16 14:39:23.000000 gpflow-2.7.1/benchmark/benchmarks.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10736 2023-03-16 14:39:23.000000 gpflow-2.7.1/benchmark/dataset_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4590 2023-03-16 14:39:23.000000 gpflow-2.7.1/benchmark/datasets.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8301 2023-03-16 14:39:23.000000 gpflow-2.7.1/benchmark/grouping.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6597 2023-03-16 14:39:23.000000 gpflow-2.7.1/benchmark/metadata.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1652 2023-03-16 14:39:23.000000 gpflow-2.7.1/benchmark/metric_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3286 2023-03-16 14:39:23.000000 gpflow-2.7.1/benchmark/metrics.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3137 2023-03-16 14:39:23.000000 gpflow-2.7.1/benchmark/model_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2921 2023-03-16 14:39:23.000000 gpflow-2.7.1/benchmark/models.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1475 2023-03-16 14:39:23.000000 gpflow-2.7.1/benchmark/paths.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6093 2023-03-16 14:39:23.000000 gpflow-2.7.1/benchmark/plot.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2792 2023-03-16 14:39:23.000000 gpflow-2.7.1/benchmark/plotter_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4478 2023-03-16 14:39:23.000000 gpflow-2.7.1/benchmark/plotters.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2438 2023-03-16 14:39:23.000000 gpflow-2.7.1/benchmark/registry.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12862 2023-03-16 14:39:23.000000 gpflow-2.7.1/benchmark/run.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3496 2023-03-16 14:39:23.000000 gpflow-2.7.1/benchmark/sharding.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4781 2023-03-16 14:39:23.000000 gpflow-2.7.1/benchmark/tag.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 14:39:37.000000 gpflow-2.7.1/doc/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 14:39:37.000000 gpflow-2.7.1/doc/sphinx/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      398 2023-03-16 14:39:23.000000 gpflow-2.7.1/doc/sphinx/benchmarks.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)       45 2023-03-16 14:39:23.000000 gpflow-2.7.1/doc/sphinx/bibliography.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3109 2023-03-16 14:39:23.000000 gpflow-2.7.1/doc/sphinx/conf.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1473 2023-03-16 14:39:23.000000 gpflow-2.7.1/doc/sphinx/getting_started.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7585 2023-03-16 14:39:23.000000 gpflow-2.7.1/doc/sphinx/index.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2468 2023-03-16 14:39:23.000000 gpflow-2.7.1/doc/sphinx/installation.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4444 2023-03-16 14:39:23.000000 gpflow-2.7.1/doc/sphinx/user_guide.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 14:39:37.000000 gpflow-2.7.1/gpflow/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1745 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13183 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1772 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/ci_utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 14:39:37.000000 gpflow-2.7.1/gpflow/conditionals/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      445 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/conditionals/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5399 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/conditionals/conditionals.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1293 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/conditionals/dispatch.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 14:39:37.000000 gpflow-2.7.1/gpflow/conditionals/multioutput/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      110 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/conditionals/multioutput/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11061 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/conditionals/multioutput/conditionals.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3007 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/conditionals/multioutput/sample_conditionals.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3281 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/conditionals/sample_conditionals.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6231 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/conditionals/uncertain_conditionals.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23736 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/conditionals/util.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 14:39:37.000000 gpflow-2.7.1/gpflow/config/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11223 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/config/__config__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      528 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/config/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 14:39:37.000000 gpflow-2.7.1/gpflow/covariances/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      165 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/covariances/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      695 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/covariances/dispatch.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2665 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/covariances/kufs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2370 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/covariances/kuus.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 14:39:37.000000 gpflow-2.7.1/gpflow/covariances/multioutput/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       64 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/covariances/multioutput/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6858 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/covariances/multioutput/kufs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4048 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/covariances/multioutput/kuus.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 14:39:37.000000 gpflow-2.7.1/gpflow/expectations/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      454 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/expectations/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5380 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/expectations/cross_kernels.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      813 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/expectations/dispatch.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5479 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/expectations/expectations.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5954 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/expectations/linears.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6170 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/expectations/mean_functions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7115 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/expectations/misc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4450 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/expectations/products.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6814 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/expectations/quadratures.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10043 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/expectations/squared_exponentials.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4972 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/expectations/sums.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 14:39:37.000000 gpflow-2.7.1/gpflow/experimental/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      879 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/experimental/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1551 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/experimental/utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10582 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/functions.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 14:39:37.000000 gpflow-2.7.1/gpflow/inducing_variables/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      785 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/inducing_variables/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      708 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/inducing_variables/inducing_patch.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3690 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/inducing_variables/inducing_variables.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 14:39:37.000000 gpflow-2.7.1/gpflow/inducing_variables/multioutput/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      515 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/inducing_variables/multioutput/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7262 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/inducing_variables/multioutput/inducing_variables.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 14:39:37.000000 gpflow-2.7.1/gpflow/kernels/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2513 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/kernels/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10659 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/kernels/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6817 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/kernels/changepoints.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6351 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/kernels/convolutional.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3844 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/kernels/linears.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11102 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/kernels/misc.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 14:39:37.000000 gpflow-2.7.1/gpflow/kernels/multioutput/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      311 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/kernels/multioutput/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15660 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/kernels/multioutput/kernels.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4042 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/kernels/periodic.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2823 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/kernels/statics.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11179 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/kernels/stationaries.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5901 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/kullback_leiblers.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 14:39:37.000000 gpflow-2.7.1/gpflow/likelihoods/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3720 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/likelihoods/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24692 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/likelihoods/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      869 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/likelihoods/misc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9162 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/likelihoods/multiclass.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4782 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/likelihoods/multilatent.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11354 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/likelihoods/scalar_continuous.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7553 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/likelihoods/scalar_discrete.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      948 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/likelihoods/utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4530 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/logdensities.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1022 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/mean_functions.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 14:39:37.000000 gpflow-2.7.1/gpflow/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1909 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/models/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14250 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/models/cglb.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11614 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/models/gplvm.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4451 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/models/gpmc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7000 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/models/gpr.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13688 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/models/model.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4718 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/models/sgpmc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22082 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/models/sgpr.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10487 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/models/svgp.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5794 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/models/training_mixins.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3692 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/models/util.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15454 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/models/vgp.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 14:39:37.000000 gpflow-2.7.1/gpflow/monitor/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      915 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/monitor/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5300 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/monitor/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8983 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/monitor/tensorboard.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      839 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/mypy_flags.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 14:39:37.000000 gpflow-2.7.1/gpflow/optimizers/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      269 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/optimizers/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5294 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/optimizers/mcmc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18062 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/optimizers/natgrad.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9075 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/optimizers/scipy.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    40522 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/posteriors.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3005 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/probability_distributions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       27 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/py.typed
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 14:39:37.000000 gpflow-2.7.1/gpflow/quadrature/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      360 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/quadrature/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4887 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/quadrature/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9494 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/quadrature/deprecated.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5590 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/quadrature/gauss_hermite.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1784 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/type_flags.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 14:39:37.000000 gpflow-2.7.1/gpflow/utilities/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1217 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/utilities/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2169 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/utilities/bijectors.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3724 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/utilities/misc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1547 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/utilities/model_utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3325 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/utilities/multipledispatch.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5626 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/utilities/ops.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1736 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/utilities/parameter_or_function.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13979 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/utilities/traversal.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      177 2023-03-16 14:39:23.000000 gpflow-2.7.1/gpflow/versions.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 14:39:37.000000 gpflow-2.7.1/gpflow.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12653 2023-03-16 14:39:37.000000 gpflow-2.7.1/gpflow.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7251 2023-03-16 14:39:37.000000 gpflow-2.7.1/gpflow.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-03-16 14:39:37.000000 gpflow-2.7.1/gpflow.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      354 2023-03-16 14:39:37.000000 gpflow-2.7.1/gpflow.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       23 2023-03-16 14:39:37.000000 gpflow-2.7.1/gpflow.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-03-16 14:39:37.000000 gpflow-2.7.1/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2592 2023-03-16 14:39:23.000000 gpflow-2.7.1/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 14:39:37.000000 gpflow-2.7.1/tests/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 14:39:37.000000 gpflow-2.7.1/tests/gpflow/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 14:39:37.000000 gpflow-2.7.1/tests/gpflow/conditionals/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/conditionals/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7895 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/conditionals/test_broadcasted_conditionals.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6959 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/conditionals/test_conditionals.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    32563 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/conditionals/test_multioutput.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10722 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/conditionals/test_uncertain_conditional.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4537 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/conditionals/test_util.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 14:39:37.000000 gpflow-2.7.1/tests/gpflow/config/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/config/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6006 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/config/test_config.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1278 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/conftest.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 14:39:37.000000 gpflow-2.7.1/tests/gpflow/covariances/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/covariances/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4244 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/covariances/test_base_covariances.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4968 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/covariances/test_multioutput.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 14:39:37.000000 gpflow-2.7.1/tests/gpflow/expectations/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/expectations/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12096 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/expectations/test_expectations.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 14:39:37.000000 gpflow-2.7.1/tests/gpflow/experimental/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/experimental/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      954 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/experimental/test_utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 14:39:37.000000 gpflow-2.7.1/tests/gpflow/kernels/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/kernels/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3473 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/kernels/reference.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9065 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/kernels/test_broadcasting.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      475 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/kernels/test_changepoints.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7805 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/kernels/test_coregion.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20972 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/kernels/test_kernels.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2071 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/kernels/test_positive_semidefinite.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1940 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/kernels/test_scaled_euclid_dist.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 14:39:37.000000 gpflow-2.7.1/tests/gpflow/likelihoods/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/likelihoods/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7752 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/likelihoods/test_function_params.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1688 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/likelihoods/test_heteroskedastic.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5586 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/likelihoods/test_heteroskedastic_constant_variance.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11288 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/likelihoods/test_likelihoods.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8112 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/likelihoods/test_multiclass.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7141 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/likelihoods/test_switched_likelihood.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 14:39:37.000000 gpflow-2.7.1/tests/gpflow/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/models/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6499 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/models/test_cglb.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3806 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/models/test_gplvm.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2220 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/models/test_gpr.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2496 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/models/test_gpr_posterior.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1814 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/models/test_mcmc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3160 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/models/test_methods.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7970 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/models/test_model_predict.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2662 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/models/test_sgpr.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4189 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/models/test_sgpr_posterior.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6777 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/models/test_svgp.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3056 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/models/test_svgp_posterior.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1042 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/models/test_training_mixins.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8714 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/models/test_variational.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1991 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/models/test_vgp.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2997 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/models/test_vgp_posterior.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 14:39:37.000000 gpflow-2.7.1/tests/gpflow/optimizers/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/optimizers/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7811 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/optimizers/test_mcmc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6341 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/optimizers/test_natural_gradient.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4763 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/optimizers/test_scipy.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 14:39:37.000000 gpflow-2.7.1/tests/gpflow/posteriors/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/posteriors/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2280 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/posteriors/conftest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13721 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/posteriors/test_bo_integration.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    27405 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/posteriors/test_posteriors.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3877 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/test_all.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9354 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/test_base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4993 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/test_base_prior.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4057 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/test_base_training.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13060 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/test_functions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4391 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/test_inducing_variables.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5127 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/test_initial_value.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9171 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/test_kullback_leiblers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4339 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/test_logdensities.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9554 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/test_monitor.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 14:39:37.000000 gpflow-2.7.1/tests/gpflow/utilities/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/utilities/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2224 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/utilities/test_bijectors.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3094 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/utilities/test_deepcopy.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2740 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/utilities/test_misc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2785 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/utilities/test_model_utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3422 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/utilities/test_multipledispatch.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2251 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/utilities/test_ops.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3234 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/utilities/test_parameter_or_function.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1232 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/utilities/test_set_trainable.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1845 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/utilities/test_training_loop.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21264 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/utilities/test_traversal.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1226 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/gpflow/utilities/test_utilities.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 14:39:37.000000 gpflow-2.7.1/tests/integration/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/integration/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2481 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/integration/test_benchmark.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1441 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/integration/test_docs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5442 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/integration/test_dynamic_shapes.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3329 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/integration/test_linear_noise.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11174 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/integration/test_method_equivalence.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1393 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/integration/test_model_serialization.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3020 2023-03-16 14:39:23.000000 gpflow-2.7.1/tests/integration/test_notebooks.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2023-05-04 08:51:07.000000 gpflow-2.8.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      182 2023-05-04 08:51:07.000000 gpflow-2.8.0/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12653 2023-05-04 08:51:21.000000 gpflow-2.8.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11316 2023-05-04 08:51:07.000000 gpflow-2.8.0/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21377 2023-05-04 08:51:07.000000 gpflow-2.8.0/RELEASE.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-05-04 08:51:07.000000 gpflow-2.8.0/VERSION
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/benchmark/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:07.000000 gpflow-2.8.0/benchmark/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9767 2023-05-04 08:51:07.000000 gpflow-2.8.0/benchmark/benchmark_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3524 2023-05-04 08:51:07.000000 gpflow-2.8.0/benchmark/benchmarks.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10736 2023-05-04 08:51:07.000000 gpflow-2.8.0/benchmark/dataset_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4590 2023-05-04 08:51:07.000000 gpflow-2.8.0/benchmark/datasets.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8301 2023-05-04 08:51:07.000000 gpflow-2.8.0/benchmark/grouping.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6597 2023-05-04 08:51:07.000000 gpflow-2.8.0/benchmark/metadata.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1652 2023-05-04 08:51:07.000000 gpflow-2.8.0/benchmark/metric_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3286 2023-05-04 08:51:07.000000 gpflow-2.8.0/benchmark/metrics.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3137 2023-05-04 08:51:07.000000 gpflow-2.8.0/benchmark/model_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2921 2023-05-04 08:51:07.000000 gpflow-2.8.0/benchmark/models.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1475 2023-05-04 08:51:07.000000 gpflow-2.8.0/benchmark/paths.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6093 2023-05-04 08:51:07.000000 gpflow-2.8.0/benchmark/plot.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2792 2023-05-04 08:51:07.000000 gpflow-2.8.0/benchmark/plotter_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4478 2023-05-04 08:51:07.000000 gpflow-2.8.0/benchmark/plotters.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2438 2023-05-04 08:51:07.000000 gpflow-2.8.0/benchmark/registry.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12862 2023-05-04 08:51:07.000000 gpflow-2.8.0/benchmark/run.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3496 2023-05-04 08:51:07.000000 gpflow-2.8.0/benchmark/sharding.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4781 2023-05-04 08:51:07.000000 gpflow-2.8.0/benchmark/tag.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/doc/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/doc/sphinx/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      398 2023-05-04 08:51:07.000000 gpflow-2.8.0/doc/sphinx/benchmarks.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       45 2023-05-04 08:51:07.000000 gpflow-2.8.0/doc/sphinx/bibliography.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3109 2023-05-04 08:51:07.000000 gpflow-2.8.0/doc/sphinx/conf.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1473 2023-05-04 08:51:07.000000 gpflow-2.8.0/doc/sphinx/getting_started.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7585 2023-05-04 08:51:07.000000 gpflow-2.8.0/doc/sphinx/index.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2468 2023-05-04 08:51:07.000000 gpflow-2.8.0/doc/sphinx/installation.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4444 2023-05-04 08:51:07.000000 gpflow-2.8.0/doc/sphinx/user_guide.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/gpflow/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1745 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13183 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1772 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/ci_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/gpflow/conditionals/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      445 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/conditionals/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5399 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/conditionals/conditionals.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1293 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/conditionals/dispatch.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/gpflow/conditionals/multioutput/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      110 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/conditionals/multioutput/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11061 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/conditionals/multioutput/conditionals.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3007 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/conditionals/multioutput/sample_conditionals.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3281 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/conditionals/sample_conditionals.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6231 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/conditionals/uncertain_conditionals.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23736 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/conditionals/util.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/gpflow/config/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12677 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/config/__config__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      618 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/config/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/gpflow/covariances/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      165 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/covariances/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      695 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/covariances/dispatch.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2665 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/covariances/kufs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2370 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/covariances/kuus.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/gpflow/covariances/multioutput/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       64 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/covariances/multioutput/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6858 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/covariances/multioutput/kufs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4048 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/covariances/multioutput/kuus.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/gpflow/expectations/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      454 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/expectations/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5380 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/expectations/cross_kernels.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      813 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/expectations/dispatch.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5479 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/expectations/expectations.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5954 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/expectations/linears.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6170 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/expectations/mean_functions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7115 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/expectations/misc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4450 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/expectations/products.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6814 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/expectations/quadratures.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10043 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/expectations/squared_exponentials.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4972 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/expectations/sums.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/gpflow/experimental/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      879 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/experimental/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1551 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/experimental/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10582 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/functions.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/gpflow/inducing_variables/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      785 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/inducing_variables/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      708 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/inducing_variables/inducing_patch.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3690 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/inducing_variables/inducing_variables.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/gpflow/inducing_variables/multioutput/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      515 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/inducing_variables/multioutput/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7262 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/inducing_variables/multioutput/inducing_variables.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/gpflow/kernels/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2532 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/kernels/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10659 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/kernels/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5135 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/kernels/categorical.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6817 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/kernels/changepoints.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6351 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/kernels/convolutional.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3844 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/kernels/linears.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11102 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/kernels/misc.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/gpflow/kernels/multioutput/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      311 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/kernels/multioutput/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15660 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/kernels/multioutput/kernels.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4042 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/kernels/periodic.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2823 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/kernels/statics.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11179 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/kernels/stationaries.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5901 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/kullback_leiblers.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/gpflow/likelihoods/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3720 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/likelihoods/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24692 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/likelihoods/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      869 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/likelihoods/misc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9162 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/likelihoods/multiclass.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4782 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/likelihoods/multilatent.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11574 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/likelihoods/scalar_continuous.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7553 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/likelihoods/scalar_discrete.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      948 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/likelihoods/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4530 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/logdensities.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1022 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/mean_functions.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/gpflow/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1909 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/models/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14250 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/models/cglb.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11614 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/models/gplvm.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4451 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/models/gpmc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7000 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/models/gpr.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13688 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/models/model.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4718 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/models/sgpmc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22082 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/models/sgpr.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10487 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/models/svgp.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5794 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/models/training_mixins.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3692 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/models/util.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15454 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/models/vgp.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/gpflow/monitor/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      915 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/monitor/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5300 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/monitor/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8983 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/monitor/tensorboard.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      839 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/mypy_flags.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/gpflow/optimizers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      269 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/optimizers/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5294 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/optimizers/mcmc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18062 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/optimizers/natgrad.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9750 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/optimizers/scipy.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    40522 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/posteriors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3005 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/probability_distributions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       27 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/py.typed
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/gpflow/quadrature/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      360 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/quadrature/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4887 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/quadrature/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9494 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/quadrature/deprecated.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5590 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/quadrature/gauss_hermite.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1784 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/type_flags.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/gpflow/utilities/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1217 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/utilities/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2169 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/utilities/bijectors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3724 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/utilities/misc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1547 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/utilities/model_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3325 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/utilities/multipledispatch.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5626 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/utilities/ops.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1736 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/utilities/parameter_or_function.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13979 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/utilities/traversal.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      177 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/versions.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/gpflow.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12653 2023-05-04 08:51:21.000000 gpflow-2.8.0/gpflow.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7281 2023-05-04 08:51:21.000000 gpflow-2.8.0/gpflow.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-04 08:51:21.000000 gpflow-2.8.0/gpflow.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      354 2023-05-04 08:51:21.000000 gpflow-2.8.0/gpflow.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       23 2023-05-04 08:51:21.000000 gpflow-2.8.0/gpflow.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-05-04 08:51:21.000000 gpflow-2.8.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2592 2023-05-04 08:51:07.000000 gpflow-2.8.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/tests/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/tests/gpflow/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/tests/gpflow/conditionals/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/conditionals/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7895 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/conditionals/test_broadcasted_conditionals.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6959 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/conditionals/test_conditionals.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    32563 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/conditionals/test_multioutput.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10722 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/conditionals/test_uncertain_conditional.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4537 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/conditionals/test_util.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/tests/gpflow/config/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/config/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6991 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/config/test_config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1278 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/conftest.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/tests/gpflow/covariances/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/covariances/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4244 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/covariances/test_base_covariances.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4968 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/covariances/test_multioutput.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/tests/gpflow/expectations/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/expectations/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12096 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/expectations/test_expectations.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/tests/gpflow/experimental/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/experimental/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      954 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/experimental/test_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/tests/gpflow/kernels/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/kernels/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3473 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/kernels/reference.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9302 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/kernels/test_broadcasting.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      475 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/kernels/test_changepoints.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7805 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/kernels/test_coregion.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23223 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/kernels/test_kernels.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2071 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/kernels/test_positive_semidefinite.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1940 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/kernels/test_scaled_euclid_dist.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/tests/gpflow/likelihoods/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/likelihoods/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7752 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/likelihoods/test_function_params.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1688 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/likelihoods/test_heteroskedastic.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5586 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/likelihoods/test_heteroskedastic_constant_variance.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11288 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/likelihoods/test_likelihoods.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8112 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/likelihoods/test_multiclass.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7141 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/likelihoods/test_switched_likelihood.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/tests/gpflow/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/models/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6499 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/models/test_cglb.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3806 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/models/test_gplvm.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2220 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/models/test_gpr.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2496 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/models/test_gpr_posterior.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1814 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/models/test_mcmc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3160 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/models/test_methods.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7970 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/models/test_model_predict.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2662 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/models/test_sgpr.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4189 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/models/test_sgpr_posterior.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6777 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/models/test_svgp.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3056 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/models/test_svgp_posterior.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1042 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/models/test_training_mixins.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8714 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/models/test_variational.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1991 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/models/test_vgp.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2997 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/models/test_vgp_posterior.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/tests/gpflow/optimizers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/optimizers/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7811 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/optimizers/test_mcmc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6341 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/optimizers/test_natural_gradient.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7186 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/optimizers/test_scipy.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/tests/gpflow/posteriors/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/posteriors/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2280 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/posteriors/conftest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13721 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/posteriors/test_bo_integration.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    27405 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/posteriors/test_posteriors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3877 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/test_all.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9354 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/test_base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4993 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/test_base_prior.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4057 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/test_base_training.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13060 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/test_functions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4391 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/test_inducing_variables.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5127 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/test_initial_value.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9171 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/test_kullback_leiblers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4339 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/test_logdensities.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9554 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/test_monitor.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/tests/gpflow/utilities/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/utilities/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2224 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/utilities/test_bijectors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3094 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/utilities/test_deepcopy.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2740 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/utilities/test_misc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2785 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/utilities/test_model_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3422 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/utilities/test_multipledispatch.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2251 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/utilities/test_ops.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3234 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/utilities/test_parameter_or_function.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1232 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/utilities/test_set_trainable.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1845 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/utilities/test_training_loop.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21264 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/utilities/test_traversal.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1226 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/utilities/test_utilities.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/tests/integration/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/integration/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2481 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/integration/test_benchmark.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1441 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/integration/test_docs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5442 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/integration/test_dynamic_shapes.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3329 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/integration/test_linear_noise.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11174 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/integration/test_method_equivalence.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1393 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/integration/test_model_serialization.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3020 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/integration/test_notebooks.py
```

### Comparing `gpflow-2.7.1/LICENSE` & `gpflow-2.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/PKG-INFO` & `gpflow-2.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpflow
-Version: 2.7.1
+Version: 2.8.0
 Summary: Gaussian process methods in TensorFlow
 Home-page: https://www.gpflow.org
 Author: James Hensman, Alex Matthews
 Author-email: james.hensman@gmail.com
 License: Apache License 2.0
 Project-URL: Source on GitHub, https://github.com/GPflow/GPflow
 Project-URL: Documentation, https://gpflow.github.io/GPflow/
```

### Comparing `gpflow-2.7.1/README.md` & `gpflow-2.8.0/README.md`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/RELEASE.md` & `gpflow-2.8.0/RELEASE.md`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 ## Thanks to our Contributors
 
 This release contains contributions from:
 
 <INSERT>, <NAME>, <HERE>, <USING>, <GITHUB>, <HANDLE>
 
 
-# Release 2.8.0 (next release)
+# Release 2.9.0 (next release)
 
 <INSERT SMALL BLURB ABOUT RELEASE FOCUS AREA AND POTENTIAL TOOLCHAIN CHANGES>
 
 ## Breaking Changes
 
 * <DOCUMENT BREAKING CHANGES HERE>
 * <THIS SECTION SHOULD CONTAIN API AND BEHAVIORAL BREAKING CHANGES>
@@ -46,27 +46,56 @@
 
 * <CAVEATS REGARDING THE RELEASE (BUT NOT BREAKING CHANGES).>
 * <ADDING/BUMPING DEPENDENCIES SHOULD GO HERE>
 * <KNOWN LACK OF SUPPORT ON SOME PLATFORM SHOULD GO HERE>
 
 ## Major Features and Improvements
 
-* Major rework of documentation landing page and "getting started" section.
+* <INSERT MAJOR FEATURE HERE, USING MARKDOWN SYNTAX>
+* <IF RELEASE CONTAINS MULTIPLE FEATURES FROM SAME AREA, GROUP THEM TOGETHER>
 
 ## Bug Fixes and Other Changes
 
-* Fixed bug related to `tf.saved_model` and methods wrapped in `@check_shapes`.
+* <SIMILAR TO ABOVE SECTION, BUT FOR OTHER IMPORTANT CHANGES / BUG FIXES>
+* <IF A CHANGE CLOSES A GITHUB ISSUE, IT SHOULD BE DOCUMENTED HERE>
+* <NOTES SHOULD BE GROUPED PER AREA>
 
 ## Thanks to our Contributors
 
 This release contains contributions from:
 
 <INSERT>, <NAME>, <HERE>, <USING>, <GITHUB>, <HANDLE>
 
 
+# Release 2.8.0
+
+The main focus of this release is to provide users control over arguments for `tf.function`
+compilation inside the Scipy minimize wrapper. It also adds support for a new categorical kernel.
+
+## Major Features and Improvements
+
+* Added a new categorical kernel that implements categorical variables by mapping them to values in
+  a latent space. (#2055)
+* Added support for passing `tf.function` arguments for compilation in `gpflow.optimizers.Scipy`.
+  (#2064)
+* Default lower bound for parameters of scalar likelihoods can now be set via configuration.
+  (#1985, #2066)
+
+## Bug Fixes and Other Changes
+
+* Fixed some notebook typos and a link. (#2052, #2057)
+* Fixed missing docs for `SquaredExponential` and `Constant` kernels. (#2056, #2063)
+
+## Thanks to our Contributors
+
+This release contains contributions from:
+
+sc336, partev, khurram-ghani, uri-granta, awav, jesnie
+
+
 # Release 2.7.1
 
 A small fix for a bug in the scipy optimize wrapper.
 
 ## Breaking Changes
 
 * None
```

### Comparing `gpflow-2.7.1/benchmark/benchmark_api.py` & `gpflow-2.8.0/benchmark/benchmark_api.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/benchmark/benchmarks.py` & `gpflow-2.8.0/benchmark/benchmarks.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/benchmark/dataset_api.py` & `gpflow-2.8.0/benchmark/dataset_api.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/benchmark/datasets.py` & `gpflow-2.8.0/benchmark/datasets.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/benchmark/grouping.py` & `gpflow-2.8.0/benchmark/grouping.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/benchmark/metadata.py` & `gpflow-2.8.0/benchmark/metadata.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/benchmark/metric_api.py` & `gpflow-2.8.0/benchmark/metric_api.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/benchmark/metrics.py` & `gpflow-2.8.0/benchmark/metrics.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/benchmark/model_api.py` & `gpflow-2.8.0/benchmark/model_api.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/benchmark/models.py` & `gpflow-2.8.0/benchmark/models.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/benchmark/paths.py` & `gpflow-2.8.0/benchmark/paths.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/benchmark/plot.py` & `gpflow-2.8.0/benchmark/plot.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/benchmark/plotter_api.py` & `gpflow-2.8.0/benchmark/plotter_api.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/benchmark/plotters.py` & `gpflow-2.8.0/benchmark/plotters.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/benchmark/registry.py` & `gpflow-2.8.0/benchmark/registry.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/benchmark/run.py` & `gpflow-2.8.0/benchmark/run.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/benchmark/sharding.py` & `gpflow-2.8.0/benchmark/sharding.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/benchmark/tag.py` & `gpflow-2.8.0/benchmark/tag.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/doc/sphinx/conf.py` & `gpflow-2.8.0/doc/sphinx/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 # import sys
 # sys.path.insert(0, os.path.abspath('.'))
 
 
 # -- Project information -----------------------------------------------------
 
 project = "GPflow"
-copyright = "2022, The GPflow Contributors"
+copyright = "2023, The GPflow Contributors"
 author = "The GPflow Contributors"
 
 # The full version, including alpha/beta/rc tags
-release = "2.7.1"
+release = "2.8.0"
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
```

### Comparing `gpflow-2.7.1/doc/sphinx/getting_started.rst` & `gpflow-2.8.0/doc/sphinx/getting_started.rst`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/doc/sphinx/index.rst` & `gpflow-2.8.0/doc/sphinx/index.rst`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/doc/sphinx/installation.rst` & `gpflow-2.8.0/doc/sphinx/installation.rst`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/doc/sphinx/user_guide.rst` & `gpflow-2.8.0/doc/sphinx/user_guide.rst`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/__init__.py` & `gpflow-2.8.0/gpflow/__init__.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/base.py` & `gpflow-2.8.0/gpflow/base.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/ci_utils.py` & `gpflow-2.8.0/gpflow/ci_utils.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/conditionals/conditionals.py` & `gpflow-2.8.0/gpflow/conditionals/conditionals.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/conditionals/dispatch.py` & `gpflow-2.8.0/gpflow/conditionals/dispatch.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/conditionals/multioutput/conditionals.py` & `gpflow-2.8.0/gpflow/conditionals/multioutput/conditionals.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/conditionals/multioutput/sample_conditionals.py` & `gpflow-2.8.0/gpflow/conditionals/multioutput/sample_conditionals.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/conditionals/sample_conditionals.py` & `gpflow-2.8.0/gpflow/conditionals/sample_conditionals.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/conditionals/uncertain_conditionals.py` & `gpflow-2.8.0/gpflow/conditionals/uncertain_conditionals.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/conditionals/util.py` & `gpflow-2.8.0/gpflow/conditionals/util.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/config/__config__.py` & `gpflow-2.8.0/gpflow/config/__config__.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 
 Full set of environment variables and available options:
 
 * ``GPFLOW_INT``: "int16", "int32", or "int64"
 * ``GPFLOW_FLOAT``: "float16", "float32", or "float64"
 * ``GPFLOW_POSITIVE_BIJECTOR``: "exp" or "softplus"
 * ``GPFLOW_POSITIVE_MINIMUM``: Any positive float number
+* ``GPFLOW_LIKELIHOOD_POSITIVE_MINIMUM``: Any positive float number
 * ``GPFLOW_SUMMARY_FMT``: "notebook" or any other format that :mod:`tabulate` can handle.
 * ``GPFLOW_JITTER``: Any positive float number
 
 The user can also change the GPflow configuration temporarily with a context
 manager :func:`as_context`:
 
 >>> config = Config(jitter=1e-5)
@@ -48,68 +49,73 @@
 >>>     # ...code here sees new config
 """
 
 import contextlib
 import enum
 import os
 from dataclasses import dataclass, field, replace
-from typing import Any, Dict, Generator, List, Mapping, Optional, Union
+from typing import Any, Dict, Generator, List, Mapping, Optional, Tuple, Union
 
 import numpy as np
 import tabulate
 import tensorflow as tf
 import tensorflow_probability as tfp
 
 __all__ = [
     "Config",
     "as_context",
     "config",
     "default_float",
     "default_int",
     "default_jitter",
+    "default_likelihood_positive_minimum",
     "default_positive_bijector",
     "default_positive_minimum",
     "default_summary_fmt",
     "positive_bijector_type_map",
     "set_config",
     "set_default_float",
     "set_default_int",
     "set_default_jitter",
+    "set_default_likelihood_positive_minimum",
     "set_default_positive_bijector",
     "set_default_positive_minimum",
     "set_default_summary_fmt",
 ]
 
 __config: Optional["Config"] = None
 
 
-class _Values(enum.Enum):
-    """Setting's names collection with default values. The `name` method returns name
-    of the environment variable. E.g. for `SUMMARY_FMT` field the environment variable
-    will be `GPFLOW_SUMMARY_FMT`."""
-
-    INT = np.int32
-    FLOAT = np.float64
-    POSITIVE_BIJECTOR = "softplus"
-    POSITIVE_MINIMUM = 0.0
-    SUMMARY_FMT = "fancy_grid"
-    JITTER = 1e-6
-
-    @property
-    def name(self) -> str:  # type: ignore[override]  # name is generated and has weird typing.
-        return f"GPFLOW_{super().name}"
+@dataclass(frozen=True)
+class _Value:
+    """Individual setting's environment variable name and default value."""
+
+    name: str
+    value: Any
+
 
+class _Values:
+    """Collection of default settings."""
 
-def _default(value: _Values) -> Any:
+    INT = _Value("GPFLOW_INT", np.int32)
+    FLOAT = _Value("GPFLOW_FLOAT", np.float64)
+    POSITIVE_BIJECTOR = _Value("GPFLOW_POSITIVE_BIJECTOR", "softplus")
+    POSITIVE_MINIMUM = _Value("GPFLOW_POSITIVE_MINIMUM", 0.0)
+    LIKELIHOOD_POSITIVE_MINIMUM = _Value("GPFLOW_LIKELIHOOD_POSITIVE_MINIMUM", 1e-6)
+    SUMMARY_FMT = _Value("GPFLOW_SUMMARY_FMT", "fancy_grid")
+    JITTER = _Value("GPFLOW_JITTER", 1e-6)
+
+
+def _default(value: _Value) -> Any:
     """Checks if value is set in the environment."""
     return os.getenv(value.name, default=value.value)
 
 
 def _default_numeric_type_factory(
-    valid_types: Mapping[str, type], enum_key: _Values, type_name: str
+    valid_types: Mapping[str, type], enum_key: _Value, type_name: str
 ) -> type:
     value: Union[str, type] = _default(enum_key)
     if isinstance(value, type) and (value in valid_types.values()):
         return value
     assert isinstance(value, str)  # Hint for mypy
     if value not in valid_types:
         raise TypeError(f"Config cannot recognize {type_name} type.")
@@ -148,14 +154,24 @@
     value = _default(_Values.POSITIVE_MINIMUM)
     try:
         return float(value)
     except ValueError:
         raise TypeError("Config cannot set the positive_minimum value with non float type.")
 
 
+def _default_likelihood_positive_minimum_factory() -> float:
+    value = _default(_Values.LIKELIHOOD_POSITIVE_MINIMUM)
+    try:
+        return float(value)
+    except ValueError:
+        raise TypeError(
+            "Config cannot set the likelihood_positive_minimum value with non float type."
+        )
+
+
 def _default_summary_fmt_factory() -> Optional[str]:
     result: Optional[str] = _default(_Values.SUMMARY_FMT)
     return result
 
 
 # The following type alias is for the Config class, to help a static analyser distinguish
 # between the built-in 'float' type and the 'float' type defined in the that class.
@@ -187,14 +203,19 @@
 
     Default is "softplus".
     """
 
     positive_minimum: Float = field(default_factory=_default_positive_minimum_factory)
     """Lower bound for the positive transformation."""
 
+    likelihood_positive_minimum: Float = field(
+        default_factory=_default_likelihood_positive_minimum_factory
+    )
+    """Lower bound for the positive transformation for positive likelihood parameters."""
+
     summary_fmt: Optional[str] = field(default_factory=_default_summary_fmt_factory)
     """Summary format for module printing."""
 
 
 def config() -> Config:
     """Returns current active config."""
     assert __config is not None, "__config is None. This should never happen."
@@ -226,14 +247,19 @@
 
 
 def default_positive_minimum() -> float:
     """Shift constant that GPflow adds to all positive constraints."""
     return config().positive_minimum
 
 
+def default_likelihood_positive_minimum() -> float:
+    """Shift constant that GPflow adds to all positive likelihood parameter constraints."""
+    return config().likelihood_positive_minimum
+
+
 def default_summary_fmt() -> Optional[str]:
     """Summary printing format as understood by :mod:`tabulate` or a special case "notebook"."""
     return config().summary_fmt
 
 
 def set_config(new_config: Config) -> None:
     """Update GPflow config with new settings from `new_config`."""
@@ -314,14 +340,27 @@
 
     if value < 0:
         raise ValueError("Positive minimum must be non-negative")
 
     set_config(replace(config(), positive_minimum=value))
 
 
+def set_default_likelihood_positive_minimum(value: float) -> None:
+    """Sets shift constant for positive likelihood transformation."""
+    if not (
+        isinstance(value, (tf.Tensor, np.ndarray)) and len(value.shape) == 0
+    ) and not isinstance(value, float):
+        raise TypeError("Expected float32 or float64 scalar value")
+
+    if value < 0:
+        raise ValueError("Likelihood positive minimum must be non-negative")
+
+    set_config(replace(config(), likelihood_positive_minimum=value))
+
+
 def set_default_summary_fmt(value: Optional[str]) -> None:
     formats: List[Optional[str]] = list(tabulate.tabulate_formats)
     formats.extend(["notebook", None])
     if value not in formats:
         raise ValueError(f"Summary does not support '{value}' format")
 
     set_config(replace(config(), summary_fmt=value))
```

### Comparing `gpflow-2.7.1/gpflow/config/__init__.py` & `gpflow-2.8.0/gpflow/config/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,19 +4,21 @@
 __all__ = [
     "Config",
     "as_context",
     "config",
     "default_float",
     "default_int",
     "default_jitter",
+    "default_likelihood_positive_minimum",
     "default_positive_bijector",
     "default_positive_minimum",
     "default_summary_fmt",
     "positive_bijector_type_map",
     "set_config",
     "set_default_float",
     "set_default_int",
     "set_default_jitter",
+    "set_default_likelihood_positive_minimum",
     "set_default_positive_bijector",
     "set_default_positive_minimum",
     "set_default_summary_fmt",
 ]
```

### Comparing `gpflow-2.7.1/gpflow/covariances/dispatch.py` & `gpflow-2.8.0/gpflow/covariances/dispatch.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/covariances/kufs.py` & `gpflow-2.8.0/gpflow/covariances/kufs.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/covariances/kuus.py` & `gpflow-2.8.0/gpflow/covariances/kuus.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/covariances/multioutput/kufs.py` & `gpflow-2.8.0/gpflow/covariances/multioutput/kufs.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/covariances/multioutput/kuus.py` & `gpflow-2.8.0/gpflow/covariances/multioutput/kuus.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/expectations/cross_kernels.py` & `gpflow-2.8.0/gpflow/expectations/cross_kernels.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/expectations/dispatch.py` & `gpflow-2.8.0/gpflow/expectations/dispatch.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/expectations/expectations.py` & `gpflow-2.8.0/gpflow/expectations/expectations.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/expectations/linears.py` & `gpflow-2.8.0/gpflow/expectations/linears.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/expectations/mean_functions.py` & `gpflow-2.8.0/gpflow/expectations/mean_functions.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/expectations/misc.py` & `gpflow-2.8.0/gpflow/expectations/misc.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/expectations/products.py` & `gpflow-2.8.0/gpflow/expectations/products.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/expectations/quadratures.py` & `gpflow-2.8.0/gpflow/expectations/quadratures.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/expectations/squared_exponentials.py` & `gpflow-2.8.0/gpflow/expectations/squared_exponentials.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/expectations/sums.py` & `gpflow-2.8.0/gpflow/expectations/sums.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/experimental/__init__.py` & `gpflow-2.8.0/gpflow/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/experimental/utils.py` & `gpflow-2.8.0/gpflow/experimental/utils.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/functions.py` & `gpflow-2.8.0/gpflow/functions.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/inducing_variables/__init__.py` & `gpflow-2.8.0/gpflow/inducing_variables/__init__.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/inducing_variables/inducing_patch.py` & `gpflow-2.8.0/gpflow/inducing_variables/inducing_patch.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/inducing_variables/inducing_variables.py` & `gpflow-2.8.0/gpflow/inducing_variables/inducing_variables.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/inducing_variables/multioutput/__init__.py` & `gpflow-2.8.0/gpflow/inducing_variables/multioutput/__init__.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/inducing_variables/multioutput/inducing_variables.py` & `gpflow-2.8.0/gpflow/inducing_variables/multioutput/inducing_variables.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/kernels/__init__.py` & `gpflow-2.8.0/gpflow/kernels/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,15 @@
     "SharedIndependent",
     "SquaredExponential",
     "Static",
     "Stationary",
     "Sum",
     "White",
     "base",
+    "categorical",
     "changepoints",
     "convolutional",
     "linears",
     "misc",
     "multioutput",
     "periodic",
     "statics",
```

### Comparing `gpflow-2.7.1/gpflow/kernels/base.py` & `gpflow-2.8.0/gpflow/kernels/base.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/kernels/changepoints.py` & `gpflow-2.8.0/gpflow/kernels/changepoints.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/kernels/convolutional.py` & `gpflow-2.8.0/gpflow/kernels/convolutional.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/kernels/linears.py` & `gpflow-2.8.0/gpflow/kernels/linears.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/kernels/misc.py` & `gpflow-2.8.0/gpflow/kernels/misc.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/kernels/multioutput/kernels.py` & `gpflow-2.8.0/gpflow/kernels/multioutput/kernels.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/kernels/periodic.py` & `gpflow-2.8.0/gpflow/kernels/periodic.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/kernels/statics.py` & `gpflow-2.8.0/gpflow/kernels/statics.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/kernels/stationaries.py` & `gpflow-2.8.0/gpflow/kernels/stationaries.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/kullback_leiblers.py` & `gpflow-2.8.0/gpflow/kullback_leiblers.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/likelihoods/__init__.py` & `gpflow-2.8.0/gpflow/likelihoods/__init__.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/likelihoods/base.py` & `gpflow-2.8.0/gpflow/likelihoods/base.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/likelihoods/misc.py` & `gpflow-2.8.0/gpflow/likelihoods/misc.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/likelihoods/multiclass.py` & `gpflow-2.8.0/gpflow/likelihoods/multiclass.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/likelihoods/multilatent.py` & `gpflow-2.8.0/gpflow/likelihoods/multilatent.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/likelihoods/scalar_continuous.py` & `gpflow-2.8.0/gpflow/likelihoods/scalar_continuous.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,24 +17,29 @@
 
 import numpy as np
 import tensorflow as tf
 from check_shapes import check_shapes, inherit_check_shapes
 
 from .. import logdensities
 from ..base import MeanAndVariance, TensorType
+from ..config import default_likelihood_positive_minimum
 from ..utilities.parameter_or_function import (
     ConstantOrFunction,
     ParameterOrFunction,
     evaluate_parameter_or_function,
     prepare_parameter_or_function,
 )
 from .base import ScalarLikelihood
 from .utils import inv_probit
 
-DEFAULT_LOWER_BOUND = 1e-6
+
+def _lower_bound(value: Optional[float] = None) -> float:
+    if value is None:
+        return default_likelihood_positive_minimum()
+    return value
 
 
 class Gaussian(ScalarLikelihood):
     r"""
     The Gaussian likelihood is appropriate where uncertainties associated with
     the data are believed to follow a normal distribution, with constant
     variance.
@@ -45,29 +50,29 @@
     """
 
     def __init__(
         self,
         variance: Optional[ConstantOrFunction] = None,
         *,
         scale: Optional[ConstantOrFunction] = None,
-        variance_lower_bound: float = DEFAULT_LOWER_BOUND,
+        variance_lower_bound: Optional[float] = None,
         **kwargs: Any,
     ) -> None:
         """
         :param variance: The noise variance; must be greater than
             ``variance_lower_bound``. This is mutually exclusive with `scale`.
         :param scale: The noise scale; must be greater than
             ``sqrt(variance_lower_bound)``. This is mutually exclusive with `variance`.
         :param variance_lower_bound: The lower (exclusive) bound of ``variance``.
         :param kwargs: Keyword arguments forwarded to :class:`ScalarLikelihood`.
         """
         super().__init__(**kwargs)
 
-        self.variance_lower_bound = variance_lower_bound
-        self.scale_lower_bound = sqrt(variance_lower_bound)
+        self.variance_lower_bound = _lower_bound(variance_lower_bound)
+        self.scale_lower_bound = sqrt(self.variance_lower_bound)
         if scale is None:
             if variance is None:
                 variance = 1.0
             self.variance: Optional[ParameterOrFunction] = prepare_parameter_or_function(
                 variance, lower_bound=self.variance_lower_bound
             )
             self.scale: Optional[ParameterOrFunction] = None
@@ -170,24 +175,24 @@
 
 
 class StudentT(ScalarLikelihood):
     def __init__(
         self,
         scale: ConstantOrFunction = 1.0,
         df: float = 3.0,
-        scale_lower_bound: float = DEFAULT_LOWER_BOUND,
+        scale_lower_bound: Optional[float] = None,
         **kwargs: Any,
     ) -> None:
         """
         :param scale float: scale parameter
         :param df float: degrees of freedom
         """
         super().__init__(**kwargs)
         self.df = df
-        self.scale_lower_bound = scale_lower_bound
+        self.scale_lower_bound = _lower_bound(scale_lower_bound)
         self.scale = prepare_parameter_or_function(scale, lower_bound=self.scale_lower_bound)
 
     @check_shapes(
         "X: [batch..., N, D]",
         "return: [broadcast batch..., broadcast N, broadcast P]",
     )
     def _scale(self, X: TensorType) -> tf.Tensor:
@@ -213,20 +218,20 @@
     Use the transformed GP to give the *scale* (inverse rate) of the Gamma
     """
 
     def __init__(
         self,
         invlink: Callable[[tf.Tensor], tf.Tensor] = tf.exp,
         shape: ConstantOrFunction = 1.0,
-        shape_lower_bound: float = DEFAULT_LOWER_BOUND,
+        shape_lower_bound: Optional[float] = None,
         **kwargs: Any,
     ) -> None:
         super().__init__(**kwargs)
         self.invlink = invlink
-        self.shape_lower_bound = shape_lower_bound
+        self.shape_lower_bound = _lower_bound(shape_lower_bound)
         self.shape = prepare_parameter_or_function(shape, lower_bound=self.shape_lower_bound)
 
     @check_shapes(
         "X: [batch..., N, D]",
         "return: [broadcast batch..., broadcast N, broadcast P]",
     )
     def _shape(self, X: TensorType) -> tf.Tensor:
@@ -279,19 +284,19 @@
         β  = scale * (1-m)
     """
 
     def __init__(
         self,
         invlink: Callable[[tf.Tensor], tf.Tensor] = inv_probit,
         scale: ConstantOrFunction = 1.0,
-        scale_lower_bound: float = DEFAULT_LOWER_BOUND,
+        scale_lower_bound: Optional[float] = None,
         **kwargs: Any,
     ) -> None:
         super().__init__(**kwargs)
-        self.scale_lower_bound = DEFAULT_LOWER_BOUND
+        self.scale_lower_bound = _lower_bound(scale_lower_bound)
         self.scale = prepare_parameter_or_function(scale, lower_bound=self.scale_lower_bound)
         self.invlink = invlink
 
     @check_shapes(
         "X: [batch..., N, D]",
         "return: [broadcast batch..., broadcast N, broadcast P]",
     )
```

### Comparing `gpflow-2.7.1/gpflow/likelihoods/scalar_discrete.py` & `gpflow-2.8.0/gpflow/likelihoods/scalar_discrete.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/likelihoods/utils.py` & `gpflow-2.8.0/gpflow/likelihoods/utils.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/logdensities.py` & `gpflow-2.8.0/gpflow/logdensities.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/mean_functions.py` & `gpflow-2.8.0/gpflow/mean_functions.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/models/__init__.py` & `gpflow-2.8.0/gpflow/models/__init__.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/models/cglb.py` & `gpflow-2.8.0/gpflow/models/cglb.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/models/gplvm.py` & `gpflow-2.8.0/gpflow/models/gplvm.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/models/gpmc.py` & `gpflow-2.8.0/gpflow/models/gpmc.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/models/gpr.py` & `gpflow-2.8.0/gpflow/models/gpr.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/models/model.py` & `gpflow-2.8.0/gpflow/models/model.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/models/sgpmc.py` & `gpflow-2.8.0/gpflow/models/sgpmc.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/models/sgpr.py` & `gpflow-2.8.0/gpflow/models/sgpr.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/models/svgp.py` & `gpflow-2.8.0/gpflow/models/svgp.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/models/training_mixins.py` & `gpflow-2.8.0/gpflow/models/training_mixins.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/models/util.py` & `gpflow-2.8.0/gpflow/models/util.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/models/vgp.py` & `gpflow-2.8.0/gpflow/models/vgp.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/monitor/__init__.py` & `gpflow-2.8.0/gpflow/monitor/__init__.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/monitor/base.py` & `gpflow-2.8.0/gpflow/monitor/base.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/monitor/tensorboard.py` & `gpflow-2.8.0/gpflow/monitor/tensorboard.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/mypy_flags.py` & `gpflow-2.8.0/gpflow/mypy_flags.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/optimizers/mcmc.py` & `gpflow-2.8.0/gpflow/optimizers/mcmc.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/optimizers/natgrad.py` & `gpflow-2.8.0/gpflow/optimizers/natgrad.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/optimizers/scipy.py` & `gpflow-2.8.0/gpflow/optimizers/scipy.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import warnings
-from typing import Any, Callable, Iterable, List, Optional, Sequence, Tuple, Union
+from typing import Any, Callable, Iterable, List, Mapping, Optional, Sequence, Tuple, Union
 
 import numpy as np
 import scipy.optimize
 import tensorflow as tf
 from scipy.optimize import OptimizeResult
 
 from ..base import AnyNDArray
@@ -35,14 +35,15 @@
         self,
         closure: LossClosure,
         variables: Sequence[tf.Variable],
         method: Optional[str] = "L-BFGS-B",
         step_callback: Optional[StepCallback] = None,
         compile: bool = True,
         allow_unused_variables: bool = False,
+        tf_fun_args: Optional[Mapping[str, Any]] = None,
         **scipy_kwargs: Any,
     ) -> OptimizeResult:
         """
         Minimize `closure`.
 
         Minimize is a wrapper around the `scipy.optimize.minimize` function handling the packing and
         unpacking of a list of shaped variables on the TensorFlow side vs. the flat numpy array
@@ -58,35 +59,48 @@
             and `values` is the corresponding list of tensors of matching shape that contains their
             value at this optimisation step.
         :param compile: If True, wraps the evaluation function (the passed `closure` as well as its
             gradient computation) inside a `tf.function()`, which will improve optimization speed in
             most cases.
         :param allow_unused_variables: Whether to allow variables that are not actually used in the
             closure.
+        :param tf_fun_args: Arguments passed through to `tf.function()` when `compile` is True.
+            For example, to enable XLA compilation::
+
+                opt = gpflow.optimizers.Scipy()
+                opt.minimize(..., compile=True, tf_fun_args=dict(jit_compile=True))
         :param scipy_kwargs: Arguments passed through to `scipy.optimize.minimize`.
             Note that Scipy's minimize() takes a `callback` argument, but you probably want to use
             our wrapper and pass in `step_callback`.
         :returns:
             The optimization result represented as a Scipy ``OptimizeResult`` object.
             See the Scipy documentation for description of attributes.
         """
+        if tf_fun_args is None:
+            tf_fun_args = {}
         if not callable(closure):
             raise TypeError(
                 "The 'closure' argument is expected to be a callable object."
             )  # pragma: no cover
         variables = tuple(variables)
         if not all(isinstance(v, tf.Variable) for v in variables):
             raise TypeError(
                 "The 'variables' argument is expected to only contain tf.Variable instances"
                 " (use model.trainable_variables, not model.trainable_parameters)"
             )  # pragma: no cover
+        if not compile and len(tf_fun_args) > 0:
+            raise ValueError("`tf_fun_args` should only be set when `compile` is True")
         initial_params = self.initial_parameters(variables)
 
         func = self.eval_func(
-            closure, variables, compile=compile, allow_unused_variables=allow_unused_variables
+            closure,
+            variables,
+            compile=compile,
+            allow_unused_variables=allow_unused_variables,
+            tf_fun_args=tf_fun_args,
         )
         if step_callback is not None:
             if "callback" in scipy_kwargs:
                 raise ValueError("Callback passed both via `step_callback` and `callback`")
 
             callback = self.callback_func(variables, step_callback)
             scipy_kwargs.update(dict(callback=callback))
@@ -103,14 +117,15 @@
         return cls.pack_tensors(variables)
 
     @classmethod
     def eval_func(
         cls,
         closure: LossClosure,
         variables: Sequence[tf.Variable],
+        tf_fun_args: Mapping[str, Any],
         compile: bool = True,
         allow_unused_variables: bool = False,
     ) -> Callable[[AnyNDArray], Tuple[AnyNDArray, AnyNDArray]]:
         first_call = True
 
         def _tf_eval(x: tf.Tensor) -> Tuple[tf.Tensor, tf.Tensor]:
             nonlocal first_call
@@ -129,15 +144,15 @@
                 loss, grads = _compute_loss_and_gradients(
                     closure, variables, tf.UnconnectedGradients.ZERO
                 )
 
             return loss, cls.pack_tensors(grads)
 
         if compile:
-            _tf_eval = tf.function(_tf_eval)
+            _tf_eval = tf.function(_tf_eval, **tf_fun_args)
 
         def _eval(x: AnyNDArray) -> Tuple[AnyNDArray, AnyNDArray]:
             loss, grad = _tf_eval(tf.convert_to_tensor(x))
             return loss.numpy().astype(np.float64), grad.numpy().astype(np.float64)
 
         return _eval
```

### Comparing `gpflow-2.7.1/gpflow/posteriors.py` & `gpflow-2.8.0/gpflow/posteriors.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/probability_distributions.py` & `gpflow-2.8.0/gpflow/probability_distributions.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/quadrature/base.py` & `gpflow-2.8.0/gpflow/quadrature/base.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/quadrature/deprecated.py` & `gpflow-2.8.0/gpflow/quadrature/deprecated.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/quadrature/gauss_hermite.py` & `gpflow-2.8.0/gpflow/quadrature/gauss_hermite.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/type_flags.py` & `gpflow-2.8.0/gpflow/type_flags.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/utilities/__init__.py` & `gpflow-2.8.0/gpflow/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/utilities/bijectors.py` & `gpflow-2.8.0/gpflow/utilities/bijectors.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/utilities/misc.py` & `gpflow-2.8.0/gpflow/utilities/misc.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/utilities/model_utils.py` & `gpflow-2.8.0/gpflow/utilities/model_utils.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/utilities/multipledispatch.py` & `gpflow-2.8.0/gpflow/utilities/multipledispatch.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/utilities/ops.py` & `gpflow-2.8.0/gpflow/utilities/ops.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/utilities/parameter_or_function.py` & `gpflow-2.8.0/gpflow/utilities/parameter_or_function.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow/utilities/traversal.py` & `gpflow-2.8.0/gpflow/utilities/traversal.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/gpflow.egg-info/PKG-INFO` & `gpflow-2.8.0/gpflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpflow
-Version: 2.7.1
+Version: 2.8.0
 Summary: Gaussian process methods in TensorFlow
 Home-page: https://www.gpflow.org
 Author: James Hensman, Alex Matthews
 Author-email: james.hensman@gmail.com
 License: Apache License 2.0
 Project-URL: Source on GitHub, https://github.com/GPflow/GPflow
 Project-URL: Documentation, https://gpflow.github.io/GPflow/
```

### Comparing `gpflow-2.7.1/gpflow.egg-info/SOURCES.txt` & `gpflow-2.8.0/gpflow.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -82,14 +82,15 @@
 gpflow/inducing_variables/__init__.py
 gpflow/inducing_variables/inducing_patch.py
 gpflow/inducing_variables/inducing_variables.py
 gpflow/inducing_variables/multioutput/__init__.py
 gpflow/inducing_variables/multioutput/inducing_variables.py
 gpflow/kernels/__init__.py
 gpflow/kernels/base.py
+gpflow/kernels/categorical.py
 gpflow/kernels/changepoints.py
 gpflow/kernels/convolutional.py
 gpflow/kernels/linears.py
 gpflow/kernels/misc.py
 gpflow/kernels/periodic.py
 gpflow/kernels/statics.py
 gpflow/kernels/stationaries.py
```

### Comparing `gpflow-2.7.1/setup.py` & `gpflow-2.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/conditionals/test_broadcasted_conditionals.py` & `gpflow-2.8.0/tests/gpflow/conditionals/test_broadcasted_conditionals.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/conditionals/test_conditionals.py` & `gpflow-2.8.0/tests/gpflow/conditionals/test_conditionals.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/conditionals/test_multioutput.py` & `gpflow-2.8.0/tests/gpflow/conditionals/test_multioutput.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/conditionals/test_uncertain_conditional.py` & `gpflow-2.8.0/tests/gpflow/conditionals/test_uncertain_conditional.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/conditionals/test_util.py` & `gpflow-2.8.0/tests/gpflow/conditionals/test_util.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/config/test_config.py` & `gpflow-2.8.0/tests/gpflow/config/test_config.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,50 +9,66 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
-from typing import Any, Callable
+from typing import Any, Callable, Iterable
 from unittest import mock
 
 import numpy as np
 import pytest
 import tensorflow as tf
 
 import gpflow
 from gpflow.base import TensorData
 from gpflow.config import (
+    config,
     default_float,
     default_int,
     default_jitter,
+    default_likelihood_positive_minimum,
     default_positive_bijector,
+    default_positive_minimum,
     default_summary_fmt,
+    set_config,
     set_default_float,
     set_default_int,
     set_default_jitter,
+    set_default_likelihood_positive_minimum,
     set_default_positive_bijector,
+    set_default_positive_minimum,
     set_default_summary_fmt,
 )
 from gpflow.utilities import to_default_float, to_default_int
 
 _env_values = [
     ("int", "int16", np.int16),
     ("int", "int64", np.int64),
     ("float", "float16", np.float16),
     ("float", "float32", np.float32),
     ("positive_bijector", "exp", "exp"),
     ("positive_bijector", "softplus", "softplus"),
     ("summary_fmt", "simple", "simple"),
     ("positive_minimum", "1e-3", 1e-3),
+    ("likelihood_positive_minimum", "5e-4", 5e-4),
     ("jitter", "1e-2", 1e-2),
 ]
 
 
+# Fixture to reset config back to default. Some tests change global config and can otherwise
+# effect subsequent tests.
+@pytest.fixture(autouse=True)
+def reset_config() -> Iterable[None]:
+    default_config = config()
+    yield
+    set_config(default_config)
+
+
 @pytest.mark.parametrize("attr_name, value, expected_value", _env_values)
 def test_env_variables(attr_name: str, value: str, expected_value: Any) -> None:
     env_name = f"GPFLOW_{attr_name.upper()}"
     with mock.patch.dict("os.environ", {env_name: value}):
         assert os.environ[env_name] == value
         config = gpflow.config.Config()
         assert getattr(config, attr_name) == expected_value
@@ -99,26 +115,43 @@
     ],
 )
 def test_dtype_errorcheck(setter: Callable[[type], None], invalid_type: Any) -> None:
     with pytest.raises(TypeError):
         setter(invalid_type)
 
 
-def test_jitter_setting() -> None:
-    set_default_jitter(1e-3)
-    assert default_jitter() == 1e-3
-    set_default_jitter(1e-6)
-    assert default_jitter() == 1e-6
+@pytest.mark.parametrize(
+    "setter, getter",
+    [
+        (set_default_jitter, default_jitter),
+        (set_default_likelihood_positive_minimum, default_likelihood_positive_minimum),
+        (set_default_positive_minimum, default_positive_minimum),
+    ],
+)
+@pytest.mark.parametrize("value", [1e-3, 1e-6])
+def test_floats_setting(
+    setter: Callable[[float], None], getter: Callable[[], float], value: float
+) -> None:
+    setter(value)
+    assert getter() == value
 
 
-def test_jitter_errorcheck() -> None:
+@pytest.mark.parametrize(
+    "setter",
+    [
+        set_default_jitter,
+        set_default_likelihood_positive_minimum,
+        set_default_positive_minimum,
+    ],
+)
+def test_floats_errorcheck(setter: Callable[[float], None]) -> None:
     with pytest.raises(TypeError):
-        set_default_jitter("not a float")  # type: ignore[arg-type]
+        setter("not a float")  # type: ignore[arg-type]
     with pytest.raises(ValueError):
-        set_default_jitter(-1e-10)
+        setter(-1e-10)
 
 
 @pytest.mark.parametrize(
     "value, error_msg",
     [
         ("Unknown", r"`unknown` not in set of valid bijectors: \['exp', 'softplus'\]"),
         (1.0, r"`1.0` not in set of valid bijectors: \['exp', 'softplus'\]"),
```

### Comparing `gpflow-2.7.1/tests/gpflow/conftest.py` & `gpflow-2.8.0/tests/gpflow/conftest.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/covariances/test_base_covariances.py` & `gpflow-2.8.0/tests/gpflow/covariances/test_base_covariances.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/covariances/test_multioutput.py` & `gpflow-2.8.0/tests/gpflow/covariances/test_multioutput.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/expectations/test_expectations.py` & `gpflow-2.8.0/tests/gpflow/expectations/test_expectations.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/experimental/test_utils.py` & `gpflow-2.8.0/tests/gpflow/experimental/test_utils.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/kernels/reference.py` & `gpflow-2.8.0/tests/gpflow/kernels/reference.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/kernels/test_broadcasting.py` & `gpflow-2.8.0/tests/gpflow/kernels/test_broadcasting.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from check_shapes import check_shapes
 from numpy.testing import assert_allclose
 
 import gpflow
 import gpflow.ci_utils
 from gpflow import kernels
 from gpflow.base import AnyNDArray, TensorType
+from gpflow.kernels.categorical import Categorical
 
 
 def create_kernels() -> Sequence[kernels.Kernel]:
     result: List[kernels.Kernel] = [
         # Static kernels:
         kernels.White(),
         kernels.Constant(),
@@ -57,14 +58,19 @@
         kernels.ArcCosine(),
         kernels.Coregion(output_dim=5, rank=2),
         kernels.Convolutional(kernels.Matern32(), [4, 4], [2, 2]),
         # multioutput:
         kernels.SharedIndependent(kernels.Matern32(), output_dim=5),
         kernels.SeparateIndependent([kernels.Matern32() for _ in range(5)]),
         kernels.LinearCoregionalization([kernels.Matern32() for _ in range(3)], np.ones((5, 3))),
+        Categorical(
+            non_categorical_kernel=kernels.RBF(lengthscales=0.1),
+            categorical_kernel=kernels.RBF(lengthscales=0.1),
+            num_labels=3,
+        ),
     ]
     return result
 
 
 def make_id(value: Any) -> str:
     if isinstance(value, tuple):
         return f"[{','.join(repr(x) for x in value)}]"
```

### Comparing `gpflow-2.7.1/tests/gpflow/kernels/test_coregion.py` & `gpflow-2.8.0/tests/gpflow/kernels/test_coregion.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/kernels/test_kernels.py` & `gpflow-2.8.0/tests/gpflow/kernels/test_kernels.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     RationalQuadratic,
     SeparateIndependent,
     SharedIndependent,
     SquaredExponential,
     Stationary,
     White,
 )
+from gpflow.kernels.categorical import _concat_inputs_with_latents
 from tests.gpflow.kernels.reference import ref_arccosine_kernel, ref_periodic_kernel, ref_rbf_kernel
 
 rng = np.random.RandomState(1)
 
 
 @check_shapes(
     "X: [N, D]",
@@ -666,7 +667,82 @@
     kernel = k1 + k2
     X = np.random.randn(N, D)
     K1 = k1(X, full_cov=True)
     K2 = k2(X, full_cov=True)
     K = kernel(X, full_cov=True)
     assert K.shape == [N, P, N, P]
     np.testing.assert_allclose(K, K1 + K2)
+
+
+def test_concat_inputs_with_latents() -> None:
+    X = tf.constant(
+        [
+            [0.11333948, 0.0],
+            [0.68914756, 0.0],
+            [0.49686943, 0.0],
+            [0.93093605, 0.0],
+            [0.49400229, 0.0],
+            [0.2563728, 0.0],
+            [0.60688866, 0.0],
+            [0.26627661, 0.0],
+            [0.17639742, 0.0],
+            [0.12579375, 0.0],
+            [0.94793767, 1.0],
+            [0.57164863, 1.0],
+            [0.05673398, 1.0],
+            [0.27555594, 1.0],
+            [0.89225699, 1.0],
+            [0.73987146, 1.0],
+            [0.06209851, 1.0],
+            [0.91578623, 1.0],
+            [0.38951871, 1.0],
+            [0.25707253, 1.0],
+            [0.92527423, 2.0],
+            [0.12519213, 2.0],
+            [0.27104576, 2.0],
+            [0.24123346, 2.0],
+            [0.77848324, 2.0],
+            [0.45188542, 2.0],
+            [0.12848926, 2.0],
+            [0.67861482, 2.0],
+            [0.43295772, 2.0],
+            [0.26668177, 2.0],
+        ],
+        dtype=tf.float64,
+    )
+    Z = tf.constant([[0.0], [0.5], [1.0]], dtype=tf.float64)
+    result = tf.constant(
+        [
+            [0.11333948, 0.0],
+            [0.68914756, 0.0],
+            [0.49686943, 0.0],
+            [0.93093605, 0.0],
+            [0.49400229, 0.0],
+            [0.2563728, 0.0],
+            [0.60688866, 0.0],
+            [0.26627661, 0.0],
+            [0.17639742, 0.0],
+            [0.12579375, 0.0],
+            [0.94793767, 0.5],
+            [0.57164863, 0.5],
+            [0.05673398, 0.5],
+            [0.27555594, 0.5],
+            [0.89225699, 0.5],
+            [0.73987146, 0.5],
+            [0.06209851, 0.5],
+            [0.91578623, 0.5],
+            [0.38951871, 0.5],
+            [0.25707253, 0.5],
+            [0.92527423, 1.0],
+            [0.12519213, 1.0],
+            [0.27104576, 1.0],
+            [0.24123346, 1.0],
+            [0.77848324, 1.0],
+            [0.45188542, 1.0],
+            [0.12848926, 1.0],
+            [0.67861482, 1.0],
+            [0.43295772, 1.0],
+            [0.26668177, 1.0],
+        ],
+        dtype=tf.float64,
+    )
+    assert np.all(_concat_inputs_with_latents(Z, X) == result)
```

### Comparing `gpflow-2.7.1/tests/gpflow/kernels/test_positive_semidefinite.py` & `gpflow-2.8.0/tests/gpflow/kernels/test_positive_semidefinite.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/kernels/test_scaled_euclid_dist.py` & `gpflow-2.8.0/tests/gpflow/kernels/test_scaled_euclid_dist.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/likelihoods/test_function_params.py` & `gpflow-2.8.0/tests/gpflow/likelihoods/test_function_params.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/likelihoods/test_heteroskedastic.py` & `gpflow-2.8.0/tests/gpflow/likelihoods/test_heteroskedastic.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/likelihoods/test_heteroskedastic_constant_variance.py` & `gpflow-2.8.0/tests/gpflow/likelihoods/test_heteroskedastic_constant_variance.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/likelihoods/test_likelihoods.py` & `gpflow-2.8.0/tests/gpflow/likelihoods/test_likelihoods.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/likelihoods/test_multiclass.py` & `gpflow-2.8.0/tests/gpflow/likelihoods/test_multiclass.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/likelihoods/test_switched_likelihood.py` & `gpflow-2.8.0/tests/gpflow/likelihoods/test_switched_likelihood.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/models/test_cglb.py` & `gpflow-2.8.0/tests/gpflow/models/test_cglb.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/models/test_gplvm.py` & `gpflow-2.8.0/tests/gpflow/models/test_gplvm.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/models/test_gpr.py` & `gpflow-2.8.0/tests/gpflow/models/test_gpr.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/models/test_gpr_posterior.py` & `gpflow-2.8.0/tests/gpflow/models/test_gpr_posterior.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/models/test_mcmc.py` & `gpflow-2.8.0/tests/gpflow/models/test_mcmc.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/models/test_methods.py` & `gpflow-2.8.0/tests/gpflow/models/test_methods.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/models/test_model_predict.py` & `gpflow-2.8.0/tests/gpflow/models/test_model_predict.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/models/test_sgpr.py` & `gpflow-2.8.0/tests/gpflow/models/test_sgpr.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/models/test_sgpr_posterior.py` & `gpflow-2.8.0/tests/gpflow/models/test_sgpr_posterior.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/models/test_svgp.py` & `gpflow-2.8.0/tests/gpflow/models/test_svgp.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/models/test_svgp_posterior.py` & `gpflow-2.8.0/tests/gpflow/models/test_svgp_posterior.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/models/test_training_mixins.py` & `gpflow-2.8.0/tests/gpflow/models/test_training_mixins.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/models/test_variational.py` & `gpflow-2.8.0/tests/gpflow/models/test_variational.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/models/test_vgp.py` & `gpflow-2.8.0/tests/gpflow/models/test_vgp.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/models/test_vgp_posterior.py` & `gpflow-2.8.0/tests/gpflow/models/test_vgp_posterior.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/optimizers/test_mcmc.py` & `gpflow-2.8.0/tests/gpflow/optimizers/test_mcmc.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/optimizers/test_natural_gradient.py` & `gpflow-2.8.0/tests/gpflow/optimizers/test_natural_gradient.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/optimizers/test_scipy.py` & `gpflow-2.8.0/tests/integration/test_dynamic_shapes.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,146 +8,181 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import warnings
-
 import numpy as np
 import pytest
 import tensorflow as tf
+from check_shapes import ShapeChecker
 
 import gpflow
 from gpflow.base import AnyNDArray
 from gpflow.config import default_float
-from gpflow.models import GPR, GPModel
 
 rng = np.random.RandomState(0)
 
 
 class Datum:
-    X: AnyNDArray = rng.rand(20, 1) * 10
-    Y = np.sin(X) + 0.9 * np.cos(X * 1.6) + rng.randn(*X.shape) * 0.8
-    Y = np.tile(Y, 2)  # two identical columns
-    Xtest: AnyNDArray = rng.rand(10, 1) * 10
+    cs = ShapeChecker().check_shape
+
+    n_inputs = 1
+    n_outputs = 2
+    n_outputs_c = 1
+
+    X: AnyNDArray = cs(rng.rand(20, n_inputs) * 10, "[N, n_inputs]")
+    Y = cs(np.sin(X) + 0.9 * np.cos(X * 1.6) + rng.randn(*X.shape) * 0.8, "[N, n_outputs_c]")
+    Y = cs(np.tile(Y, n_outputs), "[N, n_outputs]")  # identical columns
+    Xtest: AnyNDArray = cs(rng.rand(10, n_inputs) * 10, "[N_new, n_inputs]")
     data = (X, Y)
 
+    # for classification:
+    Yc = cs(Y[:, :n_outputs_c], "[N, n_outputs_c]")
+    cdata = (X, Yc)
 
-def _create_full_gp_model() -> GPModel:
-    """
-    GP Regression
-    """
-    return GPR(
-        (Datum.X, Datum.Y),
-        kernel=gpflow.kernels.SquaredExponential(),
-        mean_function=gpflow.mean_functions.Constant(),
+
+def test_vgp() -> None:
+    X = tf.Variable(
+        tf.zeros((1, Datum.n_inputs), dtype=default_float()), shape=(None, None), trainable=False
+    )
+    Y = tf.Variable(
+        tf.zeros((1, Datum.n_outputs), dtype=default_float()), shape=(None, None), trainable=False
     )
 
+    model = gpflow.models.VGP(
+        (X, Y),
+        gpflow.kernels.SquaredExponential(),
+        gpflow.likelihoods.Gaussian(),
+        num_latent_gps=Datum.n_outputs,
+    )
+
+    @tf.function
+    def model_closure() -> tf.Tensor:
+        return -model.elbo()
+
+    model_closure()  # Trigger compilation.
+
+    gpflow.models.vgp.update_vgp_data(model, (Datum.X, Datum.Y))
+    opt = gpflow.optimizers.Scipy()
 
-def test_scipy_jit() -> None:
-    m1 = _create_full_gp_model()
-    m2 = _create_full_gp_model()
-
-    opt1 = gpflow.optimizers.Scipy()
-    opt2 = gpflow.optimizers.Scipy()
-
-    opt1.minimize(
-        m1.training_loss,
-        variables=m1.trainable_variables,
-        options=dict(maxiter=50),
-        compile=False,
-    )
-    opt2.minimize(
-        m2.training_loss,
-        variables=m2.trainable_variables,
-        options=dict(maxiter=50),
+    # simply test whether it runs without erroring...:
+    opt.minimize(
+        model_closure,
+        variables=model.trainable_variables,
+        options=dict(maxiter=3),
         compile=True,
     )
 
-    def get_values(model: GPModel) -> AnyNDArray:
-        return np.array([var.numpy().squeeze() for var in model.trainable_variables])
 
-    np.testing.assert_allclose(get_values(m1), get_values(m2), rtol=1e-13, atol=1e-13)
+@pytest.mark.parametrize("whiten", [True, False])
+@pytest.mark.parametrize("q_diag", [True, False])
+def test_svgp(whiten: bool, q_diag: bool) -> None:
+    model = gpflow.models.SVGP(
+        gpflow.kernels.SquaredExponential(),
+        gpflow.likelihoods.Gaussian(),
+        inducing_variable=Datum.X.copy(),
+        q_diag=q_diag,
+        whiten=whiten,
+        mean_function=gpflow.mean_functions.Constant(),
+        num_latent_gps=Datum.n_outputs,
+    )
+    gpflow.set_trainable(model.inducing_variable, False)
+
+    # test with explicitly unknown shapes:
+    tensor_spec = tf.TensorSpec(shape=None, dtype=default_float())
 
+    # lambda because: https://github.com/GPflow/GPflow/issues/1929
+    elbo_lambda = lambda data: model.elbo(data)
+
+    elbo = tf.function(
+        elbo_lambda,
+        input_signature=[(tensor_spec, tensor_spec)],
+    )
 
-@pytest.mark.parametrize("compile", [True, False])
-def test_scipy__optimal(compile: bool) -> None:
-    target1 = [0.2, 0.8]
-    target2 = [0.6]
-    v1 = tf.Variable([0.5, 0.5], dtype=default_float())
-    v2 = tf.Variable([0.5], dtype=default_float())
-    compilation_count = 0
-
-    def f() -> tf.Tensor:
-        nonlocal compilation_count
-        compilation_count += 1
-        return tf.reduce_sum((target1 - v1) ** 2) + tf.reduce_sum((target2 - v2) ** 2)
+    @tf.function
+    def model_closure() -> tf.Tensor:
+        return -elbo(Datum.data)
+
+    model_closure()  # Trigger compilation.
 
     opt = gpflow.optimizers.Scipy()
-    result = opt.minimize(f, [v1, v2], compile=compile)
 
-    if compile:
-        assert 1 == compilation_count
-    else:
-        assert 1 < compilation_count
-    assert result.success
-    np.testing.assert_allclose(target1 + target2, result.x)
-    np.testing.assert_allclose(target1, v1)
-    np.testing.assert_allclose(target2, v2)
-
-
-@pytest.mark.parametrize("compile", [True, False])
-def test_scipy__partially_disconnected_variable(compile: bool) -> None:
-    target1 = 0.2
-    target2 = 0.6
-    v1 = tf.Variable([0.5, 0.5], dtype=default_float())
-    v2 = tf.Variable(0.5, dtype=default_float())
-
-    def f() -> tf.Tensor:
-        # v1[1] not used.
-        v10 = v1[0]
-        return (target1 - v10) ** 2 + (target2 - v2) ** 2
+    # simply test whether it runs without erroring...:
+    opt.minimize(
+        model_closure,
+        variables=model.trainable_variables,
+        options=dict(maxiter=3),
+        compile=True,
+    )
+
 
+def test_vgp_multiclass() -> None:
+    X = tf.Variable(
+        tf.zeros((1, Datum.n_inputs), dtype=default_float()), shape=(None, None), trainable=False
+    )
+    Yc = tf.Variable(
+        tf.zeros((1, Datum.n_outputs_c), dtype=default_float()), shape=(None, None), trainable=False
+    )
+
+    num_classes = 3
+    model = gpflow.models.VGP(
+        (X, Yc),
+        gpflow.kernels.SquaredExponential(),
+        gpflow.likelihoods.MultiClass(num_classes=num_classes),
+        num_latent_gps=num_classes,
+    )
+
+    @tf.function
+    def model_closure() -> tf.Tensor:
+        return -model.elbo()
+
+    model_closure()  # Trigger compilation.
+
+    gpflow.models.vgp.update_vgp_data(model, (Datum.X, Datum.Yc))
     opt = gpflow.optimizers.Scipy()
-    result = opt.minimize(f, [v1, v2], compile=compile)
 
-    assert result.success
-    np.testing.assert_allclose([target1, 0.5, target2], result.x)
-    np.testing.assert_allclose([target1, 0.5], v1)
-    np.testing.assert_allclose(target2, v2)
-
-
-@pytest.mark.parametrize("compile", [True, False])
-@pytest.mark.parametrize("allow_unused_variables", [True, False])
-def test_scipy__disconnected_variable(compile: bool, allow_unused_variables: bool) -> None:
-    target1 = [0.2, 0.8]
-    v1 = tf.Variable([0.5, 0.5], dtype=default_float(), name="v1")
-    v2 = tf.Variable([0.5], dtype=default_float(), name="v2")
-
-    def f() -> tf.Tensor:
-        # v2 not used.
-        return tf.reduce_sum((target1 - v1) ** 2)
+    # simply test whether it runs without erroring...:
+    opt.minimize(
+        model_closure,
+        variables=model.trainable_variables,
+        options=dict(maxiter=3),
+        compile=True,
+    )
+
+
+def test_svgp_multiclass() -> None:
+    num_classes = 3
+    model = gpflow.models.SVGP(
+        gpflow.kernels.SquaredExponential(),
+        gpflow.likelihoods.MultiClass(num_classes=num_classes),
+        inducing_variable=Datum.X.copy(),
+        num_latent_gps=num_classes,
+    )
+    gpflow.set_trainable(model.inducing_variable, False)
+
+    # lambda because: https://github.com/GPflow/GPflow/issues/1929
+    elbo_lambda = lambda data: model.elbo(data)
+
+    # test with explicitly unknown shapes:
+    tensor_spec = tf.TensorSpec(shape=None, dtype=default_float())
+    elbo = tf.function(
+        elbo_lambda,
+        input_signature=[(tensor_spec, tensor_spec)],
+    )
+
+    @tf.function
+    def model_closure() -> tf.Tensor:
+        return -elbo(Datum.cdata)
+
+    model_closure()  # Trigger compilation.
 
     opt = gpflow.optimizers.Scipy()
 
-    if allow_unused_variables:
-        with warnings.catch_warnings(record=True) as w:
-            warnings.simplefilter("always")
-            result = opt.minimize(
-                f, [v1, v2], compile=compile, allow_unused_variables=allow_unused_variables
-            )
-
-        (warning,) = w
-        message = warning.message
-        assert isinstance(message, Warning)
-        msg = message.args[0]
-        assert v2.name in msg
-
-        assert result.success
-        np.testing.assert_allclose(target1 + [0.5], result.x)
-        np.testing.assert_allclose(target1, v1)
-        np.testing.assert_allclose([0.5], v2)
-    else:
-        with pytest.raises(ValueError, match=v2.name):
-            opt.minimize(f, [v1, v2], allow_unused_variables=allow_unused_variables)
+    # simply test whether it runs without erroring...:
+    opt.minimize(
+        model_closure,
+        variables=model.trainable_variables,
+        options=dict(maxiter=3),
+        compile=True,
+    )
```

### Comparing `gpflow-2.7.1/tests/gpflow/posteriors/conftest.py` & `gpflow-2.8.0/tests/gpflow/posteriors/conftest.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/posteriors/test_bo_integration.py` & `gpflow-2.8.0/tests/gpflow/posteriors/test_bo_integration.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/posteriors/test_posteriors.py` & `gpflow-2.8.0/tests/gpflow/posteriors/test_posteriors.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/test_all.py` & `gpflow-2.8.0/tests/gpflow/test_all.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/test_base.py` & `gpflow-2.8.0/tests/gpflow/test_base.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/test_base_prior.py` & `gpflow-2.8.0/tests/gpflow/test_base_prior.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/test_base_training.py` & `gpflow-2.8.0/tests/gpflow/test_base_training.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/test_functions.py` & `gpflow-2.8.0/tests/gpflow/test_functions.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/test_inducing_variables.py` & `gpflow-2.8.0/tests/gpflow/test_inducing_variables.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/test_initial_value.py` & `gpflow-2.8.0/tests/gpflow/test_initial_value.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/test_kullback_leiblers.py` & `gpflow-2.8.0/tests/gpflow/test_kullback_leiblers.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/test_logdensities.py` & `gpflow-2.8.0/tests/gpflow/test_logdensities.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/test_monitor.py` & `gpflow-2.8.0/tests/gpflow/test_monitor.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/utilities/test_bijectors.py` & `gpflow-2.8.0/tests/gpflow/utilities/test_bijectors.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/utilities/test_deepcopy.py` & `gpflow-2.8.0/tests/gpflow/utilities/test_deepcopy.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/utilities/test_misc.py` & `gpflow-2.8.0/tests/gpflow/utilities/test_misc.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/utilities/test_model_utils.py` & `gpflow-2.8.0/tests/gpflow/utilities/test_model_utils.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/utilities/test_multipledispatch.py` & `gpflow-2.8.0/tests/gpflow/utilities/test_multipledispatch.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/utilities/test_ops.py` & `gpflow-2.8.0/tests/gpflow/utilities/test_ops.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/utilities/test_parameter_or_function.py` & `gpflow-2.8.0/tests/gpflow/utilities/test_parameter_or_function.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/utilities/test_set_trainable.py` & `gpflow-2.8.0/tests/gpflow/utilities/test_set_trainable.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/utilities/test_training_loop.py` & `gpflow-2.8.0/tests/gpflow/utilities/test_training_loop.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/utilities/test_traversal.py` & `gpflow-2.8.0/tests/gpflow/utilities/test_traversal.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/gpflow/utilities/test_utilities.py` & `gpflow-2.8.0/tests/gpflow/utilities/test_utilities.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/integration/test_benchmark.py` & `gpflow-2.8.0/tests/integration/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/integration/test_docs.py` & `gpflow-2.8.0/tests/integration/test_docs.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/integration/test_linear_noise.py` & `gpflow-2.8.0/tests/integration/test_linear_noise.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/integration/test_method_equivalence.py` & `gpflow-2.8.0/tests/integration/test_method_equivalence.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/integration/test_model_serialization.py` & `gpflow-2.8.0/tests/integration/test_model_serialization.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.7.1/tests/integration/test_notebooks.py` & `gpflow-2.8.0/tests/integration/test_notebooks.py`

 * *Files identical despite different names*

