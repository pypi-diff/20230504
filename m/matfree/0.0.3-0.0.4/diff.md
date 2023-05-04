# Comparing `tmp/matfree-0.0.3.tar.gz` & `tmp/matfree-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matfree-0.0.3.tar", last modified: Mon May  1 07:51:31 2023, max compression
+gzip compressed data, was "matfree-0.0.4.tar", last modified: Thu May  4 12:44:31 2023, max compression
```

## Comparing `matfree-0.0.3.tar` & `matfree-0.0.4.tar`

### file list

```diff
@@ -1,64 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:51:31.367911 matfree-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:51:31.355911 matfree-0.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:51:31.355911 matfree-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-01 07:51:11.000000 matfree-0.0.3/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-01 07:51:11.000000 matfree-0.0.3/.github/workflows/doc-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-01 07:51:11.000000 matfree-0.0.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-01 07:51:11.000000 matfree-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-01 07:51:11.000000 matfree-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-01 07:51:11.000000 matfree-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-01 07:51:11.000000 matfree-0.0.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-05-01 07:51:31.367911 matfree-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-05-01 07:51:11.000000 matfree-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:51:31.355911 matfree-0.0.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:51:31.359911 matfree-0.0.3/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-01 07:51:11.000000 matfree-0.0.3/docs/api/decomp.md
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-01 07:51:11.000000 matfree-0.0.3/docs/api/hutch.md
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-01 07:51:11.000000 matfree-0.0.3/docs/api/montecarlo.md
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-01 07:51:11.000000 matfree-0.0.3/docs/api/slq.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:51:31.359911 matfree-0.0.3/docs/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-05-01 07:51:11.000000 matfree-0.0.3/docs/benchmarks/control_variates.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-01 07:51:11.000000 matfree-0.0.3/docs/benchmarks/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:51:31.359911 matfree-0.0.3/docs/dev/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-01 07:51:11.000000 matfree-0.0.3/docs/dev/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-05-01 07:51:11.000000 matfree-0.0.3/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:51:31.359911 matfree-0.0.3/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-01 07:51:11.000000 matfree-0.0.3/docs/javascripts/mathjax.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:51:31.359911 matfree-0.0.3/matfree/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-01 07:51:11.000000 matfree-0.0.3/matfree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-01 07:51:31.000000 matfree-0.0.3/matfree/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:51:31.363911 matfree-0.0.3/matfree/backend/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-01 07:51:11.000000 matfree-0.0.3/matfree/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-01 07:51:11.000000 matfree-0.0.3/matfree/backend/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-01 07:51:11.000000 matfree-0.0.3/matfree/backend/control_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-01 07:51:11.000000 matfree-0.0.3/matfree/backend/func.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-01 07:51:11.000000 matfree-0.0.3/matfree/backend/linalg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-05-01 07:51:11.000000 matfree-0.0.3/matfree/backend/np.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-01 07:51:11.000000 matfree-0.0.3/matfree/backend/plt.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-01 07:51:11.000000 matfree-0.0.3/matfree/backend/prng.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-01 07:51:11.000000 matfree-0.0.3/matfree/backend/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-01 07:51:11.000000 matfree-0.0.3/matfree/backend/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-01 07:51:11.000000 matfree-0.0.3/matfree/backend/time.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-01 07:51:11.000000 matfree-0.0.3/matfree/backend/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-05-01 07:51:11.000000 matfree-0.0.3/matfree/decomp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-05-01 07:51:11.000000 matfree-0.0.3/matfree/hutch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-05-01 07:51:11.000000 matfree-0.0.3/matfree/montecarlo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-05-01 07:51:11.000000 matfree-0.0.3/matfree/slq.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-01 07:51:11.000000 matfree-0.0.3/matfree/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:51:31.363911 matfree-0.0.3/matfree.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-05-01 07:51:31.000000 matfree-0.0.3/matfree.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-01 07:51:31.000000 matfree-0.0.3/matfree.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 07:51:31.000000 matfree-0.0.3/matfree.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-01 07:51:31.000000 matfree-0.0.3/matfree.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-01 07:51:31.000000 matfree-0.0.3/matfree.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-01 07:51:11.000000 matfree-0.0.3/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-01 07:51:11.000000 matfree-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-01 07:51:31.367911 matfree-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-01 07:51:11.000000 matfree-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:51:31.367911 matfree-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-01 07:51:11.000000 matfree-0.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-01 07:51:11.000000 matfree-0.0.3/tests/test_autodiff.py
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-05-01 07:51:11.000000 matfree-0.0.3/tests/test_decomp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-05-01 07:51:11.000000 matfree-0.0.3/tests/test_hutch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-01 07:51:11.000000 matfree-0.0.3/tests/test_montecarlo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-01 07:51:11.000000 matfree-0.0.3/tests/test_slq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:44:31.929407 matfree-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:44:31.913407 matfree-0.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:44:31.917407 matfree-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-04 12:44:14.000000 matfree-0.0.4/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-04 12:44:14.000000 matfree-0.0.4/.github/workflows/doc-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-04 12:44:14.000000 matfree-0.0.4/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-04 12:44:14.000000 matfree-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-04 12:44:14.000000 matfree-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-04 12:44:14.000000 matfree-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-04 12:44:14.000000 matfree-0.0.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-05-04 12:44:31.929407 matfree-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-05-04 12:44:14.000000 matfree-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:44:31.917407 matfree-0.0.4/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:44:31.917407 matfree-0.0.4/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-04 12:44:14.000000 matfree-0.0.4/docs/api/decomp.md
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-04 12:44:14.000000 matfree-0.0.4/docs/api/hutch.md
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-04 12:44:14.000000 matfree-0.0.4/docs/api/montecarlo.md
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-04 12:44:14.000000 matfree-0.0.4/docs/api/slq.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:44:31.917407 matfree-0.0.4/docs/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-05-04 12:44:14.000000 matfree-0.0.4/docs/benchmarks/control_variates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-04 12:44:14.000000 matfree-0.0.4/docs/benchmarks/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-05-04 12:44:14.000000 matfree-0.0.4/docs/benchmarks/jacobian_squared.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:44:31.917407 matfree-0.0.4/docs/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-04 12:44:14.000000 matfree-0.0.4/docs/dev/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-05-04 12:44:14.000000 matfree-0.0.4/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:44:31.917407 matfree-0.0.4/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-04 12:44:14.000000 matfree-0.0.4/docs/javascripts/mathjax.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:44:31.921407 matfree-0.0.4/matfree/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-04 12:44:14.000000 matfree-0.0.4/matfree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-04 12:44:31.000000 matfree-0.0.4/matfree/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:44:31.925407 matfree-0.0.4/matfree/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-04 12:44:14.000000 matfree-0.0.4/matfree/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-04 12:44:14.000000 matfree-0.0.4/matfree/backend/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-04 12:44:14.000000 matfree-0.0.4/matfree/backend/control_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-04 12:44:14.000000 matfree-0.0.4/matfree/backend/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-04 12:44:14.000000 matfree-0.0.4/matfree/backend/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-05-04 12:44:14.000000 matfree-0.0.4/matfree/backend/np.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-04 12:44:14.000000 matfree-0.0.4/matfree/backend/plt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-04 12:44:14.000000 matfree-0.0.4/matfree/backend/prng.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-04 12:44:14.000000 matfree-0.0.4/matfree/backend/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-04 12:44:14.000000 matfree-0.0.4/matfree/backend/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-04 12:44:14.000000 matfree-0.0.4/matfree/backend/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-04 12:44:14.000000 matfree-0.0.4/matfree/backend/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-04 12:44:14.000000 matfree-0.0.4/matfree/benchmark_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7291 2023-05-04 12:44:14.000000 matfree-0.0.4/matfree/decomp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-05-04 12:44:14.000000 matfree-0.0.4/matfree/hutch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-05-04 12:44:14.000000 matfree-0.0.4/matfree/montecarlo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-04 12:44:14.000000 matfree-0.0.4/matfree/slq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-04 12:44:14.000000 matfree-0.0.4/matfree/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:44:31.921407 matfree-0.0.4/matfree.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-05-04 12:44:31.000000 matfree-0.0.4/matfree.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-05-04 12:44:31.000000 matfree-0.0.4/matfree.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 12:44:31.000000 matfree-0.0.4/matfree.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-04 12:44:31.000000 matfree-0.0.4/matfree.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-04 12:44:31.000000 matfree-0.0.4/matfree.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-04 12:44:14.000000 matfree-0.0.4/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-04 12:44:14.000000 matfree-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-04 12:44:31.929407 matfree-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-04 12:44:14.000000 matfree-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:44:31.925407 matfree-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-04 12:44:14.000000 matfree-0.0.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:44:31.925407 matfree-0.0.4/tests/test_decomp/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-04 12:44:14.000000 matfree-0.0.4/tests/test_decomp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-05-04 12:44:14.000000 matfree-0.0.4/tests/test_decomp/test_gkl_bidiagonal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-05-04 12:44:14.000000 matfree-0.0.4/tests/test_decomp/test_lanczos_tridiagonal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-04 12:44:14.000000 matfree-0.0.4/tests/test_decomp/test_svd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:44:31.925407 matfree-0.0.4/tests/test_hutch/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-04 12:44:14.000000 matfree-0.0.4/tests/test_hutch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-04 12:44:14.000000 matfree-0.0.4/tests/test_hutch/test_diagonal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-04 12:44:14.000000 matfree-0.0.4/tests/test_hutch/test_frobeniusnorm_squared.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-04 12:44:14.000000 matfree-0.0.4/tests/test_hutch/test_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-05-04 12:44:14.000000 matfree-0.0.4/tests/test_hutch/test_trace_and_diagonal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:44:31.925407 matfree-0.0.4/tests/test_montecarlo/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-04 12:44:14.000000 matfree-0.0.4/tests/test_montecarlo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-04 12:44:14.000000 matfree-0.0.4/tests/test_montecarlo/test_estimate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-04 12:44:14.000000 matfree-0.0.4/tests/test_montecarlo/test_van_der_corput.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:44:31.929407 matfree-0.0.4/tests/test_slq/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-04 12:44:14.000000 matfree-0.0.4/tests/test_slq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-04 12:44:14.000000 matfree-0.0.4/tests/test_slq/test_logdet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-04 12:44:14.000000 matfree-0.0.4/tests/test_slq/test_logdet_autodiff.py
```

### Comparing `matfree-0.0.3/.github/workflows/ci.yaml` & `matfree-0.0.4/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `matfree-0.0.3/.github/workflows/doc-publish.yml` & `matfree-0.0.4/.github/workflows/doc-publish.yml`

 * *Files identical despite different names*

