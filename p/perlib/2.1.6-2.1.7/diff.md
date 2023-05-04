# Comparing `tmp/perlib-2.1.6.tar.gz` & `tmp/perlib-2.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perlib-2.1.6.tar", last modified: Fri Apr 28 16:59:45 2023, max compression
+gzip compressed data, was "perlib-2.1.7.tar", last modified: Thu May  4 14:00:45 2023, max compression
```

## Comparing `perlib-2.1.6.tar` & `perlib-2.1.7.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 16:59:45.566769 perlib-2.1.6/
--rw-rw-rw-   0        0        0    11558 2023-04-04 21:29:00.000000 perlib-2.1.6/LICENSE.md
--rw-rw-rw-   0        0        0    10622 2023-04-28 16:59:45.566769 perlib-2.1.6/PKG-INFO
--rw-rw-rw-   0        0        0    10025 2023-04-04 21:32:21.000000 perlib-2.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-28 16:59:45.451923 perlib-2.1.6/perlib/
--rw-rw-rw-   0        0        0      922 2023-04-28 16:57:08.000000 perlib-2.1.6/perlib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-28 16:59:45.466502 perlib-2.1.6/perlib/analysis/
--rw-rw-rw-   0        0        0      131 2023-04-04 21:29:00.000000 perlib-2.1.6/perlib/analysis/__init__.py
--rw-rw-rw-   0        0        0      863 2023-04-04 21:29:00.000000 perlib-2.1.6/perlib/analysis/exceptions.py
--rw-rw-rw-   0        0        0     5664 2023-04-04 21:29:00.000000 perlib-2.1.6/perlib/analysis/multivariate.py
--rw-rw-rw-   0        0        0    10432 2023-04-04 21:29:00.000000 perlib-2.1.6/perlib/analysis/plotting.py
--rw-rw-rw-   0        0        0     8015 2023-04-04 21:29:00.000000 perlib-2.1.6/perlib/analysis/univariate.py
--rw-rw-rw-   0        0        0     3208 2023-04-04 21:29:00.000000 perlib-2.1.6/perlib/analysis/validate.py
-drwxrwxrwx   0        0        0        0 2023-04-28 16:59:45.472019 perlib-2.1.6/perlib/api/
--rw-rw-rw-   0        0        0       25 2023-04-04 21:29:00.000000 perlib-2.1.6/perlib/api/__init__.py
--rw-rw-rw-   0        0        0      198 2023-04-04 21:29:00.000000 perlib-2.1.6/perlib/api/api.py
-drwxrwxrwx   0        0        0        0 2023-04-28 16:59:45.482055 perlib-2.1.6/perlib/core/
--rw-rw-rw-   0        0        0      454 2023-04-04 21:29:00.000000 perlib-2.1.6/perlib/core/__init__.py
--rw-rw-rw-   0        0        0     3740 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/core/_requests.py
-drwxrwxrwx   0        0        0        0 2023-04-28 16:59:45.489653 perlib-2.1.6/perlib/core/metrics/
--rw-rw-rw-   0        0        0       56 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/core/metrics/__init__.py
--rw-rw-rw-   0        0        0    90017 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/core/metrics/classification.py
--rw-rw-rw-   0        0        0    21214 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/core/metrics/regression.py
-drwxrwxrwx   0        0        0        0 2023-04-28 16:59:45.501964 perlib-2.1.6/perlib/core/models/
--rw-rw-rw-   0        0        0       25 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/core/models/__init__.py
--rw-rw-rw-   0        0        0     4843 2023-04-04 22:12:52.000000 perlib-2.1.6/perlib/core/models/dmodels.py
--rw-rw-rw-   0        0        0     2601 2023-04-27 08:45:32.000000 perlib-2.1.6/perlib/core/models/elm.py
--rw-rw-rw-   0        0        0     7819 2023-04-04 22:13:07.000000 perlib-2.1.6/perlib/core/models/lstnet.py
--rw-rw-rw-   0        0        0     2581 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/core/models/mmodels.py
--rw-rw-rw-   0        0        0     2302 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/core/models/smodels.py
-drwxrwxrwx   0        0        0        0 2023-04-28 16:59:45.505483 perlib-2.1.6/perlib/core/optimizers/
--rw-rw-rw-   0        0        0    32659 2023-04-04 21:52:50.000000 perlib-2.1.6/perlib/core/optimizers/Optimizers.py
--rw-rw-rw-   0        0        0       25 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/core/optimizers/__init__.py
--rw-rw-rw-   0        0        0    11950 2023-04-26 13:57:44.000000 perlib-2.1.6/perlib/core/req_utils.py
--rw-rw-rw-   0        0        0    13165 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/core/tester.py
--rw-rw-rw-   0        0        0    20205 2023-04-28 16:52:41.000000 perlib-2.1.6/perlib/core/train.py
-drwxrwxrwx   0        0        0        0 2023-04-28 16:59:45.522002 perlib-2.1.6/perlib/datasets/
--rw-rw-rw-   0        0        0      273 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/datasets/__init__.py
--rw-rw-rw-   0        0        0     3158 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/datasets/airpassengers.py
--rw-rw-rw-   0        0        0     5263 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/datasets/ausbeer.py
--rw-rw-rw-   0        0        0     3337 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/datasets/austres.py
--rw-rw-rw-   0        0        0     4709 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/datasets/heartrate.py
--rw-rw-rw-   0        0        0     3515 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/datasets/lynx.py
--rw-rw-rw-   0        0        0    36115 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/datasets/taylor.py
--rw-rw-rw-   0        0        0     4820 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/datasets/wineind.py
--rw-rw-rw-   0        0        0     3645 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/datasets/woolyrnq.py
--rw-rw-rw-   0        0        0    11981 2023-04-05 07:46:38.000000 perlib-2.1.6/perlib/forecaster.py
-drwxrwxrwx   0        0        0        0 2023-04-28 16:59:45.531943 perlib-2.1.6/perlib/piplines/
--rw-rw-rw-   0        0        0        0 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/piplines/__init__.py
--rw-rw-rw-   0        0        0     3450 2023-04-04 22:58:03.000000 perlib-2.1.6/perlib/piplines/dpipline.py
--rw-rw-rw-   0        0        0    21347 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/piplines/mpipline.py
-drwxrwxrwx   0        0        0        0 2023-04-28 16:59:45.552153 perlib-2.1.6/perlib/preprocessing/
--rw-rw-rw-   0        0        0     5447 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/preprocessing/Normalizing.py
--rw-rw-rw-   0        0        0      241 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/preprocessing/__init__.py
--rw-rw-rw-   0        0        0     9739 2023-04-28 16:40:53.000000 perlib-2.1.6/perlib/preprocessing/_split.py
-drwxrwxrwx   0        0        0        0 2023-04-28 16:59:45.566769 perlib-2.1.6/perlib/preprocessing/_utils/
--rw-rw-rw-   0        0        0      111 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/preprocessing/_utils/__init__.py
--rw-rw-rw-   0        0        0     8551 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/preprocessing/_utils/dataframe.py
--rw-rw-rw-   0        0        0    27299 2023-04-12 17:23:29.000000 perlib-2.1.6/perlib/preprocessing/_utils/dataset_utils.py
--rw-rw-rw-   0        0        0     9766 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/preprocessing/_utils/timeseries_dataset.py
--rw-rw-rw-   0        0        0    12153 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/preprocessing/_utils/tools.py
--rw-rw-rw-   0        0        0    13496 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/preprocessing/autopreprocess.py
--rw-rw-rw-   0        0        0     4491 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/preprocessing/encode.py
--rw-rw-rw-   0        0        0    13956 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/preprocessing/imputer.py
--rw-rw-rw-   0        0        0     3446 2023-04-04 21:29:01.000000 perlib-2.1.6/perlib/preprocessing/outliers.py
--rw-rw-rw-   0        0        0    19319 2023-04-13 12:15:50.000000 perlib-2.1.6/perlib/preprocessing/preparate.py
-drwxrwxrwx   0        0        0        0 2023-04-28 16:59:45.457435 perlib-2.1.6/perlib.egg-info/
--rw-rw-rw-   0        0        0    10622 2023-04-28 16:59:45.000000 perlib-2.1.6/perlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1719 2023-04-28 16:59:45.000000 perlib-2.1.6/perlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 16:59:45.000000 perlib-2.1.6/perlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      143 2023-04-28 16:59:45.000000 perlib-2.1.6/perlib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-28 16:59:45.000000 perlib-2.1.6/perlib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-28 16:59:45.566769 perlib-2.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1682 2023-04-04 21:29:01.000000 perlib-2.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 14:00:45.237763 perlib-2.1.7/
+-rw-rw-rw-   0        0        0    11558 2023-04-04 21:29:00.000000 perlib-2.1.7/LICENSE.md
+-rw-rw-rw-   0        0        0    10622 2023-05-04 14:00:45.237763 perlib-2.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0    10025 2023-04-04 21:32:21.000000 perlib-2.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 14:00:45.143610 perlib-2.1.7/perlib/
+-rw-rw-rw-   0        0        0      922 2023-05-04 14:00:24.000000 perlib-2.1.7/perlib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 14:00:45.159234 perlib-2.1.7/perlib/analysis/
+-rw-rw-rw-   0        0        0      131 2023-04-04 21:29:00.000000 perlib-2.1.7/perlib/analysis/__init__.py
+-rw-rw-rw-   0        0        0      863 2023-04-04 21:29:00.000000 perlib-2.1.7/perlib/analysis/exceptions.py
+-rw-rw-rw-   0        0        0     5664 2023-04-04 21:29:00.000000 perlib-2.1.7/perlib/analysis/multivariate.py
+-rw-rw-rw-   0        0        0    10432 2023-04-04 21:29:00.000000 perlib-2.1.7/perlib/analysis/plotting.py
+-rw-rw-rw-   0        0        0     8015 2023-04-04 21:29:00.000000 perlib-2.1.7/perlib/analysis/univariate.py
+-rw-rw-rw-   0        0        0     3208 2023-04-04 21:29:00.000000 perlib-2.1.7/perlib/analysis/validate.py
+drwxrwxrwx   0        0        0        0 2023-05-04 14:00:45.159234 perlib-2.1.7/perlib/api/
+-rw-rw-rw-   0        0        0       25 2023-04-04 21:29:00.000000 perlib-2.1.7/perlib/api/__init__.py
+-rw-rw-rw-   0        0        0      198 2023-04-04 21:29:00.000000 perlib-2.1.7/perlib/api/api.py
+drwxrwxrwx   0        0        0        0 2023-05-04 14:00:45.174861 perlib-2.1.7/perlib/core/
+-rw-rw-rw-   0        0        0      454 2023-04-04 21:29:00.000000 perlib-2.1.7/perlib/core/__init__.py
+-rw-rw-rw-   0        0        0     3806 2023-05-04 08:47:33.000000 perlib-2.1.7/perlib/core/_requests.py
+drwxrwxrwx   0        0        0        0 2023-05-04 14:00:45.190486 perlib-2.1.7/perlib/core/metrics/
+-rw-rw-rw-   0        0        0       56 2023-04-04 21:29:01.000000 perlib-2.1.7/perlib/core/metrics/__init__.py
+-rw-rw-rw-   0        0        0    90017 2023-04-04 21:29:01.000000 perlib-2.1.7/perlib/core/metrics/classification.py
+-rw-rw-rw-   0        0        0    21214 2023-04-04 21:29:01.000000 perlib-2.1.7/perlib/core/metrics/regression.py
+drwxrwxrwx   0        0        0        0 2023-05-04 14:00:45.190486 perlib-2.1.7/perlib/core/models/
+-rw-rw-rw-   0        0        0       25 2023-04-04 21:29:01.000000 perlib-2.1.7/perlib/core/models/__init__.py
+-rw-rw-rw-   0        0        0     4843 2023-04-04 22:12:52.000000 perlib-2.1.7/perlib/core/models/dmodels.py
+-rw-rw-rw-   0        0        0     2601 2023-04-27 08:45:32.000000 perlib-2.1.7/perlib/core/models/elm.py
+-rw-rw-rw-   0        0        0     7819 2023-04-04 22:13:07.000000 perlib-2.1.7/perlib/core/models/lstnet.py
+-rw-rw-rw-   0        0        0     1130 2023-05-04 13:58:25.000000 perlib-2.1.7/perlib/core/models/mmodels.py
+-rw-rw-rw-   0        0        0     2302 2023-04-04 21:29:01.000000 perlib-2.1.7/perlib/core/models/smodels.py
+drwxrwxrwx   0        0        0        0 2023-05-04 14:00:45.206504 perlib-2.1.7/perlib/core/optimizers/
+-rw-rw-rw-   0        0        0    32659 2023-04-04 21:52:50.000000 perlib-2.1.7/perlib/core/optimizers/Optimizers.py
+-rw-rw-rw-   0        0        0       25 2023-04-04 21:29:01.000000 perlib-2.1.7/perlib/core/optimizers/__init__.py
+-rw-rw-rw-   0        0        0    11950 2023-04-26 13:57:44.000000 perlib-2.1.7/perlib/core/req_utils.py
+-rw-rw-rw-   0        0        0    13165 2023-04-04 21:29:01.000000 perlib-2.1.7/perlib/core/tester.py
+-rw-rw-rw-   0        0        0    20138 2023-05-04 13:58:32.000000 perlib-2.1.7/perlib/core/train.py
+drwxrwxrwx   0        0        0        0 2023-05-04 14:00:45.222139 perlib-2.1.7/perlib/datasets/
+-rw-rw-rw-   0        0        0      273 2023-04-04 21:29:01.000000 perlib-2.1.7/perlib/datasets/__init__.py
+-rw-rw-rw-   0        0        0     3158 2023-04-04 21:29:01.000000 perlib-2.1.7/perlib/datasets/airpassengers.py
+-rw-rw-rw-   0        0        0     5263 2023-04-04 21:29:01.000000 perlib-2.1.7/perlib/datasets/ausbeer.py
+-rw-rw-rw-   0        0        0     3337 2023-04-04 21:29:01.000000 perlib-2.1.7/perlib/datasets/austres.py
+-rw-rw-rw-   0        0        0     4709 2023-04-04 21:29:01.000000 perlib-2.1.7/perlib/datasets/heartrate.py
+-rw-rw-rw-   0        0        0     3515 2023-04-04 21:29:01.000000 perlib-2.1.7/perlib/datasets/lynx.py
+-rw-rw-rw-   0        0        0    36115 2023-04-04 21:29:01.000000 perlib-2.1.7/perlib/datasets/taylor.py
+-rw-rw-rw-   0        0        0     4820 2023-04-04 21:29:01.000000 perlib-2.1.7/perlib/datasets/wineind.py
+-rw-rw-rw-   0        0        0     3645 2023-04-04 21:29:01.000000 perlib-2.1.7/perlib/datasets/woolyrnq.py
+-rw-rw-rw-   0        0        0    11981 2023-04-05 07:46:38.000000 perlib-2.1.7/perlib/forecaster.py
+drwxrwxrwx   0        0        0        0 2023-05-04 14:00:45.222139 perlib-2.1.7/perlib/piplines/
+-rw-rw-rw-   0        0        0        0 2023-04-04 21:29:01.000000 perlib-2.1.7/perlib/piplines/__init__.py
+-rw-rw-rw-   0        0        0     3450 2023-04-04 22:58:03.000000 perlib-2.1.7/perlib/piplines/dpipline.py
+-rw-rw-rw-   0        0        0    21795 2023-05-04 13:49:39.000000 perlib-2.1.7/perlib/piplines/mpipline.py
+drwxrwxrwx   0        0        0        0 2023-05-04 14:00:45.237763 perlib-2.1.7/perlib/preprocessing/
+-rw-rw-rw-   0        0        0     5447 2023-04-04 21:29:01.000000 perlib-2.1.7/perlib/preprocessing/Normalizing.py
+-rw-rw-rw-   0        0        0      241 2023-04-04 21:29:01.000000 perlib-2.1.7/perlib/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0     9753 2023-05-04 10:06:09.000000 perlib-2.1.7/perlib/preprocessing/_split.py
+drwxrwxrwx   0        0        0        0 2023-05-04 14:00:45.237763 perlib-2.1.7/perlib/preprocessing/_utils/
+-rw-rw-rw-   0        0        0      111 2023-04-04 21:29:01.000000 perlib-2.1.7/perlib/preprocessing/_utils/__init__.py
+-rw-rw-rw-   0        0        0     8551 2023-04-04 21:29:01.000000 perlib-2.1.7/perlib/preprocessing/_utils/dataframe.py
+-rw-rw-rw-   0        0        0    27299 2023-04-12 17:23:29.000000 perlib-2.1.7/perlib/preprocessing/_utils/dataset_utils.py
+-rw-rw-rw-   0        0        0     9766 2023-04-04 21:29:01.000000 perlib-2.1.7/perlib/preprocessing/_utils/timeseries_dataset.py
+-rw-rw-rw-   0        0        0    12153 2023-04-04 21:29:01.000000 perlib-2.1.7/perlib/preprocessing/_utils/tools.py
+-rw-rw-rw-   0        0        0    13496 2023-04-04 21:29:01.000000 perlib-2.1.7/perlib/preprocessing/autopreprocess.py
+-rw-rw-rw-   0        0        0     4491 2023-04-04 21:29:01.000000 perlib-2.1.7/perlib/preprocessing/encode.py
+-rw-rw-rw-   0        0        0    13956 2023-04-04 21:29:01.000000 perlib-2.1.7/perlib/preprocessing/imputer.py
+-rw-rw-rw-   0        0        0     3446 2023-04-04 21:29:01.000000 perlib-2.1.7/perlib/preprocessing/outliers.py
+-rw-rw-rw-   0        0        0    19325 2023-05-04 13:51:58.000000 perlib-2.1.7/perlib/preprocessing/preparate.py
+drwxrwxrwx   0        0        0        0 2023-05-04 14:00:45.143610 perlib-2.1.7/perlib.egg-info/
+-rw-rw-rw-   0        0        0    10622 2023-05-04 14:00:45.000000 perlib-2.1.7/perlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1719 2023-05-04 14:00:45.000000 perlib-2.1.7/perlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 14:00:45.000000 perlib-2.1.7/perlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      143 2023-05-04 14:00:45.000000 perlib-2.1.7/perlib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-04 14:00:45.000000 perlib-2.1.7/perlib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 14:00:45.237763 perlib-2.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1682 2023-04-04 21:29:01.000000 perlib-2.1.7/setup.py
```

### Comparing `perlib-2.1.6/LICENSE.md` & `perlib-2.1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `perlib-2.1.6/PKG-INFO` & `perlib-2.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perlib
-Version: 2.1.6
+Version: 2.1.7
 Summary: Deep learning, Machine learning and Statistical learning for humans.
 Home-page: https://github.com/Ruzzg/perlib
 Author: Rüzgar Ersin Kanar
 Author-email: ruzgarknr@gmail.com
 License: Apache Software License
 Keywords: perlib,tensorflow,machine learning,deep learning
 Platform: UNKNOWN
```

