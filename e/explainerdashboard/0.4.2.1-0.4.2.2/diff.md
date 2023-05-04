# Comparing `tmp/explainerdashboard-0.4.2.1.tar.gz` & `tmp/explainerdashboard-0.4.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "explainerdashboard-0.4.2.1.tar", last modified: Sun Feb 19 21:13:51 2023, max compression
+gzip compressed data, was "explainerdashboard-0.4.2.2.tar", last modified: Thu May  4 07:30:33 2023, max compression
```

## Comparing `explainerdashboard-0.4.2.1.tar` & `explainerdashboard-0.4.2.2.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 21:13:51.915591 explainerdashboard-0.4.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-02-19 21:13:51.915591 explainerdashboard-0.4.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    28835 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 21:13:51.911591 explainerdashboard-0.4.2.1/explainerdashboard/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/explainerdashboard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 21:13:51.911591 explainerdashboard-0.4.2.1/explainerdashboard/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   155845 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/explainerdashboard/assets/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/explainerdashboard/assets/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    19256 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/explainerdashboard/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/explainerdashboard/custom.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 21:13:51.911591 explainerdashboard-0.4.2.1/explainerdashboard/dashboard_components/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/explainerdashboard/dashboard_components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   141545 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/explainerdashboard/dashboard_components/classifier_components.py
--rw-r--r--   0 runner    (1001) docker     (123)    64829 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/explainerdashboard/dashboard_components/composites.py
--rw-r--r--   0 runner    (1001) docker     (123)    21897 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/explainerdashboard/dashboard_components/connectors.py
--rw-r--r--   0 runner    (1001) docker     (123)    32702 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/explainerdashboard/dashboard_components/decisiontree_components.py
--rw-r--r--   0 runner    (1001) docker     (123)    63569 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/explainerdashboard/dashboard_components/overview_components.py
--rw-r--r--   0 runner    (1001) docker     (123)   106836 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/explainerdashboard/dashboard_components/regression_components.py
--rw-r--r--   0 runner    (1001) docker     (123)   142789 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/explainerdashboard/dashboard_components/shap_components.py
--rw-r--r--   0 runner    (1001) docker     (123)    34809 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/explainerdashboard/dashboard_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)   131505 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/explainerdashboard/dashboards.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 21:13:51.911591 explainerdashboard-0.4.2.1/explainerdashboard/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)    16766 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/explainerdashboard/datasets/titanic_test.csv
--rw-r--r--   0 runner    (1001) docker     (123)    56452 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/explainerdashboard/datasets/titanic_train.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/explainerdashboard/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    66498 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/explainerdashboard/explainer_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)   107784 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/explainerdashboard/explainer_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)   198359 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/explainerdashboard/explainers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 21:13:51.915591 explainerdashboard-0.4.2.1/explainerdashboard/static/
--rw-r--r--   0 runner    (1001) docker     (123)   155845 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/explainerdashboard/static/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    60089 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/explainerdashboard/static/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/explainerdashboard/static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     9317 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/explainerdashboard/to_html.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 21:13:51.911591 explainerdashboard-0.4.2.1/explainerdashboard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-02-19 21:13:51.000000 explainerdashboard-0.4.2.1/explainerdashboard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-02-19 21:13:51.000000 explainerdashboard-0.4.2.1/explainerdashboard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-19 21:13:51.000000 explainerdashboard-0.4.2.1/explainerdashboard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-02-19 21:13:51.000000 explainerdashboard-0.4.2.1/explainerdashboard.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-02-19 21:13:51.000000 explainerdashboard-0.4.2.1/explainerdashboard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-19 21:13:51.000000 explainerdashboard-0.4.2.1/explainerdashboard.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-02-19 21:13:51.915591 explainerdashboard-0.4.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 21:13:51.915591 explainerdashboard-0.4.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22347 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 21:13:51.915591 explainerdashboard-0.4.2.1/tests/hub/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/tests/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/tests/hub/test_hub.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/tests/hub/test_hub_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/tests/hub/test_hub_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 21:13:51.915591 explainerdashboard-0.4.2.1/tests/integration_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/tests/integration_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/tests/integration_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/tests/integration_tests/test_customdashboards.py
--rw-r--r--   0 runner    (1001) docker     (123)     6570 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/tests/integration_tests/test_dashboards.py
--rw-r--r--   0 runner    (1001) docker     (123)    10780 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/tests/test_boosting_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    14361 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/tests/test_catboost_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    14877 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/tests/test_catboost_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)    14898 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/tests/test_classifier_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7017 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/tests/test_classifier_explainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/tests/test_cv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/tests/test_dashboard_dumps.py
--rw-r--r--   0 runner    (1001) docker     (123)    10521 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/tests/test_decisiontrees.py
--rw-r--r--   0 runner    (1001) docker     (123)    10508 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/tests/test_externalsource.py
--rw-r--r--   0 runner    (1001) docker     (123)     9200 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/tests/test_linear_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    13661 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/tests/test_multiclass.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/tests/test_njobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/tests/test_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/tests/test_randomforest_explainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13223 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/tests/test_regression_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/tests/test_regression_explainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/tests/test_skorch_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-02-19 21:13:41.000000 explainerdashboard-0.4.2.1/tests/test_xgboost_treeviz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:30:33.050698 explainerdashboard-0.4.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-05-04 07:30:33.050698 explainerdashboard-0.4.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    28835 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:30:33.026697 explainerdashboard-0.4.2.2/explainerdashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/explainerdashboard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:30:33.030697 explainerdashboard-0.4.2.2/explainerdashboard/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   155845 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/explainerdashboard/assets/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/explainerdashboard/assets/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    19256 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/explainerdashboard/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/explainerdashboard/custom.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:30:33.034697 explainerdashboard-0.4.2.2/explainerdashboard/dashboard_components/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/explainerdashboard/dashboard_components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   141545 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/explainerdashboard/dashboard_components/classifier_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64829 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/explainerdashboard/dashboard_components/composites.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21897 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/explainerdashboard/dashboard_components/connectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32702 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/explainerdashboard/dashboard_components/decisiontree_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63569 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/explainerdashboard/dashboard_components/overview_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)   106836 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/explainerdashboard/dashboard_components/regression_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)   142789 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/explainerdashboard/dashboard_components/shap_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34809 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/explainerdashboard/dashboard_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)   131505 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/explainerdashboard/dashboards.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:30:33.038697 explainerdashboard-0.4.2.2/explainerdashboard/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)    16766 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/explainerdashboard/datasets/titanic_test.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    56452 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/explainerdashboard/datasets/titanic_train.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/explainerdashboard/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66498 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/explainerdashboard/explainer_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107784 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/explainerdashboard/explainer_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)   198359 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/explainerdashboard/explainers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:30:33.038697 explainerdashboard-0.4.2.2/explainerdashboard/static/
+-rw-r--r--   0 runner    (1001) docker     (123)   155845 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/explainerdashboard/static/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    60089 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/explainerdashboard/static/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/explainerdashboard/static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     9317 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/explainerdashboard/to_html.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:30:33.030697 explainerdashboard-0.4.2.2/explainerdashboard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-05-04 07:30:32.000000 explainerdashboard-0.4.2.2/explainerdashboard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-05-04 07:30:32.000000 explainerdashboard-0.4.2.2/explainerdashboard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 07:30:32.000000 explainerdashboard-0.4.2.2/explainerdashboard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-04 07:30:32.000000 explainerdashboard-0.4.2.2/explainerdashboard.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-04 07:30:32.000000 explainerdashboard-0.4.2.2/explainerdashboard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-04 07:30:32.000000 explainerdashboard-0.4.2.2/explainerdashboard.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-04 07:30:33.054698 explainerdashboard-0.4.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:30:33.046697 explainerdashboard-0.4.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22347 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:30:33.050698 explainerdashboard-0.4.2.2/tests/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/tests/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/tests/hub/test_hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/tests/hub/test_hub_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/tests/hub/test_hub_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:30:33.050698 explainerdashboard-0.4.2.2/tests/integration_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/tests/integration_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/tests/integration_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/tests/integration_tests/test_customdashboards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6570 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/tests/integration_tests/test_dashboards.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10780 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/tests/test_boosting_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14361 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/tests/test_catboost_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14877 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/tests/test_catboost_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14898 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/tests/test_classifier_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7017 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/tests/test_classifier_explainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/tests/test_cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/tests/test_dashboard_dumps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10521 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/tests/test_decisiontrees.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10508 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/tests/test_externalsource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9200 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/tests/test_linear_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13661 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/tests/test_multiclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/tests/test_njobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/tests/test_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/tests/test_randomforest_explainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13223 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/tests/test_regression_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/tests/test_regression_explainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/tests/test_skorch_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-05-04 07:30:20.000000 explainerdashboard-0.4.2.2/tests/test_xgboost_treeviz.py
```

### Comparing `explainerdashboard-0.4.2.1/LICENSE.txt` & `explainerdashboard-0.4.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `explainerdashboard-0.4.2.1/PKG-INFO` & `explainerdashboard-0.4.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: explainerdashboard
-Version: 0.4.2.1
+Version: 0.4.2.2
 Summary: Quickly build Explainable AI dashboards that show the inner workings of so-called "blackbox" machine learning models.
 Home-page: https://github.com/oegedijk/explainerdashboard
 Author: Oege Dijk
 Author-email: oegedijk@gmail.com
 License: MIT
 Project-URL: Github page, https://github.com/oegedijk/explainerdashboard/
 Project-URL: Documentation, https://explainerdashboard.readthedocs.io/
```