### Comparing `matfree-0.0.3/.github/workflows/release.yml` & `matfree-0.0.4/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `matfree-0.0.3/.gitignore` & `matfree-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `matfree-0.0.3/.pre-commit-config.yaml` & `matfree-0.0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `matfree-0.0.3/LICENSE` & `matfree-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `matfree-0.0.3/PKG-INFO` & `matfree-0.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matfree
-Version: 0.0.3
+Version: 0.0.4
 Summary: Matrix-free numerical linear algebra including trace-estimation.
 Author: Nicholas Krämer
 Author-email: pekra@dtu.dk
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: cpu
@@ -54,48 +54,48 @@
 
 Estimate traces as such:
 ```python
 >>> sample_fun = montecarlo.normal(shape=(2,))
 >>> matvec = lambda x: a.T @ (a @ x)
 >>> trace = hutch.trace(matvec, key=key, sample_fun=sample_fun)
 >>> print(jnp.round(trace))
-515.0
+514.0
 >>> # for comparison:
 >>> print(jnp.round(jnp.trace(a.T @ a)))
 506.0
 
 ```
 The number of keys determines the number of sequential batches.
 Many small batches reduces memory.
 Few large batches increases memory and runtime.
 
 Determine the number of samples per batch as follows.
 
 ```python
 >>> trace = hutch.trace(matvec, key=key, sample_fun=sample_fun, num_batches=10)
 >>> print(jnp.round(trace))
-507.0
+508.0
 >>> # for comparison:
 >>> print(jnp.round(jnp.trace(a.T @ a)))
 506.0
 
 ```
 
 ### Traces and diagonals
 
 Jointly estimating traces and diagonals improves performance.
 Here is how to use it:
 
 ```python
 >>> trace, diagonal = hutch.trace_and_diagonal(matvec, key=key, num_levels=10_000, sample_fun=sample_fun)
 >>> print(jnp.round(trace))
-507.0
+497.0
 
 >>> print(jnp.round(diagonal))
-[221. 287.]
+[216. 281.]
 
 >>> # for comparison:
 >>> print(jnp.round(jnp.trace(a.T @ a)))
 506.0
 
 >>> print(jnp.round(jnp.diagonal(a.T @ a)))
 [220. 286.]
@@ -107,22 +107,22 @@
 `trace_and_diagonal` implements a multilevel diagonal-estimation scheme:
 ```python
 >>> _, diagonal_1 = hutch.trace_and_diagonal(matvec, key=key, num_levels=10_000, sample_fun=sample_fun)
 >>> init = jnp.zeros(shape=(2,), dtype=float)
 >>> diagonal_2 = hutch.diagonal_multilevel(matvec, init, key=key, num_levels=10_000, sample_fun=sample_fun)
 
 >>> print(jnp.round(diagonal_1, 4))