### Comparing `perlib-2.1.6/README.md` & `perlib-2.1.7/README.md`

 * *Files identical despite different names*

### Comparing `perlib-2.1.6/perlib/__init__.py` & `perlib-2.1.7/perlib/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Bu projenin tüm hakları Rüzgar Ersin Kanar'a aittir. Harici kimse ticari amaçlı kullanamaz.
-__version__ = "2.1.6"
+__version__ = "2.1.7"
 from .forecaster import *
 from .core._requests import req_info,aR_info,m_info
 from .core.models.dmodels import models as dmodels
 from .core.models.mmodels import models as mmodels
 from .core.models.smodels import models as smodels
 from .core.train import dTrain,sTrain,mTrain
 from .core.tester import dTester,sTester
```

### Comparing `perlib-2.1.6/perlib/analysis/exceptions.py` & `perlib-2.1.7/perlib/analysis/exceptions.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.6/perlib/analysis/multivariate.py` & `perlib-2.1.7/perlib/analysis/multivariate.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.6/perlib/analysis/plotting.py` & `perlib-2.1.7/perlib/analysis/plotting.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.6/perlib/analysis/univariate.py` & `perlib-2.1.7/perlib/analysis/univariate.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.6/perlib/analysis/validate.py` & `perlib-2.1.7/perlib/analysis/validate.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.6/perlib/core/_requests.py` & `perlib-2.1.7/perlib/core/_requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,26 +6,28 @@
     """
 
     def __init__(self,
                  y=None,
                  modelname="SVR",
                  scaler="minmax",
                  testsize=0.2,
+                 shuffle = True,
                  metric="mape",
                  modelparams=None,
                  auto=False,
                  forecastNumber=24,
                  forecastingStartDate=False,
 
                  ):
         self.y = y
         self.modelname = modelname
         self.modelparams = modelparams
         self.testsize = testsize
         self.scaler = scaler
+        self.shuffle = shuffle
         self.auto = auto
         self.forecastNumber = forecastNumber
         self.forecastingStartDate = forecastingStartDate
         self.metric              = metric
 
 class aR_info(object):
```

### Comparing `perlib-2.1.6/perlib/core/metrics/classification.py` & `perlib-2.1.7/perlib/core/metrics/classification.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.6/perlib/core/metrics/regression.py` & `perlib-2.1.7/perlib/core/metrics/regression.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.6/perlib/core/models/dmodels.py` & `perlib-2.1.7/perlib/core/models/dmodels.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.6/perlib/core/models/elm.py` & `perlib-2.1.7/perlib/core/models/elm.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.6/perlib/core/models/lstnet.py` & `perlib-2.1.7/perlib/core/models/lstnet.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.6/perlib/core/models/smodels.py` & `perlib-2.1.7/perlib/core/models/smodels.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.6/perlib/core/optimizers/Optimizers.py` & `perlib-2.1.7/perlib/core/optimizers/Optimizers.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.6/perlib/core/req_utils.py` & `perlib-2.1.7/perlib/core/req_utils.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.6/perlib/core/tester.py` & `perlib-2.1.7/perlib/core/tester.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.6/perlib/core/train.py` & `perlib-2.1.7/perlib/core/train.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,21 +74,18 @@
                             is_categorical_dtype(self.dataFrame[self.object.m_info.y]):
                         if hasattr(self.dataFrame[self.object.m_info.y], "cat"):
                             return Classifier
                 else:
                     if hasattr(self.dataFrame[self.object.m_info.y], "cat"):
                         return Classifier
                     return Regressor
-    def c_opt(self):
+    def c_opt(self,X_train, X_test, y_train, y_test):
         if self.object.m_info.auto:
             mod = self.check_mod()
-            model, predictions = mmodels.opt(dataFrame=self.dataFrame,
-                                             testsize=self.object.m_info.testsize,
-                                             y=self.object.m_info.y,
-                                             mod=mod)
+            model, predictions = mmodels.opt(X_train, X_test, y_train, y_test,mod=mod,scaler=self.pr.get_scaler(self.object.m_info.scaler))
             if model.shape[0] > 1:
                 try:
                     model = model.sort_values("Accuracy", ascending=False)
                 except:
                     model = model.sort_values("R-Squared", ascending=False)
                 print(model)
                 return model.head(1).index.tolist()[0]
@@ -129,15 +126,15 @@
             self.y = self.scalery.fit_transform(y)
         else:
             self.y=y
         return self.X,self.y,self.scalerX,self.scalery
 
     def _test_size(self,X,y):
         if self.object.m_info.testsize is not None:
-            X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=self.object.m_info.testsize)
+            X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=self.object.m_info.testsize,shuffle=self.object.m_info.shuffle)
             return X_train, X_test, y_train, y_test
         else:
             return X,None,y,None
 
 
     def tr(self):
         if self.check_dataFrame():
@@ -146,19 +143,19 @@
             remove_column = []
             for col in columns:
                 column = self.dataFrame.loc[:, self.dataFrame.columns.str.startswith(col)].select_dtypes(
                     "object").columns.tolist()
                 if len(column) != 0:
                     remove_column.extend(column)
             self.dataFrame = self.dataFrame.drop(remove_column, axis=1)
-            if self.object.m_info.auto:
-                self.object.m_info.modelname = self.c_opt()
             X,y = self.data_split_()
             X,y,scalerX,scalery =self._scaler(X,y)
             X_train, X_test, y_train, y_test  = self._test_size(X,y)
+            if self.object.m_info.auto:
+                self.object.m_info.modelname = self.c_opt(X_train, X_test, y_train, y_test)
             m = eval(self.object.m_info.modelname)
             return m,scalerX,scalery,X_train,X_test, y_train, y_test
 
     def fit(self):
         m,scalerX,scalery,X_train,X_test, y_train, y_test = self.tr()
         if self.object.m_info.modelparams:
             try:
@@ -204,16 +201,15 @@
         remove_column = []
         for col in columns:
             column = testData.loc[:, testData.columns.str.startswith(col)].select_dtypes(
                 "object").columns.tolist()
             if len(column) != 0:
                 remove_column.extend(column)
         testData = testData.drop(remove_column, axis=1)
-        preds = model.predict(self.scalerX.fit_transform(testData))
-        preds = preds.reshape(-1,1)
+        preds = model.predict(self.scalerX.transform(testData)).reshape(-1,1)
         inverse_data = self.scalery.inverse_transform(preds)
         predicts_data = pd.DataFrame(inverse_data,columns=["Predicts"])
         return predicts_data
 
 class sTrain:
     def __init__(self,
                  dataFrame: pd.DataFrame,
```

### Comparing `perlib-2.1.6/perlib/datasets/airpassengers.py` & `perlib-2.1.7/perlib/datasets/airpassengers.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.6/perlib/datasets/ausbeer.py` & `perlib-2.1.7/perlib/datasets/ausbeer.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.6/perlib/datasets/austres.py` & `perlib-2.1.7/perlib/datasets/austres.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.6/perlib/datasets/heartrate.py` & `perlib-2.1.7/perlib/datasets/heartrate.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.6/perlib/datasets/lynx.py` & `perlib-2.1.7/perlib/datasets/lynx.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.6/perlib/datasets/taylor.py` & `perlib-2.1.7/perlib/datasets/taylor.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.6/perlib/datasets/wineind.py` & `perlib-2.1.7/perlib/datasets/wineind.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.6/perlib/datasets/woolyrnq.py` & `perlib-2.1.7/perlib/datasets/woolyrnq.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.6/perlib/forecaster.py` & `perlib-2.1.7/perlib/forecaster.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.6/perlib/piplines/dpipline.py` & `perlib-2.1.7/perlib/piplines/dpipline.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.6/perlib/piplines/mpipline.py` & `perlib-2.1.7/perlib/piplines/mpipline.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
     "MultiTaskLasso",
     "MultiTaskLassoCV",
     "PLSCanonical",
     "PLSRegression",
     "RadiusNeighborsRegressor",
     "RegressorChain",
     "VotingRegressor",
+    "QuantileRegressor"
 ]
 
 
 
 
 CLASSIFIERS = [
     est
@@ -82,17 +83,19 @@
 REGRESSORS.append(('MLPRegressor',sklearn.neural_network._multilayer_perceptron.MLPRegressor))
 
 CLASSIFIERS.append(("XGBClassifier", xgboost.XGBClassifier))
 CLASSIFIERS.append(("LGBMClassifier", lightgbm.LGBMClassifier))
 CLASSIFIERS.append(('CatBoostClassifier',catboost.CatBoostClassifier))
 CLASSIFIERS.append(('MLPClassifier',sklearn.neural_network._multilayer_perceptron.MLPClassifier))
 
-numeric_transformer = Pipeline(
-    steps=[("imputer", SimpleImputer(strategy="mean")), ("scaler", StandardScaler())]
-)
+
+
+#numeric_transformer = Pipeline(
+#    steps=[("imputer", SimpleImputer(strategy="mean")), ("scaler", StandardScaler())]
+#)
 
 categorical_transformer_low = Pipeline(
     steps=[
         ("imputer", SimpleImputer(strategy="constant", fill_value="missing")),
         ("encoding", OneHotEncoder(handle_unknown="ignore", sparse=False)),
     ]
 )
@@ -158,22 +161,24 @@
         self,
         verbose=0,
         ignore_warnings=True,
         custom_metric=None,
         predictions=False,
         random_state=42,
         classifiers="all",
+        scaler = StandardScaler()
     ):
         self.verbose = verbose
         self.ignore_warnings = ignore_warnings
         self.custom_metric = custom_metric
         self.predictions = predictions
         self.models = {}
         self.random_state = random_state
         self.classifiers = classifiers
+        self.scaler = scaler
 
     def fit(self, X_train, X_test, y_train, y_test):
         """Fit Classification algorithms to X_train and y_train, predict and score on X_test, y_test.
         Parameters
         ----------
         X_train : array-like,
             Training vectors, where rows is the number of samples