### Comparing `explainerdashboard-0.4.2.1/README.md` & `explainerdashboard-0.4.2.2/README.md`

 * *Files identical despite different names*

### Comparing `explainerdashboard-0.4.2.1/explainerdashboard/assets/bootstrap.min.css` & `explainerdashboard-0.4.2.2/explainerdashboard/assets/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `explainerdashboard-0.4.2.1/explainerdashboard/assets/favicon.ico` & `explainerdashboard-0.4.2.2/explainerdashboard/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `explainerdashboard-0.4.2.1/explainerdashboard/cli.py` & `explainerdashboard-0.4.2.2/explainerdashboard/cli.py`

 * *Files identical despite different names*

### Comparing `explainerdashboard-0.4.2.1/explainerdashboard/dashboard_components/classifier_components.py` & `explainerdashboard-0.4.2.2/explainerdashboard/dashboard_components/classifier_components.py`

 * *Files identical despite different names*

### Comparing `explainerdashboard-0.4.2.1/explainerdashboard/dashboard_components/composites.py` & `explainerdashboard-0.4.2.2/explainerdashboard/dashboard_components/composites.py`

 * *Files identical despite different names*

### Comparing `explainerdashboard-0.4.2.1/explainerdashboard/dashboard_components/connectors.py` & `explainerdashboard-0.4.2.2/explainerdashboard/dashboard_components/connectors.py`

 * *Files identical despite different names*