-[220.54979 286.7476 ]
+[215.7592 281.245 ]
 
 >>> print(jnp.round(diagonal_2, 4))
-[220.54979 286.7476 ]
+[215.7592 281.245 ]
 
 >>> diagonal = hutch.diagonal_multilevel(matvec, init, key=key, num_levels=10, num_samples_per_batch=1000, num_batches_per_level=10, sample_fun=sample_fun)
 >>> print(jnp.round(diagonal))
-[219. 285.]
+[220. 286.]
 
 ```
 
 Does the multilevel scheme help? That is not always clear; but [here](https://github.com/pnkraemer/matfree/blob/main/docs/benchmarks/control_variates.py) is a benchmark.
 
 ### Determinants
```

### Comparing `matfree-0.0.3/README.md` & `matfree-0.0.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -37,48 +37,48 @@
 
 Estimate traces as such:
 ```python
 >>> sample_fun = montecarlo.normal(shape=(2,))
 >>> matvec = lambda x: a.T @ (a @ x)
 >>> trace = hutch.trace(matvec, key=key, sample_fun=sample_fun)
 >>> print(jnp.round(trace))
-515.0
+514.0
 >>> # for comparison:
 >>> print(jnp.round(jnp.trace(a.T @ a)))
 506.0
 
 ```
 The number of keys determines the number of sequential batches.
 Many small batches reduces memory.
 Few large batches increases memory and runtime.
 
 Determine the number of samples per batch as follows.
 
 ```python
 >>> trace = hutch.trace(matvec, key=key, sample_fun=sample_fun, num_batches=10)
 >>> print(jnp.round(trace))
-507.0
+508.0
 >>> # for comparison:
 >>> print(jnp.round(jnp.trace(a.T @ a)))
 506.0
 
 ```
 
 ### Traces and diagonals
 
 Jointly estimating traces and diagonals improves performance.
 Here is how to use it:
 
 ```python
 >>> trace, diagonal = hutch.trace_and_diagonal(matvec, key=key, num_levels=10_000, sample_fun=sample_fun)
 >>> print(jnp.round(trace))
-507.0
+497.0
 
 >>> print(jnp.round(diagonal))
-[221. 287.]
+[216. 281.]
 
 >>> # for comparison:
 >>> print(jnp.round(jnp.trace(a.T @ a)))
 506.0
 
 >>> print(jnp.round(jnp.diagonal(a.T @ a)))
 [220. 286.]
@@ -90,22 +90,22 @@
 `trace_and_diagonal` implements a multilevel diagonal-estimation scheme:
 ```python
 >>> _, diagonal_1 = hutch.trace_and_diagonal(matvec, key=key, num_levels=10_000, sample_fun=sample_fun)
 >>> init = jnp.zeros(shape=(2,), dtype=float)
 >>> diagonal_2 = hutch.diagonal_multilevel(matvec, init, key=key, num_levels=10_000, sample_fun=sample_fun)
 
 >>> print(jnp.round(diagonal_1, 4))
-[220.54979 286.7476 ]
+[215.7592 281.245 ]
 
 >>> print(jnp.round(diagonal_2, 4))
-[220.54979 286.7476 ]
+[215.7592 281.245 ]
 
 >>> diagonal = hutch.diagonal_multilevel(matvec, init, key=key, num_levels=10, num_samples_per_batch=1000, num_batches_per_level=10, sample_fun=sample_fun)
 >>> print(jnp.round(diagonal))
-[219. 285.]
+[220. 286.]
 
 ```
 
 Does the multilevel scheme help? That is not always clear; but [here](https://github.com/pnkraemer/matfree/blob/main/docs/benchmarks/control_variates.py) is a benchmark.
 
 ### Determinants
```

### Comparing `matfree-0.0.3/docs/benchmarks/control_variates.py` & `matfree-0.0.4/docs/benchmarks/control_variates.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,14 @@
 """Control_variates benchmark.
 
 Runtime: ~10 seconds.
 """
 