@@ -212,14 +217,17 @@
         numeric_features = X_train.select_dtypes(include=[np.number]).columns
         categorical_features = X_train.select_dtypes(include=["object"]).columns
 
         categorical_low, categorical_high = get_card_split(
             X_train, categorical_features
         )
 
+        numeric_transformer = Pipeline(
+            steps=[("imputer", SimpleImputer(strategy="mean")), ("scaler", self.scaler)]
+        )
         preprocessor = ColumnTransformer(
             transformers=[
                 ("numeric", numeric_transformer, numeric_features),
                 ("categorical_low", categorical_transformer_low, categorical_low),
                 ("categorical_high", categorical_transformer_high, categorical_high),
             ]
         )
@@ -394,16 +402,19 @@
         self,
         verbose=0,
         ignore_warnings=True,
         custom_metric=None,
         predictions=False,
         random_state=42,
         regressors="all",
+        scaler = StandardScaler()
     ):
+
         self.verbose = verbose
+        self.scaler = scaler
         self.ignore_warnings = ignore_warnings
         self.custom_metric = custom_metric
         self.predictions = predictions
         self.models = {}
         self.random_state = random_state
         self.regressors = regressors
 
@@ -448,14 +459,17 @@
         numeric_features = X_train.select_dtypes(include=[np.number]).columns
         categorical_features = X_train.select_dtypes(include=["object"]).columns
 
         categorical_low, categorical_high = get_card_split(
             X_train, categorical_features
         )
 