### Comparing `explainerdashboard-0.4.2.1/explainerdashboard/dashboard_components/decisiontree_components.py` & `explainerdashboard-0.4.2.2/explainerdashboard/dashboard_components/decisiontree_components.py`

 * *Files identical despite different names*

### Comparing `explainerdashboard-0.4.2.1/explainerdashboard/dashboard_components/overview_components.py` & `explainerdashboard-0.4.2.2/explainerdashboard/dashboard_components/overview_components.py`

 * *Files identical despite different names*

### Comparing `explainerdashboard-0.4.2.1/explainerdashboard/dashboard_components/regression_components.py` & `explainerdashboard-0.4.2.2/explainerdashboard/dashboard_components/regression_components.py`

 * *Files identical despite different names*

### Comparing `explainerdashboard-0.4.2.1/explainerdashboard/dashboard_components/shap_components.py` & `explainerdashboard-0.4.2.2/explainerdashboard/dashboard_components/shap_components.py`

 * *Files identical despite different names*

### Comparing `explainerdashboard-0.4.2.1/explainerdashboard/dashboard_methods.py` & `explainerdashboard-0.4.2.2/explainerdashboard/dashboard_methods.py`

 * *Files identical despite different names*

### Comparing `explainerdashboard-0.4.2.1/explainerdashboard/dashboards.py` & `explainerdashboard-0.4.2.2/explainerdashboard/dashboards.py`

 * *Files identical despite different names*