-from matfree import hutch, montecarlo
-from matfree.backend import func, linalg, np, plt, prng, progressbar, time
-
-
-def rmse_relative(received, *, expected):
-    """Compute the relative root-mean-square error."""
-    return linalg.vector_norm((received - expected) / expected) / np.sqrt(expected.size)
-
-
-def error_and_time(fun, error_fun):
-    """Compute error and runtime of a function with a single outputs."""
-
-    def fun_wrapped(*args, **kwargs):
-        # Execute once for compilation
-        _ = fun(*args, **kwargs)
-
-        # Execute and time
-        t0 = time.perf_counter()
-        result = fun(*args, **kwargs)
-        result.block_until_ready()
-        t1 = time.perf_counter()
-        return error_fun(result), (t1 - t0)
-
-    return fun_wrapped
+from matfree import benchmark_util, hutch, montecarlo
+from matfree.backend import func, linalg, np, plt, prng, progressbar
 
 
 def problem(n):
     """Create an example problem."""
 
     # This function has a Jacobian with x-shaped sparsity pattern
     # We expect control variates to do pretty well
@@ -52,25 +30,25 @@
 if __name__ == "__main__":
     dim = 100
     num_samples = 2 ** np.arange(4, 10)
     num_restarts = 5
 
     (Av, trace, J), (k, sample_fun) = problem(dim)
 
-    error_fun = func.partial(rmse_relative, expected=trace)
+    error_fun = func.partial(benchmark_util.rmse_relative, expected=trace)
 
-    @func.partial(error_and_time, error_fun=error_fun)
+    @func.partial(benchmark_util.error_and_time, error_fun=error_fun)
     @func.partial(func.jit, static_argnums=0)
     def fun1(num, key):
         """Estimate the trace conventionally."""
         return hutch.trace(
             Av, key=key, sample_fun=sample_fun, num_batches=num, num_samples_per_batch=1
         )
 
-    @func.partial(error_and_time, error_fun=error_fun)
+    @func.partial(benchmark_util.error_and_time, error_fun=error_fun)
     @func.partial(func.jit, static_argnums=0)
     def fun2(num, key):
         """Estimate trace and diagonal jointly and discard the diagonal."""
         trace2, _ = hutch.trace_and_diagonal(
             Av, key=key, num_levels=num, sample_fun=sample_fun
         )
         return trace2
```

### Comparing `matfree-0.0.3/docs/index.md` & `matfree-0.0.4/docs/index.md`

 * *Files 3% similar despite different names*

```diff
@@ -37,48 +37,48 @@
 
 Estimate traces as such:
 ```python
 >>> sample_fun = montecarlo.normal(shape=(2,))
 >>> matvec = lambda x: a.T @ (a @ x)
 >>> trace = hutch.trace(matvec, key=key, sample_fun=sample_fun)
 >>> print(jnp.round(trace))
-515.0
+514.0
 >>> # for comparison:
 >>> print(jnp.round(jnp.trace(a.T @ a)))
 506.0
 
 ```
 The number of keys determines the number of sequential batches.
 Many small batches reduces memory.
 Few large batches increases memory and runtime.
 
 Determine the number of samples per batch as follows.
 
 ```python
 >>> trace = hutch.trace(matvec, key=key, sample_fun=sample_fun, num_batches=10)
 >>> print(jnp.round(trace))
-507.0
+508.0
 >>> # for comparison:
 >>> print(jnp.round(jnp.trace(a.T @ a)))
 506.0
 
 ```
 
 ### Traces and diagonals
 
 Jointly estimating traces and diagonals improves performance.
 Here is how to use it:
 
 ```python
 >>> trace, diagonal = hutch.trace_and_diagonal(matvec, key=key, num_levels=10_000, sample_fun=sample_fun)
 >>> print(jnp.round(trace))
-507.0
+497.0
 
 >>> print(jnp.round(diagonal))
-[221. 287.]
+[216. 281.]
 
 >>> # for comparison:
 >>> print(jnp.round(jnp.trace(a.T @ a)))
 506.0
 
 >>> print(jnp.round(jnp.diagonal(a.T @ a)))
 [220. 286.]
@@ -90,22 +90,22 @@
 `trace_and_diagonal` implements a multilevel diagonal-estimation scheme:
 ```python
 >>> _, diagonal_1 = hutch.trace_and_diagonal(matvec, key=key, num_levels=10_000, sample_fun=sample_fun)
 >>> init = jnp.zeros(shape=(2,), dtype=float)
 >>> diagonal_2 = hutch.diagonal_multilevel(matvec, init, key=key, num_levels=10_000, sample_fun=sample_fun)
 
 >>> print(jnp.round(diagonal_1, 4))
-[220.54979 286.7476 ]
+[215.7592 281.245 ]
 
 >>> print(jnp.round(diagonal_2, 4))
-[220.54979 286.7476 ]
+[215.7592 281.245 ]
 
 >>> diagonal = hutch.diagonal_multilevel(matvec, init, key=key, num_levels=10, num_samples_per_batch=1000, num_batches_per_level=10, sample_fun=sample_fun)
 >>> print(jnp.round(diagonal))
-[219. 285.]
+[220. 286.]
 
 ```
 
 Does the multilevel scheme help? That is not always clear; but [here](https://github.com/pnkraemer/matfree/blob/main/docs/benchmarks/control_variates.py) is a benchmark.
 
 ### Determinants
```

### Comparing `matfree-0.0.3/matfree/backend/control_flow.py` & `matfree-0.0.4/matfree/backend/control_flow.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,7 +18,11 @@
 
 def fori_loop(lower, upper, body_fun, init_val):
     return jax.lax.fori_loop(lower, upper, body_fun, init_val)
 
 
 def while_loop(cond_fun, body_fun, init_val):
     return jax.lax.while_loop(cond_fun, body_fun, init_val)
