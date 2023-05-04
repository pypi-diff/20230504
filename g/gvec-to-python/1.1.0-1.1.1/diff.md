# Comparing `tmp/gvec-to-python-1.1.0.tar.gz` & `tmp/gvec-to-python-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gvec-to-python-1.1.0.tar", last modified: Wed Apr 26 07:45:35 2023, max compression
+gzip compressed data, was "gvec-to-python-1.1.1.tar", last modified: Thu May  4 07:23:11 2023, max compression
```

## Comparing `gvec-to-python-1.1.0.tar` & `gvec-to-python-1.1.1.tar`

### file list

```diff
@@ -1,114 +1,89 @@
-drwxrwxr-x   0 spossann  (1000) spossann  (1000)        0 2023-04-26 07:45:35.308210 gvec-to-python-1.1.0/
--rw-rw-r--   0 spossann  (1000) spossann  (1000)      835 2022-03-10 12:28:57.000000 gvec-to-python-1.1.0/.coveragerc
--rw-rw-r--   0 spossann  (1000) spossann  (1000)     2502 2022-05-20 11:08:31.000000 gvec-to-python-1.1.0/.gitignore
--rw-rw-r--   0 spossann  (1000) spossann  (1000)     2514 2023-04-24 09:45:18.000000 gvec-to-python-1.1.0/.gitlab-ci.yml
--rw-rw-r--   0 spossann  (1000) spossann  (1000)      117 2023-01-24 08:30:08.000000 gvec-to-python-1.1.0/CONTRIBUTING.md
--rw-rw-r--   0 spossann  (1000) spossann  (1000)     1133 2023-04-26 07:34:38.000000 gvec-to-python-1.1.0/LICENSE
--rw-rw-r--   0 spossann  (1000) spossann  (1000)     5191 2021-11-12 09:28:26.000000 gvec-to-python-1.1.0/List_of_data_entries.md
--rw-rw-r--   0 spossann  (1000) spossann  (1000)     6027 2023-04-26 07:45:35.308210 gvec-to-python-1.1.0/PKG-INFO
--rw-rw-r--   0 spossann  (1000) spossann  (1000)     4005 2023-04-24 09:45:18.000000 gvec-to-python-1.1.0/README.md
-drwxrwxr-x   0 spossann  (1000) spossann  (1000)        0 2023-04-26 07:45:35.296210 gvec-to-python-1.1.0/bin/
--rw-rw-r--   0 spossann  (1000) spossann  (1000)      271 2023-01-23 09:09:02.000000 gvec-to-python-1.1.0/bin/compile_gvec_to_python
-drwxrwxr-x   0 spossann  (1000) spossann  (1000)        0 2023-04-26 07:45:35.300210 gvec-to-python-1.1.0/notebooks/
--rw-rw-r--   0 spossann  (1000) spossann  (1000)   117881 2023-04-24 09:45:18.000000 gvec-to-python-1.1.0/notebooks/absB.png
--rw-rw-r--   0 spossann  (1000) spossann  (1000)   126651 2023-04-24 09:45:18.000000 gvec-to-python-1.1.0/notebooks/det_df.png
--rw-rw-r--   0 spossann  (1000) spossann  (1000)   962785 2023-04-24 09:45:18.000000 gvec-to-python-1.1.0/notebooks/dtheta.png
--rw-rw-r--   0 spossann  (1000) spossann  (1000)    19068 2023-04-24 09:45:18.000000 gvec-to-python-1.1.0/notebooks/plot_mhd_equil.ipynb
--rw-rw-r--   0 spossann  (1000) spossann  (1000)   518793 2023-04-24 09:45:18.000000 gvec-to-python-1.1.0/notebooks/poloidal.png
--rw-rw-r--   0 spossann  (1000) spossann  (1000)   160415 2023-04-24 09:45:18.000000 gvec-to-python-1.1.0/notebooks/pressure.png
--rw-rw-r--   0 spossann  (1000) spossann  (1000)    76473 2023-01-24 08:30:08.000000 gvec-to-python-1.1.0/notebooks/profiles.png
--rw-rw-r--   0 spossann  (1000) spossann  (1000)   406292 2023-01-24 08:30:08.000000 gvec-to-python-1.1.0/notebooks/topview.png
--rw-rw-r--   0 spossann  (1000) spossann  (1000)     1819 2023-04-26 07:45:20.000000 gvec-to-python-1.1.0/pyproject.toml
--rw-rw-r--   0 spossann  (1000) spossann  (1000)       38 2023-04-26 07:45:35.308210 gvec-to-python-1.1.0/setup.cfg
-drwxrwxr-x   0 spossann  (1000) spossann  (1000)        0 2023-04-26 07:45:35.296210 gvec-to-python-1.1.0/src/
-drwxrwxr-x   0 spossann  (1000) spossann  (1000)        0 2023-04-26 07:45:35.300210 gvec-to-python-1.1.0/src/gvec_to_python/
--rw-rw-r--   0 spossann  (1000) spossann  (1000)    34611 2023-04-24 09:45:18.000000 gvec-to-python-1.1.0/src/gvec_to_python/GVEC_functions.py
--rw-rw-r--   0 spossann  (1000) spossann  (1000)     1201 2023-01-23 09:09:02.000000 gvec-to-python-1.1.0/src/gvec_to_python/Makefile
--rw-rw-r--   0 spossann  (1000) spossann  (1000)      969 2023-01-23 09:09:02.000000 gvec-to-python-1.1.0/src/gvec_to_python/__init__.py
-drwxrwxr-x   0 spossann  (1000) spossann  (1000)        0 2023-04-26 07:45:35.300210 gvec-to-python-1.1.0/src/gvec_to_python/base/
--rw-rw-r--   0 spossann  (1000) spossann  (1000)      317 2021-11-12 09:28:26.000000 gvec-to-python-1.1.0/src/gvec_to_python/base/__init__.py
--rw-rw-r--   0 spossann  (1000) spossann  (1000)     5015 2023-01-26 18:33:08.000000 gvec-to-python-1.1.0/src/gvec_to_python/base/base.py
--rw-rw-r--   0 spossann  (1000) spossann  (1000)    13375 2023-01-26 18:33:08.000000 gvec-to-python-1.1.0/src/gvec_to_python/base/fbase.py
--rw-rw-r--   0 spossann  (1000) spossann  (1000)     1103 2023-01-23 09:09:02.000000 gvec-to-python-1.1.0/src/gvec_to_python/base/make_base.py
--rw-rw-r--   0 spossann  (1000) spossann  (1000)     3070 2023-01-26 18:33:08.000000 gvec-to-python-1.1.0/src/gvec_to_python/base/sbase.py
-drwxrwxr-x   0 spossann  (1000) spossann  (1000)        0 2023-04-26 07:45:35.300210 gvec-to-python-1.1.0/src/gvec_to_python/console/
--rw-rw-r--   0 spossann  (1000) spossann  (1000)        0 2023-04-26 06:45:56.000000 gvec-to-python-1.1.0/src/gvec_to_python/console/__init__.py
--rw-rw-r--   0 spossann  (1000) spossann  (1000)      422 2023-04-26 06:53:17.000000 gvec-to-python-1.1.0/src/gvec_to_python/console/compile.py
-drwxrwxr-x   0 spossann  (1000) spossann  (1000)        0 2023-04-26 07:45:35.300210 gvec-to-python-1.1.0/src/gvec_to_python/equilibrium/
--rw-rw-r--   0 spossann  (1000) spossann  (1000)        0 2023-01-23 09:09:02.000000 gvec-to-python-1.1.0/src/gvec_to_python/equilibrium/__init__.py
--rw-rw-r--   0 spossann  (1000) spossann  (1000)     4329 2023-01-26 18:33:08.000000 gvec-to-python-1.1.0/src/gvec_to_python/equilibrium/profiles.py
-drwxrwxr-x   0 spossann  (1000) spossann  (1000)        0 2023-04-26 07:45:35.304211 gvec-to-python-1.1.0/src/gvec_to_python/geometry/
--rw-rw-r--   0 spossann  (1000) spossann  (1000)      531 2023-01-23 09:09:02.000000 gvec-to-python-1.1.0/src/gvec_to_python/geometry/__init__.py
--rw-rw-r--   0 spossann  (1000) spossann  (1000)    46341 2023-04-24 09:45:18.000000 gvec-to-python-1.1.0/src/gvec_to_python/geometry/domain.py
--rw-rw-r--   0 spossann  (1000) spossann  (1000)     1785 2023-01-23 09:09:02.000000 gvec-to-python-1.1.0/src/gvec_to_python/geometry/kernels.py
-drwxrwxr-x   0 spossann  (1000) spossann  (1000)        0 2023-04-26 07:45:35.304211 gvec-to-python-1.1.0/src/gvec_to_python/hylife/
--rw-rw-r--   0 spossann  (1000) spossann  (1000)      182 2021-11-12 09:28:26.000000 gvec-to-python-1.1.0/src/gvec_to_python/hylife/__init__.py
-drwxrwxr-x   0 spossann  (1000) spossann  (1000)        0 2023-04-26 07:45:35.304211 gvec-to-python-1.1.0/src/gvec_to_python/hylife/utilities_FEEC/
--rw-rw-r--   0 spossann  (1000) spossann  (1000)      269 2021-11-12 09:28:26.000000 gvec-to-python-1.1.0/src/gvec_to_python/hylife/utilities_FEEC/__init__.py
-drwxrwxr-x   0 spossann  (1000) spossann  (1000)        0 2023-04-26 07:45:35.304211 gvec-to-python-1.1.0/src/gvec_to_python/hylife/utilities_FEEC/basics/
--rw-rw-r--   0 spossann  (1000) spossann  (1000)      188 2021-11-12 09:28:26.000000 gvec-to-python-1.1.0/src/gvec_to_python/hylife/utilities_FEEC/basics/__init__.py
--rw-rw-r--   0 spossann  (1000) spossann  (1000)     6544 2023-01-26 18:33:08.000000 gvec-to-python-1.1.0/src/gvec_to_python/hylife/utilities_FEEC/basics/spline_evaluation_1d.py
--rw-rw-r--   0 spossann  (1000) spossann  (1000)    20753 2021-11-12 09:28:26.000000 gvec-to-python-1.1.0/src/gvec_to_python/hylife/utilities_FEEC/bsplines.py
--rw-rw-r--   0 spossann  (1000) spossann  (1000)     9693 2023-01-26 18:33:08.000000 gvec-to-python-1.1.0/src/gvec_to_python/hylife/utilities_FEEC/bsplines_kernels.py
-drwxrwxr-x   0 spossann  (1000) spossann  (1000)        0 2023-04-26 07:45:35.304211 gvec-to-python-1.1.0/src/gvec_to_python/hylife/utilities_FEEC/derivatives/
--rw-rw-r--   0 spossann  (1000) spossann  (1000)      179 2021-11-12 09:28:26.000000 gvec-to-python-1.1.0/src/gvec_to_python/hylife/utilities_FEEC/derivatives/__init__.py
--rw-rw-r--   0 spossann  (1000) spossann  (1000)     5663 2021-11-12 09:28:26.000000 gvec-to-python-1.1.0/src/gvec_to_python/hylife/utilities_FEEC/derivatives/derivatives.py
--rw-rw-r--   0 spossann  (1000) spossann  (1000)    15218 2023-01-26 18:33:08.000000 gvec-to-python-1.1.0/src/gvec_to_python/hylife/utilities_FEEC/spline_space.py
--rw-rw-r--   0 spossann  (1000) spossann  (1000)      229 2021-11-12 09:28:26.000000 gvec-to-python-1.1.0/src/gvec_to_python/main.py
-drwxrwxr-x   0 spossann  (1000) spossann  (1000)        0 2023-04-26 07:45:35.304211 gvec-to-python-1.1.0/src/gvec_to_python/reader/
--rw-rw-r--   0 spossann  (1000) spossann  (1000)      405 2022-05-20 11:08:31.000000 gvec-to-python-1.1.0/src/gvec_to_python/reader/__init__.py
--rw-rw-r--   0 spossann  (1000) spossann  (1000)    13117 2023-01-26 15:32:59.000000 gvec-to-python-1.1.0/src/gvec_to_python/reader/gvec_reader.py
-drwxrwxr-x   0 spossann  (1000) spossann  (1000)        0 2023-04-26 07:45:35.304211 gvec-to-python-1.1.0/src/gvec_to_python/testcases/
--rw-rw-r--   0 spossann  (1000) spossann  (1000)        0 2023-01-23 09:09:02.000000 gvec-to-python-1.1.0/src/gvec_to_python/testcases/__init__.py
-drwxrwxr-x   0 spossann  (1000) spossann  (1000)        0 2023-04-26 07:45:35.304211 gvec-to-python-1.1.0/src/gvec_to_python/testcases/circ_tok/
--rw-rw-r--   0 spossann  (1000) spossann  (1000)    51408 2023-01-23 09:09:02.000000 gvec-to-python-1.1.0/src/gvec_to_python/testcases/circ_tok/CIRC_TOK_State_0000_00010000.dat
--rw-rw-r--   0 spossann  (1000) spossann  (1000)    82363 2023-01-23 09:09:02.000000 gvec-to-python-1.1.0/src/gvec_to_python/testcases/circ_tok/CIRC_TOK_State_0000_00010000.json
--rw-rw-r--   0 spossann  (1000) spossann  (1000)     2287 2023-01-23 09:09:02.000000 gvec-to-python-1.1.0/src/gvec_to_python/testcases/circ_tok/iota_profile_fit.vsz
--rw-rw-r--   0 spossann  (1000) spossann  (1000)    39044 2023-01-23 09:09:02.000000 gvec-to-python-1.1.0/src/gvec_to_python/testcases/circ_tok/logMinimizer_CIRC_TOK_0000.csv
--rw-rw-r--   0 spossann  (1000) spossann  (1000)     7519 2023-01-23 09:09:02.000000 gvec-to-python-1.1.0/src/gvec_to_python/testcases/circ_tok/parameter.ini
-drwxrwxr-x   0 spossann  (1000) spossann  (1000)        0 2023-04-26 07:45:35.304211 gvec-to-python-1.1.0/src/gvec_to_python/testcases/ellipstell/
--rw-rw-r--   0 spossann  (1000) spossann  (1000)      488 2023-01-26 15:32:59.000000 gvec-to-python-1.1.0/src/gvec_to_python/testcases/ellipstell/README.md
-drwxrwxr-x   0 spossann  (1000) spossann  (1000)        0 2023-04-26 07:45:35.304211 gvec-to-python-1.1.0/src/gvec_to_python/testcases/ellipstell/newBC_E1D6_M6N6/
--rw-rw-r--   0 spossann  (1000) spossann  (1000)    49404 2023-01-26 15:32:59.000000 gvec-to-python-1.1.0/src/gvec_to_python/testcases/ellipstell/newBC_E1D6_M6N6/GVEC_ELLIPSTELL_E1D6_M6N6_State_0000_00200000.dat
--rw-rw-r--   0 spossann  (1000) spossann  (1000)     6859 2023-01-26 15:32:59.000000 gvec-to-python-1.1.0/src/gvec_to_python/testcases/ellipstell/newBC_E1D6_M6N6/parameter.ini
-drwxrwxr-x   0 spossann  (1000) spossann  (1000)        0 2023-04-26 07:45:35.304211 gvec-to-python-1.1.0/src/gvec_to_python/testcases/ellipstell/newBC_E4D6_M6N6/
--rw-rw-r--   0 spossann  (1000) spossann  (1000)    68052 2023-01-26 15:32:59.000000 gvec-to-python-1.1.0/src/gvec_to_python/testcases/ellipstell/newBC_E4D6_M6N6/GVEC_ELLIPSTELL_E4D6_M6N6_State_0001_00200000.dat
--rw-rw-r--   0 spossann  (1000) spossann  (1000)     6859 2023-01-26 15:32:59.000000 gvec-to-python-1.1.0/src/gvec_to_python/testcases/ellipstell/newBC_E4D6_M6N6/parameter.ini
-drwxrwxr-x   0 spossann  (1000) spossann  (1000)        0 2023-04-26 07:45:35.296210 gvec-to-python-1.1.0/src/gvec_to_python/testcases/ellipstell_v2/
-drwxrwxr-x   0 spossann  (1000) spossann  (1000)        0 2023-04-26 07:45:35.304211 gvec-to-python-1.1.0/src/gvec_to_python/testcases/ellipstell_v2/newBC_E1D6_M6N6/
--rw-rw-r--   0 spossann  (1000) spossann  (1000)    65028 2023-01-23 09:09:02.000000 gvec-to-python-1.1.0/src/gvec_to_python/testcases/ellipstell_v2/newBC_E1D6_M6N6/GVEC_ELLIPSTELL_V2_State_0000_00200000.dat
--rw-rw-r--   0 spossann  (1000) spossann  (1000)   118164 2023-01-26 14:58:02.000000 gvec-to-python-1.1.0/src/gvec_to_python/testcases/ellipstell_v2/newBC_E1D6_M6N6/GVEC_ELLIPSTELL_V2_State_0000_00200000.json
--rw-rw-r--   0 spossann  (1000) spossann  (1000)     7253 2023-01-23 09:09:02.000000 gvec-to-python-1.1.0/src/gvec_to_python/testcases/ellipstell_v2/newBC_E1D6_M6N6/parameter.ini
-drwxrwxr-x   0 spossann  (1000) spossann  (1000)        0 2023-04-26 07:45:35.304211 gvec-to-python-1.1.0/src/gvec_to_python/testcases/ellipstell_v2/newBC_E4D6_M6N6/
--rw-rw-r--   0 spossann  (1000) spossann  (1000)    89724 2023-01-23 09:09:02.000000 gvec-to-python-1.1.0/src/gvec_to_python/testcases/ellipstell_v2/newBC_E4D6_M6N6/GVEC_ELLIPSTELL_V2_State_0000_00200000.dat
--rw-rw-r--   0 spossann  (1000) spossann  (1000)   167883 2023-01-23 09:09:02.000000 gvec-to-python-1.1.0/src/gvec_to_python/testcases/ellipstell_v2/newBC_E4D6_M6N6/GVEC_ELLIPSTELL_V2_State_0000_00200000.json
--rw-rw-r--   0 spossann  (1000) spossann  (1000)     7276 2023-01-23 09:09:02.000000 gvec-to-python-1.1.0/src/gvec_to_python/testcases/ellipstell_v2/newBC_E4D6_M6N6/parameter.ini
-drwxrwxr-x   0 spossann  (1000) spossann  (1000)        0 2023-04-26 07:45:35.304211 gvec-to-python-1.1.0/src/gvec_to_python/testcases/ellipstell_v2/oldBC_E40D5M6N6/
--rw-rw-r--   0 spossann  (1000) spossann  (1000)   161316 2023-01-23 09:09:02.000000 gvec-to-python-1.1.0/src/gvec_to_python/testcases/ellipstell_v2/oldBC_E40D5M6N6/GVEC_ELLIPSTELL_V2_State_0000_00200000.dat
--rw-rw-r--   0 spossann  (1000) spossann  (1000)   272577 2023-01-23 09:09:02.000000 gvec-to-python-1.1.0/src/gvec_to_python/testcases/ellipstell_v2/oldBC_E40D5M6N6/GVEC_ELLIPSTELL_V2_State_0000_00200000.json
--rw-rw-r--   0 spossann  (1000) spossann  (1000)     7249 2023-01-23 09:09:02.000000 gvec-to-python-1.1.0/src/gvec_to_python/testcases/ellipstell_v2/oldBC_E40D5M6N6/parameter.ini
-drwxrwxr-x   0 spossann  (1000) spossann  (1000)        0 2023-04-26 07:45:35.308210 gvec-to-python-1.1.0/src/gvec_to_python/util/
--rw-rw-r--   0 spossann  (1000) spossann  (1000)      262 2021-11-12 09:28:26.000000 gvec-to-python-1.1.0/src/gvec_to_python/util/__init__.py
--rw-rw-r--   0 spossann  (1000) spossann  (1000)      588 2021-11-12 09:28:26.000000 gvec-to-python-1.1.0/src/gvec_to_python/util/logger.py
--rw-rw-r--   0 spossann  (1000) spossann  (1000)      629 2021-11-12 09:28:26.000000 gvec-to-python-1.1.0/src/gvec_to_python/util/numpy_encoder.py
--rw-rw-r--   0 spossann  (1000) spossann  (1000)      370 2023-04-24 09:45:18.000000 gvec-to-python-1.1.0/src/gvec_to_python/version.py
-drwxrwxr-x   0 spossann  (1000) spossann  (1000)        0 2023-04-26 07:45:35.308210 gvec-to-python-1.1.0/src/gvec_to_python/writer/
--rw-rw-r--   0 spossann  (1000) spossann  (1000)      176 2021-11-12 09:28:26.000000 gvec-to-python-1.1.0/src/gvec_to_python/writer/__init__.py
-drwxrwxr-x   0 spossann  (1000) spossann  (1000)        0 2023-04-26 07:45:35.308210 gvec-to-python-1.1.0/src/gvec_to_python/writer/paraview/
--rw-rw-r--   0 spossann  (1000) spossann  (1000)      259 2021-11-12 09:28:26.000000 gvec-to-python-1.1.0/src/gvec_to_python/writer/paraview/__init__.py
--rw-rw-r--   0 spossann  (1000) spossann  (1000)    31373 2022-05-20 11:08:31.000000 gvec-to-python-1.1.0/src/gvec_to_python/writer/paraview/mesh_creator.py
--rw-rw-r--   0 spossann  (1000) spossann  (1000)     3011 2022-03-10 12:28:57.000000 gvec-to-python-1.1.0/src/gvec_to_python/writer/paraview/vtk_writer.py
-drwxrwxr-x   0 spossann  (1000) spossann  (1000)        0 2023-04-26 07:45:35.300210 gvec-to-python-1.1.0/src/gvec_to_python.egg-info/
--rw-rw-r--   0 spossann  (1000) spossann  (1000)     6027 2023-04-26 07:45:35.000000 gvec-to-python-1.1.0/src/gvec_to_python.egg-info/PKG-INFO
--rw-rw-r--   0 spossann  (1000) spossann  (1000)     3837 2023-04-26 07:45:35.000000 gvec-to-python-1.1.0/src/gvec_to_python.egg-info/SOURCES.txt
--rw-rw-r--   0 spossann  (1000) spossann  (1000)        1 2023-04-26 07:45:35.000000 gvec-to-python-1.1.0/src/gvec_to_python.egg-info/dependency_links.txt
--rw-rw-r--   0 spossann  (1000) spossann  (1000)       90 2023-04-26 07:45:35.000000 gvec-to-python-1.1.0/src/gvec_to_python.egg-info/entry_points.txt
--rw-rw-r--   0 spossann  (1000) spossann  (1000)       90 2023-04-26 07:45:35.000000 gvec-to-python-1.1.0/src/gvec_to_python.egg-info/requires.txt
--rw-rw-r--   0 spossann  (1000) spossann  (1000)       15 2023-04-26 07:45:35.000000 gvec-to-python-1.1.0/src/gvec_to_python.egg-info/top_level.txt
-drwxrwxr-x   0 spossann  (1000) spossann  (1000)        0 2023-04-26 07:45:35.308210 gvec-to-python-1.1.0/tests/
--rw-rw-r--   0 spossann  (1000) spossann  (1000)     7356 2023-04-24 09:45:18.000000 gvec-to-python-1.1.0/tests/test_gvec_domain.py
--rw-rw-r--   0 spossann  (1000) spossann  (1000)    13089 2023-04-24 09:45:18.000000 gvec-to-python-1.1.0/tests/test_gvec_equil.py
--rw-rw-r--   0 spossann  (1000) spossann  (1000)     3929 2023-01-26 18:33:08.000000 gvec-to-python-1.1.0/tests/test_gvec_profiles.py
--rw-rw-r--   0 spossann  (1000) spossann  (1000)     2452 2023-01-26 18:33:08.000000 gvec-to-python-1.1.0/tests/test_splines.py
--rw-rw-r--   0 spossann  (1000) spossann  (1000)    15666 2023-01-23 09:09:02.000000 gvec-to-python-1.1.0/tests/xxx_test_blown_up_B.py
--rw-rw-r--   0 spossann  (1000) spossann  (1000)     6933 2023-01-23 09:09:02.000000 gvec-to-python-1.1.0/tests/xxx_test_paraview.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:23:11.195898 gvec-to-python-1.1.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1133 2023-05-04 07:22:25.000000 gvec-to-python-1.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5841 2023-05-04 07:23:11.195898 gvec-to-python-1.1.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3985 2023-05-04 07:22:25.000000 gvec-to-python-1.1.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1683 2023-05-04 07:22:25.000000 gvec-to-python-1.1.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-04 07:23:11.195898 gvec-to-python-1.1.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:23:11.179898 gvec-to-python-1.1.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:23:11.183898 gvec-to-python-1.1.1/src/gvec_to_python/
+-rw-rw-rw-   0 root         (0) root         (0)    34611 2023-05-04 07:22:25.000000 gvec-to-python-1.1.1/src/gvec_to_python/GVEC_functions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1201 2023-05-04 07:22:25.000000 gvec-to-python-1.1.1/src/gvec_to_python/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      969 2023-05-04 07:22:25.000000 gvec-to-python-1.1.1/src/gvec_to_python/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:23:11.187898 gvec-to-python-1.1.1/src/gvec_to_python/base/
+-rw-rw-rw-   0 root         (0) root         (0)      317 2023-05-04 07:22:25.000000 gvec-to-python-1.1.1/src/gvec_to_python/base/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5015 2023-05-04 07:22:25.000000 gvec-to-python-1.1.1/src/gvec_to_python/base/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    13375 2023-05-04 07:22:25.000000 gvec-to-python-1.1.1/src/gvec_to_python/base/fbase.py
+-rw-rw-rw-   0 root         (0) root         (0)     1103 2023-05-04 07:22:25.000000 gvec-to-python-1.1.1/src/gvec_to_python/base/make_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3070 2023-05-04 07:22:25.000000 gvec-to-python-1.1.1/src/gvec_to_python/base/sbase.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:23:11.187898 gvec-to-python-1.1.1/src/gvec_to_python/console/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-04 07:22:25.000000 gvec-to-python-1.1.1/src/gvec_to_python/console/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      422 2023-05-04 07:22:25.000000 gvec-to-python-1.1.1/src/gvec_to_python/console/compile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:23:11.187898 gvec-to-python-1.1.1/src/gvec_to_python/equilibrium/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-04 07:22:25.000000 gvec-to-python-1.1.1/src/gvec_to_python/equilibrium/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4329 2023-05-04 07:22:25.000000 gvec-to-python-1.1.1/src/gvec_to_python/equilibrium/profiles.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:23:11.187898 gvec-to-python-1.1.1/src/gvec_to_python/geometry/
+-rw-rw-rw-   0 root         (0) root         (0)      531 2023-05-04 07:22:25.000000 gvec-to-python-1.1.1/src/gvec_to_python/geometry/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    46341 2023-05-04 07:22:25.000000 gvec-to-python-1.1.1/src/gvec_to_python/geometry/domain.py
+-rw-rw-rw-   0 root         (0) root         (0)     1785 2023-05-04 07:22:25.000000 gvec-to-python-1.1.1/src/gvec_to_python/geometry/kernels.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:23:11.187898 gvec-to-python-1.1.1/src/gvec_to_python/hylife/
+-rw-rw-rw-   0 root         (0) root         (0)      182 2023-05-04 07:22:25.000000 gvec-to-python-1.1.1/src/gvec_to_python/hylife/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:23:11.187898 gvec-to-python-1.1.1/src/gvec_to_python/hylife/utilities_FEEC/
+-rw-rw-rw-   0 root         (0) root         (0)      269 2023-05-04 07:22:25.000000 gvec-to-python-1.1.1/src/gvec_to_python/hylife/utilities_FEEC/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:23:11.187898 gvec-to-python-1.1.1/src/gvec_to_python/hylife/utilities_FEEC/basics/
+-rw-rw-rw-   0 root         (0) root         (0)      188 2023-05-04 07:22:25.000000 gvec-to-python-1.1.1/src/gvec_to_python/hylife/utilities_FEEC/basics/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6544 2023-05-04 07:22:25.000000 gvec-to-python-1.1.1/src/gvec_to_python/hylife/utilities_FEEC/basics/spline_evaluation_1d.py
+-rw-rw-rw-   0 root         (0) root         (0)    20753 2023-05-04 07:22:25.000000 gvec-to-python-1.1.1/src/gvec_to_python/hylife/utilities_FEEC/bsplines.py
+-rw-rw-rw-   0 root         (0) root         (0)     9693 2023-05-04 07:22:25.000000 gvec-to-python-1.1.1/src/gvec_to_python/hylife/utilities_FEEC/bsplines_kernels.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:23:11.187898 gvec-to-python-1.1.1/src/gvec_to_python/hylife/utilities_FEEC/derivatives/
+-rw-rw-rw-   0 root         (0) root         (0)      179 2023-05-04 07:22:25.000000 gvec-to-python-1.1.1/src/gvec_to_python/hylife/utilities_FEEC/derivatives/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5663 2023-05-04 07:22:25.000000 gvec-to-python-1.1.1/src/gvec_to_python/hylife/utilities_FEEC/derivatives/derivatives.py
+-rw-rw-rw-   0 root         (0) root         (0)    15218 2023-05-04 07:22:25.000000 gvec-to-python-1.1.1/src/gvec_to_python/hylife/utilities_FEEC/spline_space.py
+-rw-rw-rw-   0 root         (0) root         (0)      229 2023-05-04 07:22:25.000000 gvec-to-python-1.1.1/src/gvec_to_python/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:23:11.191898 gvec-to-python-1.1.1/src/gvec_to_python/reader/
+-rw-rw-rw-   0 root         (0) root         (0)      405 2023-05-04 07:22:25.000000 gvec-to-python-1.1.1/src/gvec_to_python/reader/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13117 2023-05-04 07:22:25.000000 gvec-to-python-1.1.1/src/gvec_to_python/reader/gvec_reader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:23:11.191898 gvec-to-python-1.1.1/src/gvec_to_python/testcases/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-04 07:22:25.000000 gvec-to-python-1.1.1/src/gvec_to_python/testcases/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:23:11.191898 gvec-to-python-1.1.1/src/gvec_to_python/testcases/circ_tok/
+-rw-rw-rw-   0 root         (0) root         (0)    51408 2023-05-04 07:22:25.000000 gvec-to-python-1.1.1/src/gvec_to_python/testcases/circ_tok/CIRC_TOK_State_0000_00010000.dat
+-rw-rw-rw-   0 root         (0) root         (0)     7519 2023-05-04 07:22:25.000000 gvec-to-python-1.1.1/src/gvec_to_python/testcases/circ_tok/parameter.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:23:11.183898 gvec-to-python-1.1.1/src/gvec_to_python/testcases/ellipstell/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:23:11.191898 gvec-to-python-1.1.1/src/gvec_to_python/testcases/ellipstell/newBC_E1D6_M6N6/
+-rw-rw-rw-   0 root         (0) root         (0)    49404 2023-05-04 07:22:25.000000 gvec-to-python-1.1.1/src/gvec_to_python/testcases/ellipstell/newBC_E1D6_M6N6/GVEC_ELLIPSTELL_E1D6_M6N6_State_0000_00200000.dat
+-rw-rw-rw-   0 root         (0) root         (0)     6859 2023-05-04 07:22:25.000000 gvec-to-python-1.1.1/src/gvec_to_python/testcases/ellipstell/newBC_E1D6_M6N6/parameter.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:23:11.191898 gvec-to-python-1.1.1/src/gvec_to_python/testcases/ellipstell/newBC_E4D6_M6N6/
+-rw-rw-rw-   0 root         (0) root         (0)    68052 2023-05-04 07:22:25.000000 gvec-to-python-1.1.1/src/gvec_to_python/testcases/ellipstell/newBC_E4D6_M6N6/GVEC_ELLIPSTELL_E4D6_M6N6_State_0001_00200000.dat
+-rw-rw-rw-   0 root         (0) root         (0)     6859 2023-05-04 07:22:25.000000 gvec-to-python-1.1.1/src/gvec_to_python/testcases/ellipstell/newBC_E4D6_M6N6/parameter.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:23:11.183898 gvec-to-python-1.1.1/src/gvec_to_python/testcases/ellipstell_v2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:23:11.191898 gvec-to-python-1.1.1/src/gvec_to_python/testcases/ellipstell_v2/newBC_E1D6_M6N6/
+-rw-rw-rw-   0 root         (0) root         (0)    65028 2023-05-04 07:22:25.000000 gvec-to-python-1.1.1/src/gvec_to_python/testcases/ellipstell_v2/newBC_E1D6_M6N6/GVEC_ELLIPSTELL_V2_State_0000_00200000.dat
+-rw-rw-rw-   0 root         (0) root         (0)     7253 2023-05-04 07:22:25.000000 gvec-to-python-1.1.1/src/gvec_to_python/testcases/ellipstell_v2/newBC_E1D6_M6N6/parameter.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:23:11.191898 gvec-to-python-1.1.1/src/gvec_to_python/testcases/ellipstell_v2/newBC_E4D6_M6N6/
+-rw-rw-rw-   0 root         (0) root         (0)    89724 2023-05-04 07:22:25.000000 gvec-to-python-1.1.1/src/gvec_to_python/testcases/ellipstell_v2/newBC_E4D6_M6N6/GVEC_ELLIPSTELL_V2_State_0000_00200000.dat
+-rw-rw-rw-   0 root         (0) root         (0)     7276 2023-05-04 07:22:25.000000 gvec-to-python-1.1.1/src/gvec_to_python/testcases/ellipstell_v2/newBC_E4D6_M6N6/parameter.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:23:11.191898 gvec-to-python-1.1.1/src/gvec_to_python/testcases/ellipstell_v2/oldBC_E40D5M6N6/
+-rw-rw-rw-   0 root         (0) root         (0)   161316 2023-05-04 07:22:25.000000 gvec-to-python-1.1.1/src/gvec_to_python/testcases/ellipstell_v2/oldBC_E40D5M6N6/GVEC_ELLIPSTELL_V2_State_0000_00200000.dat
+-rw-rw-rw-   0 root         (0) root         (0)     7249 2023-05-04 07:22:25.000000 gvec-to-python-1.1.1/src/gvec_to_python/testcases/ellipstell_v2/oldBC_E40D5M6N6/parameter.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:23:11.195898 gvec-to-python-1.1.1/src/gvec_to_python/util/
+-rw-rw-rw-   0 root         (0) root         (0)      262 2023-05-04 07:22:25.000000 gvec-to-python-1.1.1/src/gvec_to_python/util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      588 2023-05-04 07:22:25.000000 gvec-to-python-1.1.1/src/gvec_to_python/util/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)      629 2023-05-04 07:22:25.000000 gvec-to-python-1.1.1/src/gvec_to_python/util/numpy_encoder.py
+-rw-rw-rw-   0 root         (0) root         (0)      370 2023-05-04 07:22:25.000000 gvec-to-python-1.1.1/src/gvec_to_python/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:23:11.195898 gvec-to-python-1.1.1/src/gvec_to_python/writer/
+-rw-rw-rw-   0 root         (0) root         (0)      176 2023-05-04 07:22:25.000000 gvec-to-python-1.1.1/src/gvec_to_python/writer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:23:11.195898 gvec-to-python-1.1.1/src/gvec_to_python/writer/paraview/
+-rw-rw-rw-   0 root         (0) root         (0)      259 2023-05-04 07:22:25.000000 gvec-to-python-1.1.1/src/gvec_to_python/writer/paraview/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    31373 2023-05-04 07:22:25.000000 gvec-to-python-1.1.1/src/gvec_to_python/writer/paraview/mesh_creator.py
+-rw-rw-rw-   0 root         (0) root         (0)     3011 2023-05-04 07:22:25.000000 gvec-to-python-1.1.1/src/gvec_to_python/writer/paraview/vtk_writer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:23:11.187898 gvec-to-python-1.1.1/src/gvec_to_python.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5841 2023-05-04 07:23:11.000000 gvec-to-python-1.1.1/src/gvec_to_python.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2934 2023-05-04 07:23:11.000000 gvec-to-python-1.1.1/src/gvec_to_python.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 07:23:11.000000 gvec-to-python-1.1.1/src/gvec_to_python.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2023-05-04 07:23:11.000000 gvec-to-python-1.1.1/src/gvec_to_python.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2023-05-04 07:23:11.000000 gvec-to-python-1.1.1/src/gvec_to_python.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-04 07:23:11.000000 gvec-to-python-1.1.1/src/gvec_to_python.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:23:11.195898 gvec-to-python-1.1.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     7356 2023-05-04 07:22:25.000000 gvec-to-python-1.1.1/tests/test_gvec_domain.py
+-rw-rw-rw-   0 root         (0) root         (0)    13089 2023-05-04 07:22:25.000000 gvec-to-python-1.1.1/tests/test_gvec_equil.py
+-rw-rw-rw-   0 root         (0) root         (0)     3929 2023-05-04 07:22:25.000000 gvec-to-python-1.1.1/tests/test_gvec_profiles.py
+-rw-rw-rw-   0 root         (0) root         (0)     2452 2023-05-04 07:22:25.000000 gvec-to-python-1.1.1/tests/test_splines.py
```

### Comparing `gvec-to-python-1.1.0/LICENSE` & `gvec-to-python-1.1.1/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright 2023 (c) T.K. Cheng, F. Hindenlang, S. Possanner | Max Planck Institute for Plasma Physics
+Copyright 2021 (c) T.K. Cheng, F. Hindenlang, S. Possanner | Max Planck Institute for Plasma Physics
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software 
 and associated documentation files (the "Software"), to deal in the Software without restriction, 
 including without limitation the rights to use, copy, modify, merge, publish, distribute, 
 sublicense, and/or sell copies of the Software, and to permit persons to whom the Software 
 is furnished to do so, subject to the following conditions:
```

### Comparing `gvec-to-python-1.1.0/PKG-INFO` & `gvec-to-python-1.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: gvec-to-python
-Version: 1.1.0
+Version: 1.1.1
 Summary: Parse GVEC output in Python
 Author: Tin Kei Cheng, Florian Hindenlang, Stefan Possanner
 Author-email: stefan.possanner@ipp.mpg.de, florian.hindenlang@ipp.mpg.de
-License: Copyright 2023 (c) T.K. Cheng, F. Hindenlang, S. Possanner | Max Planck Institute for Plasma Physics
+License: Copyright 2021 (c) T.K. Cheng, F. Hindenlang, S. Possanner | Max Planck Institute for Plasma Physics
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software 
         and associated documentation files (the "Software"), to deal in the Software without restriction, 
         including without limitation the rights to use, copy, modify, merge, publish, distribute, 
         sublicense, and/or sell copies of the Software, and to permit persons to whom the Software 
         is furnished to do so, subject to the following conditions:
         
@@ -16,41 +16,38 @@
         or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, 
         INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR 
         PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE 
         FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, 
         ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-Project-URL: homepage, https://gitlab.mpcdf.mpg.de/spossann/gvec_to_python
-Project-URL: documentation, https://readthedocs.org
-Project-URL: repository, https://github.com/me/spam.git
-Project-URL: changelog, https://github.com/me/spam/blob/master/CHANGELOG.md
-Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
+Project-URL: repository, https://gitlab.mpcdf.mpg.de/spossann/gvec_to_python
+Project-URL: Bug Tracker, https://gitlab.mpcdf.mpg.de/spossann/gvec_to_python/-/issues
 Keywords: plasma physics,fusion,numerical modeling,mhd equilibrium
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 3D GVEC equilibria in Python
 