### Comparing `explainerdashboard-0.4.2.1/explainerdashboard/datasets/titanic_test.csv` & `explainerdashboard-0.4.2.2/explainerdashboard/datasets/titanic_test.csv`

 * *Files identical despite different names*

### Comparing `explainerdashboard-0.4.2.1/explainerdashboard/datasets/titanic_train.csv` & `explainerdashboard-0.4.2.2/explainerdashboard/datasets/titanic_train.csv`

 * *Files identical despite different names*

### Comparing `explainerdashboard-0.4.2.1/explainerdashboard/datasets.py` & `explainerdashboard-0.4.2.2/explainerdashboard/datasets.py`

 * *Files identical despite different names*

### Comparing `explainerdashboard-0.4.2.1/explainerdashboard/explainer_methods.py` & `explainerdashboard-0.4.2.2/explainerdashboard/explainer_methods.py`

 * *Files identical despite different names*

### Comparing `explainerdashboard-0.4.2.1/explainerdashboard/explainer_plots.py` & `explainerdashboard-0.4.2.2/explainerdashboard/explainer_plots.py`

 * *Files identical despite different names*

### Comparing `explainerdashboard-0.4.2.1/explainerdashboard/explainers.py` & `explainerdashboard-0.4.2.2/explainerdashboard/explainers.py`

 * *Files identical despite different names*

### Comparing `explainerdashboard-0.4.2.1/explainerdashboard/static/bootstrap.min.css` & `explainerdashboard-0.4.2.2/explainerdashboard/static/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `explainerdashboard-0.4.2.1/explainerdashboard/static/bootstrap.min.js` & `explainerdashboard-0.4.2.2/explainerdashboard/static/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `explainerdashboard-0.4.2.1/explainerdashboard/static/favicon.ico` & `explainerdashboard-0.4.2.2/explainerdashboard/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `explainerdashboard-0.4.2.1/explainerdashboard/to_html.py` & `explainerdashboard-0.4.2.2/explainerdashboard/to_html.py`

 * *Files identical despite different names*

### Comparing `explainerdashboard-0.4.2.1/explainerdashboard.egg-info/PKG-INFO` & `explainerdashboard-0.4.2.2/explainerdashboard.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: explainerdashboard
-Version: 0.4.2.1
+Version: 0.4.2.2
 Summary: Quickly build Explainable AI dashboards that show the inner workings of so-called "blackbox" machine learning models.
 Home-page: https://github.com/oegedijk/explainerdashboard
 Author: Oege Dijk
 Author-email: oegedijk@gmail.com
 License: MIT
 Project-URL: Github page, https://github.com/oegedijk/explainerdashboard/
 Project-URL: Documentation, https://explainerdashboard.readthedocs.io/
```

### Comparing `explainerdashboard-0.4.2.1/explainerdashboard.egg-info/SOURCES.txt` & `explainerdashboard-0.4.2.2/explainerdashboard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `explainerdashboard-0.4.2.1/setup.py` & `explainerdashboard-0.4.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("requirements.txt", "rt") as requirements_file:
     requirements = list(filter(None, map(str.strip,
                                          requirements_file.readlines())))
 
 setup(
     name='explainerdashboard',
-    version='0.4.2.1',
+    version='0.4.2.2',
     description='Quickly build Explainable AI dashboards that show the inner workings of so-called "blackbox" machine learning models.',
     long_description="""
 
 This package makes it convenient to quickly deploy a dashboard web app
 that explains the workings of a (scikit-learn compatible) fitted machine 
 learning model. The dashboard provides interactive plots on model performance, 
 feature importances, feature contributions to individual predictions,
```

### Comparing `explainerdashboard-0.4.2.1/tests/conftest.py` & `explainerdashboard-0.4.2.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `explainerdashboard-0.4.2.1/tests/hub/test_hub.py` & `explainerdashboard-0.4.2.2/tests/hub/test_hub.py`

 * *Files identical despite different names*

### Comparing `explainerdashboard-0.4.2.1/tests/hub/test_hub_integration.py` & `explainerdashboard-0.4.2.2/tests/hub/test_hub_integration.py`

 * *Files identical despite different names*