+
+
+def map(fun, /, xs):  # noqa: A001
+    return jax.lax.map(fun, xs)
```

### Comparing `matfree-0.0.3/matfree/backend/func.py` & `matfree-0.0.4/matfree/backend/func.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,14 +19,18 @@
 # Partial and the like
 
 
 def partial(func, /, *args, **kwargs):
     return functools.partial(func, *args, **kwargs)
 
 
+def wraps(func, /):
+    return functools.wraps(func)
+
+
 # Algorithmic differentiation
 
 
 def linearize(func, /, *args):
     return jax.linearize(func, *args)
```

### Comparing `matfree-0.0.3/matfree/backend/linalg.py` & `matfree-0.0.4/matfree/backend/linalg.py`

 * *Files 11% similar despite different names*

```diff
@@ -35,7 +35,11 @@
 def diagonal_matrix(x, /, offset=0):  # not part of array API
     """Construct a diagonal matrix."""
     return jnp.diag(x, offset)
 
 
 def trace(x, /):
     return jnp.trace(x)
+
+
+def svd(A, /, *, full_matrices=True):
+    return jnp.linalg.svd(A, full_matrices=full_matrices)
```

### Comparing `matfree-0.0.3/matfree/backend/np.py` & `matfree-0.0.4/matfree/backend/np.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,14 +34,18 @@
     return jnp.ones_like(x)
 
 
 def zeros(shape, *, dtype=None):
     return jnp.zeros(shape, dtype=dtype)
 
 
+def ones(shape, *, dtype=None):
+    return jnp.ones(shape, dtype=dtype)
+
+
 # Element-wise functions
 
 
 def abs(x, /):  # noqa: A001
     return jnp.abs(x)
 
 
@@ -61,14 +65,18 @@
     return jnp.cos(x)
 
 
 def sqrt(x, /):
     return jnp.sqrt(x)
 
 
+def sign(x, /):
+    return jnp.sign(x)
+
+
 # Utility functions
 
 
 def any(x, /):  # noqa: A001
     return jnp.any(x)
 
 
@@ -87,15 +95,20 @@
     return jnp.std(x, axis)
 
 
 def sum(x, /, axis=None):  # noqa: A001
     return jnp.sum(x, axis)
 
 
-def maximum(x1, x2):  # todo: call max()
+# todo: change amax and maximum to array_max, elementwise_max
+def amin(x, /):
+    return jnp.amin(x)
+
+
+def maximum(x1, x2):  # todo: call this max()
     return jnp.maximum(x1, x2)
 
 
 def nanmean(x, /, axis=None):
     return jnp.nanmean(x, axis)
 
 
@@ -133,7 +146,14 @@
 
 
 # Functional implementation of constants
 
 
 def nan():
     return jnp.nan
+
+
+# Others
+
+
+def convolve(a, b, /, mode="full"):
+    return jnp.convolve(a, b, mode=mode)
```

### Comparing `matfree-0.0.3/matfree/backend/prng.py` & `matfree-0.0.4/matfree/backend/prng.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.3/matfree/hutch.py` & `matfree-0.0.4/matfree/hutch.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.3/matfree/montecarlo.py` & `matfree-0.0.4/matfree/montecarlo.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """Monte-Carlo estimation."""
 
 from matfree.backend import containers, control_flow, func, np, prng
-from matfree.backend.typing import Any, Array, Callable
+from matfree.backend.typing import Array, Callable
 
 
 def estimate(
     fun: Callable,
     /,
     *,
     key: Array,
     sample_fun: Callable,
     num_batches: int = 1,
     num_samples_per_batch: int = 10_000,
+    target_fun=np.nanmean,
 ) -> Array:
     """Monte-Carlo estimation: Compute the expected value of a function.
 
     Parameters
     ----------
     fun:
         Function whose expected value shall be estimated.
@@ -26,18 +27,23 @@
         For trace-estimation, use
         either [montecarlo.normal(...)][matfree.montecarlo.normal]
         or [montecarlo.rademacher(...)][matfree.montecarlo.normal].
     num_batches:
         Number of batches when computing arithmetic means.
     num_samples_per_batch:
         Number of samples per batch.
+    target_fun:
+        The target function to compute. Usually, this is np.mean. But any other
+        statistical function with a signature like
+        [those](https://data-apis.org/array-api/2022.12/API_specification/statistical_functions.html)
+        would work. The default is np.nanmean.
     """
     fun_mc = _montecarlo(fun, sample_fun=sample_fun)