+        numeric_transformer = Pipeline(
+            steps=[("imputer", SimpleImputer(strategy="mean")), ("scaler", self.scaler)]
+        )
         preprocessor = ColumnTransformer(
             transformers=[
                 ("numeric", numeric_transformer, numeric_features),
                 ("categorical_low", categorical_transformer_low, categorical_low),
                 ("categorical_high", categorical_transformer_high, categorical_high),
             ]
         )
```

### Comparing `perlib-2.1.6/perlib/preprocessing/Normalizing.py` & `perlib-2.1.7/perlib/preprocessing/Normalizing.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.6/perlib/preprocessing/_split.py` & `perlib-2.1.7/perlib/preprocessing/_split.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     'SlidingWindowForecastCV'
 ]
 
 
 def train_test_split(*arrays,
                      test_size=None,
                      train_size=None,
-                     random_state=None,
+                     random_state=123,
                      shuffle=False,
                      stratify=None
                      ):
     """Split arrays or matrices into sequential train and test subsets
     Creates train/test splits over endogenous arrays an optional exogenous
     arrays. This is a wrapper of scikit-learn's ``train_test_split`` that
     does not shuffle.
@@ -45,17 +45,17 @@
     splitting : list, length=2 * len(arrays)
         List containing train-test split of inputs.
     Examples
     --------
     """
     return tts(
         *arrays,
-        random_state=None,
-        shuffle=True,
-        stratify=None,
+        random_state=random_state,
+        shuffle=shuffle,
+        stratify=stratify,
         test_size=test_size,
         train_size=train_size)
 
 
 class BaseTSCrossValidator(BaseEstimator, metaclass=abc.ABCMeta):
     """Base class for time series cross validators
     Based on the scikit-learn base cross-validator with alterations to fit the
```

### Comparing `perlib-2.1.6/perlib/preprocessing/_utils/dataframe.py` & `perlib-2.1.7/perlib/preprocessing/_utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.6/perlib/preprocessing/_utils/dataset_utils.py` & `perlib-2.1.7/perlib/preprocessing/_utils/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.6/perlib/preprocessing/_utils/timeseries_dataset.py` & `perlib-2.1.7/perlib/preprocessing/_utils/timeseries_dataset.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.6/perlib/preprocessing/_utils/tools.py` & `perlib-2.1.7/perlib/preprocessing/_utils/tools.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.6/perlib/preprocessing/autopreprocess.py` & `perlib-2.1.7/perlib/preprocessing/autopreprocess.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.6/perlib/preprocessing/encode.py` & `perlib-2.1.7/perlib/preprocessing/encode.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.6/perlib/preprocessing/imputer.py` & `perlib-2.1.7/perlib/preprocessing/imputer.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.6/perlib/preprocessing/outliers.py` & `perlib-2.1.7/perlib/preprocessing/outliers.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.6/perlib/preprocessing/preparate.py` & `perlib-2.1.7/perlib/preprocessing/preparate.py`

 * *Files 1% similar despite different names*

```diff
@@ -373,20 +373,20 @@
                 dataFrame.loc[dataFrame[col] < 1, col] = np.nan
                 dataFrame = dataFrame.groupby(dataFrame.index.date).transform(lambda x: x.fillna(x.mean()))
         return dataFrame
 
 
     def get_scaler(self,scaler):
         scalers = {
-            "minmax": MinMaxScaler,
-            "standard": StandardScaler,
-            "maxabs": MaxAbsScaler,
-            "robust": RobustScaler,
+            "minmax": MinMaxScaler(),
+            "standard": StandardScaler(),
+            "maxabs": MaxAbsScaler(),
+            "robust": RobustScaler(),
         }
-        return scalers.get(scaler.lower())()
+        return scalers.get(scaler.lower())
 
     def inf_clean(self,dataFrame = None):
         if not isinstance(dataFrame, pd.DataFrame):
             raise ValueError("Must be dataframe.")
         return dataFrame.replace([np.inf, -np.inf], 0, inplace=True)
```

### Comparing `perlib-2.1.6/perlib.egg-info/PKG-INFO` & `perlib-2.1.7/perlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perlib
-Version: 2.1.6
+Version: 2.1.7
 Summary: Deep learning, Machine learning and Statistical learning for humans.
 Home-page: https://github.com/Ruzzg/perlib
 Author: Rüzgar Ersin Kanar
 Author-email: ruzgarknr@gmail.com
 License: Apache Software License
 Keywords: perlib,tensorflow,machine learning,deep learning
 Platform: UNKNOWN
```

### Comparing `perlib-2.1.6/perlib.egg-info/SOURCES.txt` & `perlib-2.1.7/perlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `perlib-2.1.6/setup.py` & `perlib-2.1.7/setup.py`

 * *Files identical despite different names*