### Comparing `explainerdashboard-0.4.2.1/tests/integration_tests/test_customdashboards.py` & `explainerdashboard-0.4.2.2/tests/integration_tests/test_customdashboards.py`

 * *Files identical despite different names*

### Comparing `explainerdashboard-0.4.2.1/tests/integration_tests/test_dashboards.py` & `explainerdashboard-0.4.2.2/tests/integration_tests/test_dashboards.py`

 * *Files identical despite different names*

### Comparing `explainerdashboard-0.4.2.1/tests/test_boosting_models.py` & `explainerdashboard-0.4.2.2/tests/test_boosting_models.py`

 * *Files identical despite different names*

### Comparing `explainerdashboard-0.4.2.1/tests/test_catboost_classifier.py` & `explainerdashboard-0.4.2.2/tests/test_catboost_classifier.py`

 * *Files identical despite different names*

### Comparing `explainerdashboard-0.4.2.1/tests/test_catboost_regression.py` & `explainerdashboard-0.4.2.2/tests/test_catboost_regression.py`

 * *Files identical despite different names*

### Comparing `explainerdashboard-0.4.2.1/tests/test_classifier_base.py` & `explainerdashboard-0.4.2.2/tests/test_classifier_base.py`

 * *Files identical despite different names*

### Comparing `explainerdashboard-0.4.2.1/tests/test_classifier_explainer.py` & `explainerdashboard-0.4.2.2/tests/test_classifier_explainer.py`

 * *Files identical despite different names*

### Comparing `explainerdashboard-0.4.2.1/tests/test_cli.py` & `explainerdashboard-0.4.2.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `explainerdashboard-0.4.2.1/tests/test_cv.py` & `explainerdashboard-0.4.2.2/tests/test_cv.py`

 * *Files identical despite different names*

### Comparing `explainerdashboard-0.4.2.1/tests/test_dashboard_dumps.py` & `explainerdashboard-0.4.2.2/tests/test_dashboard_dumps.py`

 * *Files identical despite different names*

### Comparing `explainerdashboard-0.4.2.1/tests/test_decisiontrees.py` & `explainerdashboard-0.4.2.2/tests/test_decisiontrees.py`

 * *Files identical despite different names*

### Comparing `explainerdashboard-0.4.2.1/tests/test_externalsource.py` & `explainerdashboard-0.4.2.2/tests/test_externalsource.py`

 * *Files identical despite different names*

### Comparing `explainerdashboard-0.4.2.1/tests/test_linear_model.py` & `explainerdashboard-0.4.2.2/tests/test_linear_model.py`

 * *Files identical despite different names*

### Comparing `explainerdashboard-0.4.2.1/tests/test_multiclass.py` & `explainerdashboard-0.4.2.2/tests/test_multiclass.py`

 * *Files identical despite different names*

### Comparing `explainerdashboard-0.4.2.1/tests/test_njobs.py` & `explainerdashboard-0.4.2.2/tests/test_njobs.py`

 * *Files identical despite different names*

### Comparing `explainerdashboard-0.4.2.1/tests/test_pipelines.py` & `explainerdashboard-0.4.2.2/tests/test_pipelines.py`

 * *Files identical despite different names*

### Comparing `explainerdashboard-0.4.2.1/tests/test_randomforest_explainer.py` & `explainerdashboard-0.4.2.2/tests/test_randomforest_explainer.py`

 * *Files identical despite different names*

### Comparing `explainerdashboard-0.4.2.1/tests/test_regression_base.py` & `explainerdashboard-0.4.2.2/tests/test_regression_base.py`

 * *Files identical despite different names*

### Comparing `explainerdashboard-0.4.2.1/tests/test_regression_explainer.py` & `explainerdashboard-0.4.2.2/tests/test_regression_explainer.py`

 * *Files identical despite different names*

### Comparing `explainerdashboard-0.4.2.1/tests/test_skorch_models.py` & `explainerdashboard-0.4.2.2/tests/test_skorch_models.py`

 * *Files identical despite different names*

### Comparing `explainerdashboard-0.4.2.1/tests/test_xgboost_treeviz.py` & `explainerdashboard-0.4.2.2/tests/test_xgboost_treeviz.py`

 * *Files identical despite different names*