-    fun_single_batch = _mean_vmap(fun_mc, num_samples_per_batch)
-    fun_batched = _mean_loop(fun_single_batch, num_batches)
+    fun_single_batch = _stats_via_vmap(fun_mc, num_samples_per_batch, target_fun)
+    fun_batched = _stats_via_map(fun_single_batch, num_batches, target_fun)
     return fun_batched(key)
 
 
 def _montecarlo(f, /, *, sample_fun):
     """Turn a function into a Monte-Carlo problem.
 
     More specifically, f(x) becomes g(key) = f(h(key)),
@@ -49,64 +55,36 @@
     def f_mc(key, /):
         sample = sample_fun(key)
         return f(sample)
 
     return f_mc
 
 
-def _mean_vmap(f, num, /):
-    """Compute a batch-mean via jax.vmap."""
+def _stats_via_vmap(f, num, /, target_fun):
+    """Compute summary statistics via jax.vmap."""
 
     def f_mean(key, /):
         subkeys = prng.split(key, num)
         fx_values = func.vmap(f)(subkeys)
-        return np.nanmean(fx_values, axis=0)
+        return target_fun(fx_values, axis=0)
 
     return f_mean
 
 
-class _MState(containers.NamedTuple):
-    mean: Any
-    key: Any
-
-
-def _mean_loop(f, num, /):
-    """Compute an on-the-fly mean via a for-loop."""
+def _stats_via_map(f, num, /, target_fun):
+    """Compute summary statistics via jax.lax.map."""
 
     def f_mean(key, /):
-        # Initialise
-        fx_shape = func.eval_shape(f, key).shape
-        mean = np.zeros(fx_shape, dtype=float)
-        mstate = _MState(mean=mean, key=key)
-
-        # Run for-loop
-        increment = func.partial(_mean_increment, fun=f)
-        mstate = control_flow.fori_loop(0, num, body_fun=increment, init_val=mstate)
-        mean, _key = mstate  # todo: why not return key?
-
-        # Return results
-        return mean
+        subkeys = prng.split(key, num)
+        fx_values = control_flow.map(f, subkeys)
+        return target_fun(fx_values, axis=0)
 
     return f_mean
 
 
-def _mean_increment(i, mstate: _MState, fun) -> _MState:
-    """Increment the current mean-estimate."""
-    # Read and split key
-    mean, key = mstate
-    _, subkey = prng.split(key)
-
-    # Evaluate function
-    fx_values = fun(subkey)
-
-    # Update mean estimate
-    mean_new = np.sum(np.asarray([mean * i, fx_values]), axis=0) / (i + 1)
-    return _MState(mean=mean_new, key=subkey)
-
-
 def normal(*, shape, dtype=float):
     """Construct a function that samples from a standard normal distribution."""
 
     def fun(key):
         return prng.normal(key, shape=shape, dtype=dtype)
 
     return fun
```

### Comparing `matfree-0.0.3/matfree/slq.py` & `matfree-0.0.4/matfree/slq.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 """Stochastic Lanczos quadrature."""
 
 from matfree import decomp, montecarlo
 from matfree.backend import func, linalg, np
 
 
 def logdet(*args, **kwargs):
-    """Estimate the log-determinant of a matrix."""
-    return trace_of_matfun(np.log, *args, **kwargs)
+    """Estimate the log-determinant of a symmetric, positive definite matrix."""
+    return trace_of_matfun_symmetric(np.log, *args, **kwargs)
 
 
 # todo: nuclear norm, schatten-p norms.
 #  But for this we should use bi-diagonalisation
 
 
-def trace_of_matfun(matfun, Av, order, /, **kwargs):
-    """Compute the trace of the function of a matrix."""
-    quadratic_form = quadratic_form_slq(matfun, Av, order)
+def trace_of_matfun_symmetric(matfun, Av, order, /, **kwargs):
+    """Compute the trace of the function of a symmetric matrix."""
+    quadratic_form = quadratic_form_slq_symmetric(matfun, Av, order)
     return montecarlo.estimate(quadratic_form, **kwargs)
 
 
-def quadratic_form_slq(matfun, Av, order, /):
+def quadratic_form_slq_symmetric(matfun, Av, order, /):
     """Approximate quadratic form for stochastic Lanczos quadrature."""
 
     def quadform(v0, /):
-        algorithm = decomp.lanczos(order)
-        _, tridiag = decomp.decompose_fori_loop(0, order + 1, Av, v0, alg=algorithm)
+        algorithm = decomp.lanczos_tridiagonal(order)
+        _, tridiag = decomp.decompose_fori_loop(0, order + 1, v0, Av, alg=algorithm)
         (diag, off_diag) = tridiag
 
         # todo: once jax supports eigh_tridiagonal(eigvals_only=False),
         #  use it here. Until then: an eigen-decomposition of size (order + 1)
         #  does not hurt too much...
         diag = linalg.diagonal_matrix(diag)
         offdiag1 = linalg.diagonal_matrix(off_diag, -1)
```

### Comparing `matfree-0.0.3/matfree/test_util.py` & `matfree-0.0.4/matfree/test_util.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Test utilities."""
 
 from matfree.backend import linalg, np
 
 
-def generate_symmetric_matrix_from_eigvals(eigvals, /):
+def symmetric_matrix_from_eigenvalues(eigvals, /):
     """Generate a symmetric matrix with prescribed eigenvalues."""
     (n,) = eigvals.shape
 
     # Need _some_ matrix to start with
     A = np.reshape(np.arange(1.0, n**2 + 1.0), (n, n))
     A = A / linalg.matrix_norm(A)
     X = A.T @ A + np.eye(n)
@@ -16,7 +16,15 @@
     # Treat Q as a stack of eigenvectors.
     Q, R = linalg.qr(X)
 
     # Treat Q as eigenvectors, and 'D' as eigenvalues.
     # return Q D Q.T.
     # This matrix will be dense, symmetric, and have a given spectrum.
     return Q @ (eigvals[:, None] * Q.T)