-PyPI install (not yet :-):
+PyPI install:
 
 ```
 pip install gvec_to_python
 ```
 Or from source:
 ```
 git clone git@gitlab.mpcdf.mpg.de:spossann/gvec_to_python.git
 cd gvec_to_python
 pip install -e .
 ```
 Compile kernels for faster evaluations:
 ```
-compile_gvec_to_python
+compile-gvec-tp
 ```
 
 # Usage
 
 The [Galerkin Variational Equilibrium Code (GVEC)](https://gitlab.mpcdf.mpg.de/gvec-group/gvec) calculates magneto-hydrodynamic (MHD) equilibria for Tokamaks and Stellarators. `gvec_to_python` parses the GVEC output file (`.dat`) and collects the data in a `.json` file: 
 ```
 from gvec_to_python.reader.gvec_reader import create_GVEC_json
```

### Comparing `gvec-to-python-1.1.0/README.md` & `gvec-to-python-1.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # 3D GVEC equilibria in Python
 
-PyPI install (not yet :-):
+PyPI install:
 
 ```
 pip install gvec_to_python
 ```
 Or from source:
 ```
 git clone git@gitlab.mpcdf.mpg.de:spossann/gvec_to_python.git
 cd gvec_to_python
 pip install -e .
 ```
 Compile kernels for faster evaluations:
 ```
-compile_gvec_to_python
+compile-gvec-tp
 ```
 
 # Usage
 
 The [Galerkin Variational Equilibrium Code (GVEC)](https://gitlab.mpcdf.mpg.de/gvec-group/gvec) calculates magneto-hydrodynamic (MHD) equilibria for Tokamaks and Stellarators. `gvec_to_python` parses the GVEC output file (`.dat`) and collects the data in a `.json` file: 
 ```
 from gvec_to_python.reader.gvec_reader import create_GVEC_json
```

### Comparing `gvec-to-python-1.1.0/pyproject.toml` & `gvec-to-python-1.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gvec-to-python"
-version = "1.1.0"
+version = "1.1.1"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 authors = [
   { name = "Tin Kei Cheng"},
   { name = "Florian Hindenlang"},
   { name = "Stefan Possanner"}, 
@@ -27,19 +27,16 @@
     'pyccel',
     'scipy>=1.6.0',
     'tqdm>=4.56.0',
     'vtk>=9.0.3', 
 ]
 
 [project.urls]
-homepage = "https://gitlab.mpcdf.mpg.de/spossann/gvec_to_python"
-documentation = "https://readthedocs.org"
-repository = "https://github.com/me/spam.git"
-changelog = "https://github.com/me/spam/blob/master/CHANGELOG.md"
-"Bug Tracker" = "https://github.com/pypa/sampleproject/issues"
+repository = "https://gitlab.mpcdf.mpg.de/spossann/gvec_to_python"
+"Bug Tracker" = "https://gitlab.mpcdf.mpg.de/spossann/gvec_to_python/-/issues"
 
 [project.scripts]
 compile-gvec-tp = "gvec_to_python.console.compile:compile_gvec_to_python"
 
 [tool.setuptools.package-data]
 'gvec_to_python.testcases' = [
             'circ_tok/*.dat',
```

### Comparing `gvec-to-python-1.1.0/src/gvec_to_python/GVEC_functions.py` & `gvec-to-python-1.1.1/src/gvec_to_python/GVEC_functions.py`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.0/src/gvec_to_python/Makefile` & `gvec-to-python-1.1.1/src/gvec_to_python/Makefile`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.0/src/gvec_to_python/__init__.py` & `gvec-to-python-1.1.1/src/gvec_to_python/__init__.py`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.0/src/gvec_to_python/base/base.py` & `gvec-to-python-1.1.1/src/gvec_to_python/base/base.py`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.0/src/gvec_to_python/base/fbase.py` & `gvec-to-python-1.1.1/src/gvec_to_python/base/fbase.py`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.0/src/gvec_to_python/base/make_base.py` & `gvec-to-python-1.1.1/src/gvec_to_python/base/make_base.py`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.0/src/gvec_to_python/base/sbase.py` & `gvec-to-python-1.1.1/src/gvec_to_python/base/sbase.py`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.0/src/gvec_to_python/equilibrium/profiles.py` & `gvec-to-python-1.1.1/src/gvec_to_python/equilibrium/profiles.py`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.0/src/gvec_to_python/geometry/__init__.py` & `gvec-to-python-1.1.1/src/gvec_to_python/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.0/src/gvec_to_python/geometry/domain.py` & `gvec-to-python-1.1.1/src/gvec_to_python/geometry/domain.py`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.0/src/gvec_to_python/geometry/kernels.py` & `gvec-to-python-1.1.1/src/gvec_to_python/geometry/kernels.py`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.0/src/gvec_to_python/hylife/utilities_FEEC/basics/spline_evaluation_1d.py` & `gvec-to-python-1.1.1/src/gvec_to_python/hylife/utilities_FEEC/basics/spline_evaluation_1d.py`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.0/src/gvec_to_python/hylife/utilities_FEEC/bsplines.py` & `gvec-to-python-1.1.1/src/gvec_to_python/hylife/utilities_FEEC/bsplines.py`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.0/src/gvec_to_python/hylife/utilities_FEEC/bsplines_kernels.py` & `gvec-to-python-1.1.1/src/gvec_to_python/hylife/utilities_FEEC/bsplines_kernels.py`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.0/src/gvec_to_python/hylife/utilities_FEEC/derivatives/derivatives.py` & `gvec-to-python-1.1.1/src/gvec_to_python/hylife/utilities_FEEC/derivatives/derivatives.py`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.0/src/gvec_to_python/hylife/utilities_FEEC/spline_space.py` & `gvec-to-python-1.1.1/src/gvec_to_python/hylife/utilities_FEEC/spline_space.py`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.0/src/gvec_to_python/reader/gvec_reader.py` & `gvec-to-python-1.1.1/src/gvec_to_python/reader/gvec_reader.py`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.0/src/gvec_to_python/testcases/circ_tok/CIRC_TOK_State_0000_00010000.dat` & `gvec-to-python-1.1.1/src/gvec_to_python/testcases/circ_tok/CIRC_TOK_State_0000_00010000.dat`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.0/src/gvec_to_python/testcases/circ_tok/parameter.ini` & `gvec-to-python-1.1.1/src/gvec_to_python/testcases/circ_tok/parameter.ini`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.0/src/gvec_to_python/testcases/ellipstell/newBC_E1D6_M6N6/GVEC_ELLIPSTELL_E1D6_M6N6_State_0000_00200000.dat` & `gvec-to-python-1.1.1/src/gvec_to_python/testcases/ellipstell/newBC_E1D6_M6N6/GVEC_ELLIPSTELL_E1D6_M6N6_State_0000_00200000.dat`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.0/src/gvec_to_python/testcases/ellipstell/newBC_E1D6_M6N6/parameter.ini` & `gvec-to-python-1.1.1/src/gvec_to_python/testcases/ellipstell/newBC_E1D6_M6N6/parameter.ini`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.0/src/gvec_to_python/testcases/ellipstell/newBC_E4D6_M6N6/GVEC_ELLIPSTELL_E4D6_M6N6_State_0001_00200000.dat` & `gvec-to-python-1.1.1/src/gvec_to_python/testcases/ellipstell/newBC_E4D6_M6N6/GVEC_ELLIPSTELL_E4D6_M6N6_State_0001_00200000.dat`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.0/src/gvec_to_python/testcases/ellipstell/newBC_E4D6_M6N6/parameter.ini` & `gvec-to-python-1.1.1/src/gvec_to_python/testcases/ellipstell/newBC_E4D6_M6N6/parameter.ini`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.0/src/gvec_to_python/testcases/ellipstell_v2/newBC_E1D6_M6N6/GVEC_ELLIPSTELL_V2_State_0000_00200000.dat` & `gvec-to-python-1.1.1/src/gvec_to_python/testcases/ellipstell_v2/newBC_E1D6_M6N6/GVEC_ELLIPSTELL_V2_State_0000_00200000.dat`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.0/src/gvec_to_python/testcases/ellipstell_v2/newBC_E1D6_M6N6/parameter.ini` & `gvec-to-python-1.1.1/src/gvec_to_python/testcases/ellipstell_v2/newBC_E1D6_M6N6/parameter.ini`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.0/src/gvec_to_python/testcases/ellipstell_v2/newBC_E4D6_M6N6/GVEC_ELLIPSTELL_V2_State_0000_00200000.dat` & `gvec-to-python-1.1.1/src/gvec_to_python/testcases/ellipstell_v2/newBC_E4D6_M6N6/GVEC_ELLIPSTELL_V2_State_0000_00200000.dat`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.0/src/gvec_to_python/testcases/ellipstell_v2/newBC_E4D6_M6N6/parameter.ini` & `gvec-to-python-1.1.1/src/gvec_to_python/testcases/ellipstell_v2/newBC_E4D6_M6N6/parameter.ini`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.0/src/gvec_to_python/testcases/ellipstell_v2/oldBC_E40D5M6N6/GVEC_ELLIPSTELL_V2_State_0000_00200000.dat` & `gvec-to-python-1.1.1/src/gvec_to_python/testcases/ellipstell_v2/oldBC_E40D5M6N6/GVEC_ELLIPSTELL_V2_State_0000_00200000.dat`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.0/src/gvec_to_python/testcases/ellipstell_v2/oldBC_E40D5M6N6/parameter.ini` & `gvec-to-python-1.1.1/src/gvec_to_python/testcases/ellipstell_v2/oldBC_E40D5M6N6/parameter.ini`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.0/src/gvec_to_python/util/logger.py` & `gvec-to-python-1.1.1/src/gvec_to_python/util/logger.py`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.0/src/gvec_to_python/util/numpy_encoder.py` & `gvec-to-python-1.1.1/src/gvec_to_python/util/numpy_encoder.py`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.0/src/gvec_to_python/writer/paraview/mesh_creator.py` & `gvec-to-python-1.1.1/src/gvec_to_python/writer/paraview/mesh_creator.py`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.0/src/gvec_to_python/writer/paraview/vtk_writer.py` & `gvec-to-python-1.1.1/src/gvec_to_python/writer/paraview/vtk_writer.py`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.0/src/gvec_to_python.egg-info/PKG-INFO` & `gvec-to-python-1.1.1/src/gvec_to_python.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: gvec-to-python
-Version: 1.1.0
+Version: 1.1.1
 Summary: Parse GVEC output in Python
 Author: Tin Kei Cheng, Florian Hindenlang, Stefan Possanner
 Author-email: stefan.possanner@ipp.mpg.de, florian.hindenlang@ipp.mpg.de
-License: Copyright 2023 (c) T.K. Cheng, F. Hindenlang, S. Possanner | Max Planck Institute for Plasma Physics
+License: Copyright 2021 (c) T.K. Cheng, F. Hindenlang, S. Possanner | Max Planck Institute for Plasma Physics
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software 
         and associated documentation files (the "Software"), to deal in the Software without restriction, 
         including without limitation the rights to use, copy, modify, merge, publish, distribute, 
         sublicense, and/or sell copies of the Software, and to permit persons to whom the Software 
         is furnished to do so, subject to the following conditions:
         
@@ -16,41 +16,38 @@
         or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, 
         INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR 
         PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE 
         FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, 
         ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-Project-URL: homepage, https://gitlab.mpcdf.mpg.de/spossann/gvec_to_python
-Project-URL: documentation, https://readthedocs.org
-Project-URL: repository, https://github.com/me/spam.git
-Project-URL: changelog, https://github.com/me/spam/blob/master/CHANGELOG.md
-Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
+Project-URL: repository, https://gitlab.mpcdf.mpg.de/spossann/gvec_to_python
+Project-URL: Bug Tracker, https://gitlab.mpcdf.mpg.de/spossann/gvec_to_python/-/issues
 Keywords: plasma physics,fusion,numerical modeling,mhd equilibrium
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 3D GVEC equilibria in Python
 
-PyPI install (not yet :-):
+PyPI install:
 
 ```
 pip install gvec_to_python
 ```
 Or from source:
 ```
 git clone git@gitlab.mpcdf.mpg.de:spossann/gvec_to_python.git
 cd gvec_to_python
 pip install -e .
 ```
 Compile kernels for faster evaluations:
 ```
-compile_gvec_to_python
+compile-gvec-tp
 ```
 
 # Usage
 
 The [Galerkin Variational Equilibrium Code (GVEC)](https://gitlab.mpcdf.mpg.de/gvec-group/gvec) calculates magneto-hydrodynamic (MHD) equilibria for Tokamaks and Stellarators. `gvec_to_python` parses the GVEC output file (`.dat`) and collects the data in a `.json` file: 
 ```
 from gvec_to_python.reader.gvec_reader import create_GVEC_json
```

### Comparing `gvec-to-python-1.1.0/tests/test_gvec_domain.py` & `gvec-to-python-1.1.1/tests/test_gvec_domain.py`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.0/tests/test_gvec_equil.py` & `gvec-to-python-1.1.1/tests/test_gvec_equil.py`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.0/tests/test_gvec_profiles.py` & `gvec-to-python-1.1.1/tests/test_gvec_profiles.py`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.0/tests/test_splines.py` & `gvec-to-python-1.1.1/tests/test_splines.py`

 * *Files identical despite different names*