+
+
+def asymmetric_matrix_from_singular_values(vals, /, nrows, ncols):
+    """Generate an asymmetric matrix with specific singular values."""
+    A = np.reshape(np.arange(1.0, nrows * ncols + 1.0), (nrows, ncols))
+    A /= nrows * ncols
+    U, S, Vt = linalg.svd(A, full_matrices=False)
+    return U @ linalg.diagonal(vals) @ Vt
```

### Comparing `matfree-0.0.3/matfree.egg-info/PKG-INFO` & `matfree-0.0.4/matfree.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matfree
-Version: 0.0.3
+Version: 0.0.4
 Summary: Matrix-free numerical linear algebra including trace-estimation.
 Author: Nicholas Krämer
 Author-email: pekra@dtu.dk
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: cpu
@@ -54,48 +54,48 @@
 
 Estimate traces as such:
 ```python
 >>> sample_fun = montecarlo.normal(shape=(2,))
 >>> matvec = lambda x: a.T @ (a @ x)
 >>> trace = hutch.trace(matvec, key=key, sample_fun=sample_fun)
 >>> print(jnp.round(trace))
-515.0
+514.0
 >>> # for comparison:
 >>> print(jnp.round(jnp.trace(a.T @ a)))
 506.0
 
 ```
 The number of keys determines the number of sequential batches.
 Many small batches reduces memory.
 Few large batches increases memory and runtime.
 
 Determine the number of samples per batch as follows.
 
 ```python
 >>> trace = hutch.trace(matvec, key=key, sample_fun=sample_fun, num_batches=10)
 >>> print(jnp.round(trace))
-507.0
+508.0
 >>> # for comparison:
 >>> print(jnp.round(jnp.trace(a.T @ a)))
 506.0
 
 ```
 
 ### Traces and diagonals
 
 Jointly estimating traces and diagonals improves performance.
 Here is how to use it:
 
 ```python
 >>> trace, diagonal = hutch.trace_and_diagonal(matvec, key=key, num_levels=10_000, sample_fun=sample_fun)
 >>> print(jnp.round(trace))
-507.0
+497.0
 
 >>> print(jnp.round(diagonal))
-[221. 287.]
+[216. 281.]
 
 >>> # for comparison:
 >>> print(jnp.round(jnp.trace(a.T @ a)))
 506.0
 
 >>> print(jnp.round(jnp.diagonal(a.T @ a)))
 [220. 286.]
@@ -107,22 +107,22 @@
 `trace_and_diagonal` implements a multilevel diagonal-estimation scheme:
 ```python
 >>> _, diagonal_1 = hutch.trace_and_diagonal(matvec, key=key, num_levels=10_000, sample_fun=sample_fun)
 >>> init = jnp.zeros(shape=(2,), dtype=float)
 >>> diagonal_2 = hutch.diagonal_multilevel(matvec, init, key=key, num_levels=10_000, sample_fun=sample_fun)
 
 >>> print(jnp.round(diagonal_1, 4))
-[220.54979 286.7476 ]
+[215.7592 281.245 ]
 
 >>> print(jnp.round(diagonal_2, 4))
-[220.54979 286.7476 ]
+[215.7592 281.245 ]
 
 >>> diagonal = hutch.diagonal_multilevel(matvec, init, key=key, num_levels=10, num_samples_per_batch=1000, num_batches_per_level=10, sample_fun=sample_fun)
 >>> print(jnp.round(diagonal))
-[219. 285.]
+[220. 286.]
 
 ```
 
 Does the multilevel scheme help? That is not always clear; but [here](https://github.com/pnkraemer/matfree/blob/main/docs/benchmarks/control_variates.py) is a benchmark.
 
 ### Determinants
```

### Comparing `matfree-0.0.3/matfree.egg-info/SOURCES.txt` & `matfree-0.0.4/matfree.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -13,18 +13,20 @@
 docs/index.md
 docs/api/decomp.md
 docs/api/hutch.md
 docs/api/montecarlo.md
 docs/api/slq.md
 docs/benchmarks/control_variates.py
 docs/benchmarks/index.md
+docs/benchmarks/jacobian_squared.py
 docs/dev/index.md
 docs/javascripts/mathjax.js
 matfree/__init__.py
 matfree/_version.py
+matfree/benchmark_util.py
 matfree/decomp.py
 matfree/hutch.py
 matfree/montecarlo.py
 matfree/slq.py
 matfree/test_util.py
 matfree.egg-info/PKG-INFO
 matfree.egg-info/SOURCES.txt
@@ -40,12 +42,22 @@
 matfree/backend/plt.py
 matfree/backend/prng.py
 matfree/backend/progressbar.py
 matfree/backend/testing.py
 matfree/backend/time.py
 matfree/backend/typing.py
 tests/__init__.py
-tests/test_autodiff.py
-tests/test_decomp.py
-tests/test_hutch.py
-tests/test_montecarlo.py
-tests/test_slq.py
+tests/test_decomp/__init__.py
+tests/test_decomp/test_gkl_bidiagonal.py
+tests/test_decomp/test_lanczos_tridiagonal.py
+tests/test_decomp/test_svd.py
+tests/test_hutch/__init__.py
+tests/test_hutch/test_diagonal.py
+tests/test_hutch/test_frobeniusnorm_squared.py
+tests/test_hutch/test_trace.py
+tests/test_hutch/test_trace_and_diagonal.py
+tests/test_montecarlo/__init__.py
+tests/test_montecarlo/test_estimate.py
+tests/test_montecarlo/test_van_der_corput.py
+tests/test_slq/__init__.py
+tests/test_slq/test_logdet.py
+tests/test_slq/test_logdet_autodiff.py
```

### Comparing `matfree-0.0.3/mkdocs.yml` & `matfree-0.0.4/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `matfree-0.0.3/pyproject.toml` & `matfree-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `matfree-0.0.3/setup.cfg` & `matfree-0.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `matfree-0.0.3/tests/test_autodiff.py` & `matfree-0.0.4/tests/test_slq/test_logdet_autodiff.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 @testing.fixture()
 def A(n, num_significant_eigvals):
     """Make a positive definite matrix with certain spectrum."""
     # 'Invent' a spectrum. Use the number of pre-defined eigenvalues.
     d = np.arange(n) + 10.0
     d = d.at[num_significant_eigvals:].set(0.001)
 
-    return test_util.generate_symmetric_matrix_from_eigvals(d)
+    return test_util.symmetric_matrix_from_eigenvalues(d)
 
 
 @testing.parametrize("n", [200])
 @testing.parametrize("num_significant_eigvals", [30])
 @testing.parametrize("order", [10])
 # usually: ~1.5 * num_significant_eigvals.
 # But logdet seems to converge sooo much faster.
-def test_logdet(A, order):
+def test_check_grads(A, order):
     """Assert that log-determinant computation admits valid VJPs and JVPs."""
     key = prng.prng_key(1)
 
     def fun(s):
         return _logdet(s, order, key)
 
     testing.check_grads(fun, (A,), order=1, atol=1e-1, rtol=1e-1)
```

### Comparing `matfree-0.0.3/tests/test_decomp.py` & `matfree-0.0.4/tests/test_decomp/test_lanczos_tridiagonal.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,43 +7,43 @@
 @testing.fixture()
 def A(n, num_significant_eigvals):
     """Make a positive definite matrix with certain spectrum."""
     # 'Invent' a spectrum. Use the number of pre-defined eigenvalues.
     d = np.arange(n) + 10.0
     d = d.at[num_significant_eigvals:].set(0.001)
 
-    return test_util.generate_symmetric_matrix_from_eigvals(d)
+    return test_util.symmetric_matrix_from_eigenvalues(d)
 
 
 @testing.parametrize("n", [6])
 @testing.parametrize("num_significant_eigvals", [4])
-def test_tridiagonal_error_for_too_high_order(A):
+def test_error_for_too_high_order(A):
     """Assert graceful failure if the depth matches or exceeds the number of columns."""
     n, _ = np.shape(A)
     key = prng.prng_key(1)
     v0 = prng.normal(key, shape=(n,))
     with testing.raises(ValueError):
-        alg = decomp.lanczos(n + 10)
-        _ = decomp.decompose_fori_loop(0, n + 10, lambda v: A @ v, v0, alg=alg)
+        alg = decomp.lanczos_tridiagonal(n + 10)
+        _ = decomp.decompose_fori_loop(0, n + 10, v0, lambda v: A @ v, alg=alg)
     with testing.raises(ValueError):
-        alg = decomp.lanczos(n)
-        _ = decomp.decompose_fori_loop(0, n + 1, lambda v: A @ v, v0, alg=alg)
+        alg = decomp.lanczos_tridiagonal(n)
+        _ = decomp.decompose_fori_loop(0, n + 1, v0, lambda v: A @ v, alg=alg)
 
 
 @testing.parametrize("n", [6])
 @testing.parametrize("num_significant_eigvals", [6])
-def test_tridiagonal_max_order(A):
+def test_max_order(A):
     """If m == n, the matrix should be equal to the full tridiagonal."""
     n, _ = np.shape(A)
     order = n - 1
     key = prng.prng_key(1)
     v0 = prng.normal(key, shape=(n,))
-    alg = decomp.lanczos(order)
+    alg = decomp.lanczos_tridiagonal(order)
     Q, (d_m, e_m) = decomp.decompose_fori_loop(
-        0, order + 1, lambda v: A @ v, v0, alg=alg
+        0, order + 1, v0, lambda v: A @ v, alg=alg
     )
 
     # Lanczos is not stable.
     tols_decomp = {"atol": 1e-5, "rtol": 1e-5}
 
     # Since full-order mode: Q must be unitary
     assert np.shape(Q) == (order + 1, n)
@@ -71,21 +71,21 @@
     # should always pass.
     assert np.allclose(Q.T @ T @ Q, A, **tols_decomp)
 
 
 @testing.parametrize("n", [50])
 @testing.parametrize("num_significant_eigvals", [4])
 @testing.parametrize("order", [6])  # ~1.5 * num_significant_eigvals
-def test_tridiagonal(A, order):
+def test_identity(A, order):
     """Test that Lanczos tridiagonalisation yields an orthogonal-tridiagonal decomp."""
     n, _ = np.shape(A)
     key = prng.prng_key(1)
     v0 = prng.normal(key, shape=(n,))
-    alg = decomp.lanczos(order)
-    Q, tridiag = decomp.decompose_fori_loop(0, order + 1, lambda v: A @ v, v0, alg=alg)
+    alg = decomp.lanczos_tridiagonal(order)
+    Q, tridiag = decomp.decompose_fori_loop(0, order + 1, v0, lambda v: A @ v, alg=alg)
     (d_m, e_m) = tridiag
 
     # Lanczos is not stable.
     tols_decomp = {"atol": 1e-5, "rtol": 1e-5}
 
     assert np.shape(Q) == (order + 1, n)
     assert np.allclose(Q @ Q.T, np.eye(order + 1), **tols_decomp), Q @ Q.T
@@ -96,15 +96,15 @@
     assert np.shape(T) == (order + 1, order + 1)
 
     # Fail early if the (off)diagonals don't coincide
     assert np.allclose(linalg.diagonal(QAQt), d_m, **tols_decomp)
     assert np.allclose(linalg.diagonal(QAQt, 1), e_m, **tols_decomp)
     assert np.allclose(linalg.diagonal(QAQt, -1), e_m, **tols_decomp)
 
-    # Test the full decompoisition
+    # Test the full decomposition
     assert np.allclose(QAQt, T, **tols_decomp)
 
 
 def _sym_tridiagonal_dense(d, e):
     diag = linalg.diagonal_matrix(d)
     offdiag1 = linalg.diagonal_matrix(e, 1)
     offdiag2 = linalg.diagonal_matrix(e, -1)
```

### Comparing `matfree-0.0.3/tests/test_slq.py` & `matfree-0.0.4/tests/test_slq/test_logdet.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 @testing.fixture()
 def A(n, num_significant_eigvals):
     """Make a positive definite matrix with certain spectrum."""
     # 'Invent' a spectrum. Use the number of pre-defined eigenvalues.
     d = np.arange(n) / n + 1.0
     d = d.at[num_significant_eigvals:].set(0.001)
 
-    return test_util.generate_symmetric_matrix_from_eigvals(d)
+    return test_util.symmetric_matrix_from_eigenvalues(d)
 
 
 @testing.parametrize("n", [200])
 @testing.parametrize("num_significant_eigvals", [30])
 @testing.parametrize("order", [10])
 # usually: ~1.5 * num_significant_eigvals.
 # But logdet seems to converge sooo much faster.
```

