# Comparing `tmp/sasctl-1.9.0.tar.gz` & `tmp/sasctl-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sasctl-1.9.0.tar", last modified: Wed Apr  5 12:53:46 2023, max compression
+gzip compressed data, was "sasctl-1.9.1.tar", last modified: Thu May  4 13:12:07 2023, max compression
```

## Comparing `sasctl-1.9.0.tar` & `sasctl-1.9.1.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:53:46.321592 sasctl-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)    17577 2023-04-05 12:53:34.000000 sasctl-1.9.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-04-05 12:53:34.000000 sasctl-1.9.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-04-05 12:53:34.000000 sasctl-1.9.0/ContributorAgreement.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-05 12:53:34.000000 sasctl-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-05 12:53:34.000000 sasctl-1.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11136 2023-04-05 12:53:46.321592 sasctl-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9790 2023-04-05 12:53:34.000000 sasctl-1.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-05 12:53:34.000000 sasctl-1.9.0/SUPPORT.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 12:53:46.321592 sasctl-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-04-05 12:53:34.000000 sasctl-1.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:53:46.293590 sasctl-1.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:53:46.301591 sasctl-1.9.0/src/sasctl/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:53:46.309591 sasctl-1.9.0/src/sasctl/_services/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/_services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19546 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/_services/cas_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/_services/concepts.py
--rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/_services/data_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/_services/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/_services/folders.py
--rw-r--r--   0 runner    (1001) docker     (123)    11901 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/_services/microanalytic_score.py
--rw-r--r--   0 runner    (1001) docker     (123)    18619 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/_services/model_management.py
--rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/_services/model_publish.py
--rw-r--r--   0 runner    (1001) docker     (123)    28696 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/_services/model_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/_services/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/_services/relationships.py
--rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/_services/report_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/_services/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/_services/saslogon.py
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/_services/sentiment_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    13771 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/_services/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/_services/text_categorization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/_services/text_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/_services/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    74999 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:53:46.313591 sasctl-1.9.0/src/sasctl/pzmm/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/pzmm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16653 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/pzmm/gitIntegration.py
--rw-r--r--   0 runner    (1001) docker     (123)    17208 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/pzmm/import_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/pzmm/mlflow_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12306 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/pzmm/model_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/pzmm/pickle_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:53:46.313591 sasctl-1.9.0/src/sasctl/pzmm/template_files/
--rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/pzmm/template_files/dmcas_fitstat.json
--rw-r--r--   0 runner    (1001) docker     (123)    51874 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/pzmm/template_files/dmcas_lift.json
--rw-r--r--   0 runner    (1001) docker     (123)   193713 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/pzmm/template_files/dmcas_roc.json
--rw-r--r--   0 runner    (1001) docker     (123)    81331 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/pzmm/write_json_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    64584 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/pzmm/write_score_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/pzmm/zip_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/services.py
--rw-r--r--   0 runner    (1001) docker     (123)    33574 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:53:46.317592 sasctl-1.9.0/src/sasctl/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16435 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/utils/astore.py
--rw-r--r--   0 runner    (1001) docker     (123)     9921 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/utils/model_migration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:53:46.317592 sasctl-1.9.0/src/sasctl/utils/pymas/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/utils/pymas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22824 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/utils/pymas/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    20869 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/utils/pymas/ds2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/utils/pymas/python.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:53:46.317592 sasctl-1.9.0/src/sasctl/utils/pyml2ds/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/utils/pyml2ds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:53:46.317592 sasctl-1.9.0/src/sasctl/utils/pyml2ds/basic/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/utils/pyml2ds/basic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/utils/pyml2ds/basic/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:53:46.317592 sasctl-1.9.0/src/sasctl/utils/pyml2ds/connectors/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/utils/pyml2ds/connectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:53:46.321592 sasctl-1.9.0/src/sasctl/utils/pyml2ds/connectors/ensembles/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/utils/pyml2ds/connectors/ensembles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/utils/pyml2ds/connectors/ensembles/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/utils/pyml2ds/connectors/ensembles/lgb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/utils/pyml2ds/connectors/ensembles/pmml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/utils/pyml2ds/connectors/ensembles/xgb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-04-05 12:53:34.000000 sasctl-1.9.0/src/sasctl/utils/pyml2ds/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:53:46.301591 sasctl-1.9.0/src/sasctl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11136 2023-04-05 12:53:46.000000 sasctl-1.9.0/src/sasctl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-04-05 12:53:46.000000 sasctl-1.9.0/src/sasctl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 12:53:46.000000 sasctl-1.9.0/src/sasctl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-05 12:53:46.000000 sasctl-1.9.0/src/sasctl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-05 12:53:46.000000 sasctl-1.9.0/src/sasctl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-05 12:53:46.000000 sasctl-1.9.0/src/sasctl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:12:07.123613 sasctl-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    18263 2023-05-04 13:11:54.000000 sasctl-1.9.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-04 13:11:54.000000 sasctl-1.9.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-05-04 13:11:54.000000 sasctl-1.9.1/ContributorAgreement.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-04 13:11:54.000000 sasctl-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-04 13:11:54.000000 sasctl-1.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11136 2023-05-04 13:12:07.119613 sasctl-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9790 2023-05-04 13:11:54.000000 sasctl-1.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-04 13:11:54.000000 sasctl-1.9.1/SUPPORT.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 13:12:07.123613 sasctl-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-05-04 13:11:55.000000 sasctl-1.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:12:07.095613 sasctl-1.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:12:07.103613 sasctl-1.9.1/src/sasctl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:12:07.111613 sasctl-1.9.1/src/sasctl/_services/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/_services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19546 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/_services/cas_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/_services/concepts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/_services/data_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/_services/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/_services/folders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11901 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/_services/microanalytic_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18619 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/_services/model_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/_services/model_publish.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28696 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/_services/model_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/_services/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/_services/relationships.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/_services/report_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/_services/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/_services/saslogon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/_services/sentiment_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13771 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/_services/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/_services/text_categorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/_services/text_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/_services/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74999 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:12:07.115613 sasctl-1.9.1/src/sasctl/pzmm/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/pzmm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16653 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/pzmm/gitIntegration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17213 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/pzmm/import_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/pzmm/mlflow_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12306 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/pzmm/model_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/pzmm/pickle_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:12:07.115613 sasctl-1.9.1/src/sasctl/pzmm/template_files/
+-rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/pzmm/template_files/dmcas_fitstat.json
+-rw-r--r--   0 runner    (1001) docker     (123)    51874 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/pzmm/template_files/dmcas_lift.json
+-rw-r--r--   0 runner    (1001) docker     (123)   193713 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/pzmm/template_files/dmcas_roc.json
+-rw-r--r--   0 runner    (1001) docker     (123)    82150 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/pzmm/write_json_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63867 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/pzmm/write_score_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/pzmm/zip_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33574 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:12:07.115613 sasctl-1.9.1/src/sasctl/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16435 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/utils/astore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9921 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/utils/model_migration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:12:07.119613 sasctl-1.9.1/src/sasctl/utils/pymas/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/utils/pymas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22824 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/utils/pymas/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20869 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/utils/pymas/ds2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/utils/pymas/python.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:12:07.119613 sasctl-1.9.1/src/sasctl/utils/pyml2ds/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/utils/pyml2ds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:12:07.119613 sasctl-1.9.1/src/sasctl/utils/pyml2ds/basic/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/utils/pyml2ds/basic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/utils/pyml2ds/basic/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:12:07.119613 sasctl-1.9.1/src/sasctl/utils/pyml2ds/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/utils/pyml2ds/connectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:12:07.119613 sasctl-1.9.1/src/sasctl/utils/pyml2ds/connectors/ensembles/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/utils/pyml2ds/connectors/ensembles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/utils/pyml2ds/connectors/ensembles/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/utils/pyml2ds/connectors/ensembles/lgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/utils/pyml2ds/connectors/ensembles/pmml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/utils/pyml2ds/connectors/ensembles/xgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-05-04 13:11:55.000000 sasctl-1.9.1/src/sasctl/utils/pyml2ds/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:12:07.103613 sasctl-1.9.1/src/sasctl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11136 2023-05-04 13:12:07.000000 sasctl-1.9.1/src/sasctl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-04 13:12:07.000000 sasctl-1.9.1/src/sasctl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 13:12:07.000000 sasctl-1.9.1/src/sasctl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-04 13:12:07.000000 sasctl-1.9.1/src/sasctl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-04 13:12:07.000000 sasctl-1.9.1/src/sasctl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-04 13:12:07.000000 sasctl-1.9.1/src/sasctl.egg-info/top_level.txt
```

### Comparing `sasctl-1.9.0/CHANGELOG.md` & `sasctl-1.9.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,25 @@
 Unreleased
 ----------
 **Improvements**
  - Refactor `tasks.py` to utilize `sasctl.pzmm` functions.
  - Add `model_info` class to better capture model information.
 
+v1.9.1 (2023-05-04)
+----------
+**Improvements**
+ - Updated handling of H2O models in `sasctl.pzmm`.
+   - Models are now saved with the appropriate `h2o` functions within the `sasctl.pzmm.PickleModel.pickle_trained_model` function.
+   - Example notebooks have been updated to reflect this change.
+
+**Bugfixes**
+ - Added check for `sasctl.pzmm.JSONFiles.calculate_model_statsistics` function to replace float NaN values invalid for JSON files.
+ - Fixed issue where the `sasctl.pzmm.JSONFiles.write_model_properties` function was replacing the user-defined model_function argument.
+ - Added NpEncoder class to check for numpy values in JSON files. Numpy-types cannot be used in SAS Viya.
+
 v1.9.0 (2023-04-04)
 ----------
 **Improvements**
  - `sasctl.pzmm` refactored to follow PEP8 standards, include type hinting, and major expansion of code coverage.
    - `sasctl.pzmm` functions that can generate files can now run in-memory instead of writing to disk.
  - Added custom KPI handling via `pzmm.model_parameters`, allowing users to interact with the KPI table generated by model performance via API.
    - Added a method for scikit-learn models to generate hyperparameters as custom KPIs.
```

### Comparing `sasctl-1.9.0/CONTRIBUTING.md` & `sasctl-1.9.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.0/ContributorAgreement.txt` & `sasctl-1.9.1/ContributorAgreement.txt`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.0/LICENSE` & `sasctl-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.0/PKG-INFO` & `sasctl-1.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sasctl
-Version: 1.9.0
+Version: 1.9.1
 Summary: SAS Viya Python Client
 Home-page: https://github.com/sassoftware/python-sasctl/
 Author: SAS
 License: Apache v2.0
 Project-URL: Bug Tracker, https://github.com/sassoftware/python-sasctl/issues
 Project-URL: Documentation, https://sassoftware.github.io/python-sasctl/
 Project-URL: Source Code, https://github.com/sassoftware/python-sasctl
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sasctl Version: 1.9.0 Summary: SAS Viya Python
+Metadata-Version: 2.1 Name: sasctl Version: 1.9.1 Summary: SAS Viya Python
 Client Home-page: https://github.com/sassoftware/python-sasctl/ Author: SAS
 License: Apache v2.0 Project-URL: Bug Tracker, https://github.com/sassoftware/
 python-sasctl/issues Project-URL: Documentation, https://sassoftware.github.io/
 python-sasctl/ Project-URL: Source Code, https://github.com/sassoftware/python-
 sasctl Classifier: Development Status :: 5 - Production/Stable Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Environment ::
 Console Classifier: Intended Audience :: Science/Research Classifier: Intended
```

### Comparing `sasctl-1.9.0/README.md` & `sasctl-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.0/setup.py` & `sasctl-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.0/src/sasctl/__init__.py` & `sasctl-1.9.1/src/sasctl/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 # encoding: utf-8
 #
 # Copyright © 2019, SAS Institute Inc., Cary, NC, USA.  All Rights Reserved.
 # SPDX-License-Identifier: Apache-2.0
 
-__version__ = "1.9.0"
+__version__ = "1.9.1"
 __author__ = "SAS"
 __credits__ = [
     "Yi Jian Ching",
     "Lucas De Paula",
     "James Kochuba",
     "Peter Tobac",
     "Chris Toth",
```

### Comparing `sasctl-1.9.0/src/sasctl/_services/cas_management.py` & `sasctl-1.9.1/src/sasctl/_services/cas_management.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.0/src/sasctl/_services/concepts.py` & `sasctl-1.9.1/src/sasctl/_services/concepts.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.0/src/sasctl/_services/data_sources.py` & `sasctl-1.9.1/src/sasctl/_services/data_sources.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.0/src/sasctl/_services/files.py` & `sasctl-1.9.1/src/sasctl/_services/files.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.0/src/sasctl/_services/folders.py` & `sasctl-1.9.1/src/sasctl/_services/folders.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.0/src/sasctl/_services/microanalytic_score.py` & `sasctl-1.9.1/src/sasctl/_services/microanalytic_score.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.0/src/sasctl/_services/model_management.py` & `sasctl-1.9.1/src/sasctl/_services/model_management.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.0/src/sasctl/_services/model_publish.py` & `sasctl-1.9.1/src/sasctl/_services/model_publish.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.0/src/sasctl/_services/model_repository.py` & `sasctl-1.9.1/src/sasctl/_services/model_repository.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.0/src/sasctl/_services/projects.py` & `sasctl-1.9.1/src/sasctl/_services/projects.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.0/src/sasctl/_services/relationships.py` & `sasctl-1.9.1/src/sasctl/_services/relationships.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.0/src/sasctl/_services/report_images.py` & `sasctl-1.9.1/src/sasctl/_services/report_images.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.0/src/sasctl/_services/reports.py` & `sasctl-1.9.1/src/sasctl/_services/reports.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.0/src/sasctl/_services/saslogon.py` & `sasctl-1.9.1/src/sasctl/_services/saslogon.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.0/src/sasctl/_services/sentiment_analysis.py` & `sasctl-1.9.1/src/sasctl/_services/sentiment_analysis.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.0/src/sasctl/_services/service.py` & `sasctl-1.9.1/src/sasctl/_services/service.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.0/src/sasctl/_services/text_categorization.py` & `sasctl-1.9.1/src/sasctl/_services/text_categorization.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.0/src/sasctl/_services/text_parsing.py` & `sasctl-1.9.1/src/sasctl/_services/text_parsing.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.0/src/sasctl/_services/workflow.py` & `sasctl-1.9.1/src/sasctl/_services/workflow.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.0/src/sasctl/core.py` & `sasctl-1.9.1/src/sasctl/core.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.0/src/sasctl/exceptions.py` & `sasctl-1.9.1/src/sasctl/exceptions.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.0/src/sasctl/pzmm/gitIntegration.py` & `sasctl-1.9.1/src/sasctl/pzmm/gitIntegration.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.0/src/sasctl/pzmm/import_model.py` & `sasctl-1.9.1/src/sasctl/pzmm/import_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
     @classmethod
     def import_model(
         cls,
         model_files: Union[str, Path, dict],
         model_prefix: str,
         project: Union[str, dict, RestObj],
         input_data: Optional[DataFrame] = None,
-        predict_method: [Callable[..., List], List[Any]] = None,
+        predict_method: Union[Callable[..., List], List[Any]] = None,
         score_metrics: Optional[List[str]] = None,
         pickle_type: str = "pickle",
         project_version: str = "latest",
         missing_values: bool = False,
         overwrite_model: bool = False,
         score_cas: bool = True,
         mlflow_details: Optional[dict] = None,
```

### Comparing `sasctl-1.9.0/src/sasctl/pzmm/mlflow_model.py` & `sasctl-1.9.1/src/sasctl/pzmm/mlflow_model.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.0/src/sasctl/pzmm/model_parameters.py` & `sasctl-1.9.1/src/sasctl/pzmm/model_parameters.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.0/src/sasctl/pzmm/pickle_model.py` & `sasctl-1.9.1/src/sasctl/pzmm/pickle_model.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,30 +2,35 @@
 # SPDX-License-Identifier: Apache-2.0
 # %%
 import codecs
 import gzip
 import pickle
 import shutil
 from pathlib import Path
-from typing import Optional, Union
+from typing import Any, Optional, Union
+
+try:
+    import h2o
+except ImportError:
+    h2o = None
 
 from ..utils.misc import check_if_jupyter
 
 PICKLE = ".pickle"
 # TODO: Break up function to lower CC
 
 
 class PickleModel:
     notebook_output: bool = check_if_jupyter()
 
     @classmethod
     def pickle_trained_model(
         cls,
-        trained_model,
-        model_prefix,
+        model_prefix: str,
+        trained_model: Optional[Any] = None,
         pickle_path: Union[str, Path, None] = None,
         is_h2o_model: bool = False,
         is_binary_model: bool = False,
         is_binary_string: bool = False,
         mlflow_details: Optional[dict] = None,
     ) -> Union[dict, str, None]:
         """
@@ -36,35 +41,34 @@
             * '*.pickle'
                 Binary pickle file containing a trained model.
             * '*.mojo'
                 Archived H2O.ai MOJO file containing a trained model.
 
         Parameters
         ---------------
-        trained_model : model object, str, or Path
-            For non-H2O models, this argument contains the model variable. Otherwise,
-            this should be the file path of the MOJO file.
         model_prefix : str or Path
             Variable name for the model to be displayed in SAS Open Model Manager
             (i.e. hmeqClassTree + [Score.py || .pickle]).
+        trained_model : model object
+            The trained model to be exported.
         pickle_path : str, optional
             File location for the output pickle file. The default value is None.
         is_h2o_model : bool, optional
             Sets whether the model file is an H2O.ai MOJO file. If set as True,
             the MOJO file will be gzipped before uploading to SAS Model Manager.
             The default value is False.
         is_binary_model : bool, optional
             Sets whether the H2O model provided is a binary model or a MOJO model. The
             default value is False.
         is_binary_string : bool, optional
             Sets whether the model is to be set as a binary string instead of a pickle
             file. The default value is False.
         mlflow_details : dict, optional
             Model details from an MLFlow model. This dictionary is created by the
-            readMLModelFile function. The default value is None
+            readMLModelFile function. The default value is None.
 
         Returns
         -------
         binary_string : binary str
             When the is_binary_string flag is set to True, return a binary string
             representation of the model instead of a pickle or MOJO file.
         dict
@@ -102,27 +106,34 @@
                     if cls.notebook_output:
                         print(
                             f"Model {model_prefix} was successfully pickled and saved "
                             f"to {Path(pickle_path) / (model_prefix + PICKLE)}."
                         )
                 else:
                     return {model_prefix + PICKLE: pickle.dumps(trained_model)}
-            # For binary H2O models, rename the binary file as a pickle file
-            elif is_binary_model and pickle_path:
-                binary_file = Path(pickle_path) / model_prefix
-                binary_file.rename(binary_file.with_suffix(PICKLE))
-            # For MOJO H2O models, gzip the model file and adjust the file extension
+            # For binary H2O models, save the binary file as a "pickle" file
+            elif is_h2o_model and is_binary_model and pickle_path:
+                if not h2o:
+                    raise RuntimeError(
+                        "The h2o package is required to save the model as a binary h2o"
+                        "model."
+                    )
+                h2o.save_model(
+                    model=trained_model,
+                    force=True,
+                    path=str(pickle_path),
+                    filename=f"{model_prefix}.pickle",
+                )
+            # For MOJO H2O models, save as a mojo file and adjust the extension to .mojo
             elif is_h2o_model and pickle_path:
-                with open(Path(trained_model), "rb") as fileIn, gzip.open(
-                    Path(pickle_path) / (model_prefix + ".mojo"), "wb"
-                ) as fileOut:
-                    fileOut.writelines(fileIn)
-                if cls.notebook_output:
-                    print(
-                        f"MOJO model {model_prefix} was successfully gzipped and saved "
-                        f"to {Path(pickle_path) / (model_prefix + '.mojo')}."
+                if not h2o:
+                    raise RuntimeError(
+                        "The h2o package is required to save the model as a mojo model."
                     )
-            else:
+                trained_model.save_mojo(
+                    force=True, path=str(pickle_path), filename=f"{model_prefix}.mojo"
+                )
+            elif is_binary_model or is_h2o_model:
                 raise ValueError(
                     "There is currently no support for file-less H2O.ai model handling."
                     " Please include a value for the pickle_path argument."
                 )
```

### Comparing `sasctl-1.9.0/src/sasctl/pzmm/template_files/dmcas_fitstat.json` & `sasctl-1.9.1/src/sasctl/pzmm/template_files/dmcas_fitstat.json`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.0/src/sasctl/pzmm/template_files/dmcas_lift.json` & `sasctl-1.9.1/src/sasctl/pzmm/template_files/dmcas_lift.json`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.0/src/sasctl/pzmm/template_files/dmcas_roc.json` & `sasctl-1.9.1/src/sasctl/pzmm/template_files/dmcas_roc.json`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.0/src/sasctl/pzmm/write_json_files.py` & `sasctl-1.9.1/src/sasctl/pzmm/write_json_files.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,35 @@
 from pandas import DataFrame, Series
 
 # Package Imports
 from ..core import current_session
 from ..utils.decorators import deprecated
 from ..utils.misc import check_if_jupyter
 
+try:
+    # noinspection PyPackageRequirements
+    import numpy as np
+
+    class NpEncoder(json.JSONEncoder):
+        def default(self, obj):
+            if isinstance(obj, np.integer):
+                return int(obj)
+            if isinstance(obj, np.floating):
+                return float(obj)
+            if isinstance(obj, np.ndarray):
+                return obj.tolist()
+            return json.JSONEncoder.default(self, obj)
+
+except ImportError:
+    np = None
+
+    class NpEncoder(json.JSONEncoder):
+        pass
+
+
 # TODO: add converter for any type of dataset (list, dataframe, numpy array)
 
 # Constants
 INPUT = "inputVar.json"
 OUTPUT = "outputVar.json"
 PROP = "ModelProperties.json"
 META = "fileMetadata.json"
@@ -121,25 +142,25 @@
         if json_path:
             if is_input:
                 file_name = INPUT
             else:
                 file_name = OUTPUT
 
             with open(Path(json_path) / file_name, "w") as json_file:
-                json_file.write(json.dumps(dict_list, indent=4))
+                json_file.write(json.dumps(dict_list, indent=4, cls=NpEncoder))
             if cls.notebook_output:
                 print(
                     f"{file_name} was successfully written and saved to "
                     f"{Path(json_path) / file_name}"
                 )
         else:
             if is_input:
-                return {INPUT: json.dumps(dict_list)}
+                return {INPUT: json.dumps(dict_list, indent=4, cls=NpEncoder)}
             else:
-                return {OUTPUT: json.dumps(dict_list)}
+                return {OUTPUT: json.dumps(dict_list, indent=4, cls=NpEncoder)}
 
     @staticmethod
     def generate_variable_properties(
         input_data: Union[DataFrame, Series]
     ) -> List[dict]:
         """
         Generate a list of dictionaries of variable properties given an input dataframe.
@@ -325,25 +346,25 @@
                 model_desc = model_desc[:1024]
                 warnings.warn(
                     "WARNING: The provided model description was truncated to 1024 "
                     "characters."
                 )
 
         if not target_values:
-            model_function = "Prediction"
+            model_function = model_function if model_function else "Prediction"
             target_level = "INTERVAL"
             target_event = ""
             event_prob_var = ""
         elif isinstance(target_values, list) and len(target_values) == 2:
-            model_function = "Classification"
+            model_function = model_function if model_function else "Classification"
             target_level = "BINARY"
             target_event = str(target_values[0])
             event_prob_var = f"P_{target_values[0]}"
         elif isinstance(target_values, list) and len(target_values) > 2:
-            model_function = "Classification"
+            model_function = model_function if model_function else "Classification"
             target_level = "NOMINAL"
             target_event = ""
             event_prob_var = ""
             targets = [str(x) for x in target_values]
             properties.append(
                 {
                     "name": "multiclass_target_events",
@@ -573,22 +594,22 @@
             data_map = cls.add_df_to_fitstat(fitstat_df, data_map)
 
         for i in range(3):
             json_dict["data"][i] = data_map[i]
 
         if json_path:
             with open(Path(json_path) / FITSTAT, "w") as json_file:
-                json_file.write(json.dumps(json_dict, indent=4))
+                json_file.write(json.dumps(json_dict, indent=4, cls=NpEncoder))
             if cls.notebook_output:
                 print(
                     f"{FITSTAT} was successfully written and saved to "
                     f"{Path(json_path) / FITSTAT}"
                 )
         else:
-            return {FITSTAT: json.dumps(json_dict, indent=4)}
+            return {FITSTAT: json.dumps(json_dict, indent=4, cls=NpEncoder)}
 
     @classmethod
     def add_tuple_to_fitstat(
         cls, data: List[dict], parameters: List[tuple]
     ) -> List[dict]:
         """
         Using tuples defined in input_fit_statistics, add them to the dmcas_fitstat json
@@ -857,25 +878,25 @@
             lift_dict = cls.apply_dataframe_to_json(json_dict[2]["data"], i, lift_df)
             for j in range(len(lift_dict)):
                 json_dict[2]["data"][j].update(lift_dict[j])
 
         if json_path:
             for name in [FITSTAT, ROC, LIFT]:
                 with open(Path(json_path) / name, "w") as json_file:
-                    json_file.write(json.dumps(json_dict, indent=4))
+                    json_file.write(json.dumps(json_dict, indent=4, cls=NpEncoder))
                 if cls.notebook_output:
                     print(
                         f"{name} was successfully written and saved to "
                         f"{Path(json_path) / name}"
                     )
         else:
             return {
-                FITSTAT: json.dumps(json_dict[0], indent=4),
-                ROC: json.dumps(json_dict[1], indent=4),
-                LIFT: json.dumps(json_dict[2], indent=4),
+                FITSTAT: json.dumps(json_dict[0], indent=4, cls=NpEncoder),
+                ROC: json.dumps(json_dict[1], indent=4, cls=NpEncoder),
+                LIFT: json.dumps(json_dict[2], indent=4, cls=NpEncoder),
             }
 
     @staticmethod
     def check_for_data(
         validate: Union[DataFrame, List[list], Type["numpy.array"]] = None,
         train: Union[DataFrame, List[list], Type["numpy.array"]] = None,
         test: Union[DataFrame, List[list], Type["numpy.array"]] = None,
@@ -1016,19 +1037,19 @@
         Returns
         -------
         json_dict : dict
             Dictionary representation of the ROC or Lift chart json file, with the
             values from the SAS CAS percentile action set added in.
         """
         for row_num in range(len(stat_df)):
-            row_dict = stat_df.iloc[row_num].to_dict()
+            row_dict = stat_df.iloc[row_num].replace(float("nan"), None).to_dict()
             json_dict[row_num + partition * len(stat_df)]["dataMap"].update(row_dict)
         return json_dict
 
-    # noinspection PyCallingNonCallable,PyNestedDecorators
+    # noinspection PyCallingNonCallable, PyNestedDecorators
     @deprecated(
         "Please use the calculate_model_statistics method instead.",
         version="1.9",
         removed_in="1.10",
     )
     @classmethod
     def calculateFitStat(
```

### Comparing `sasctl-1.9.0/src/sasctl/pzmm/write_score_code.py` & `sasctl-1.9.1/src/sasctl/pzmm/write_score_code.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     score_code: str = ""
 
     @classmethod
     def write_score_code(
         cls,
         model_prefix: str,
         input_data: Union[DataFrame, List[dict]],
-        predict_method: [Callable[..., List], List[Any]],
+        predict_method: Union[Callable[..., List], List[Any]],
         target_variable: Optional[str] = None,
         target_values: Optional[List] = None,
         score_metrics: Optional[List[str]] = None,
         predict_threshold: Optional[float] = None,
         model: Union[str, dict, RestObj, None] = None,
         pickle_type: str = "pickle",
         missing_values: Optional[bool] = False,
@@ -511,31 +511,16 @@
         binary_h2o_model : boolean, optional
             Flag to indicate that the model is a H2O.ai binary model. The default value
             is None.
         """
         pickle_type = pickle_type if pickle_type else "pickle"
 
         if mojo_model:
-            cls.score_code += (
-                f"with gzip.open(Path(settings.pickle_path) / "
-                '"{model_file_name}", "r") as fileIn, '
-                "open(Path(settings.pickle_path) / "
-                f"\"{str(Path(model_file_name).with_suffix('.zip'))}\","
-                f" \"wb\") as fileOut:\n{'':4}shutil.copyfileobj(fileIn,"
-                " fileOut)\nos.chmod(Path(settings.pickle_path) / "
-                f"\"{str(Path(model_file_name).with_suffix('.zip'))}\""
-                ", 0o777)\nmodel = h2o.import_mojo("
-                "Path(settings.pickle_path) / "
-                f"\"{str(Path(model_file_name).with_suffix('.zip'))}\")"
-                "\n\n"
-            )
-            return (
-                f"{'':8}model = h2o.import_mojo(Path(settings.pickle_path) / "
-                f"\"{str(Path(model_file_name).with_suffix('.zip'))}\")\n\n"
-            )
+            cls.score_code += "model = h2o.import_mojo(Path(settings.pickle_path))\n\n"
+            return f"{'':8}model = h2o.import_mojo(Path(settings.pickle_path))\n\n"
         elif binary_h2o_model:
             cls.score_code += "model = h2o.load(Path(settings.pickle_path))\n\n"
             return f"{'':8}model = h2o.load(Path(settings.pickle_path))\n\n"
         else:
             cls.score_code += (
                 f"with open(Path(settings.pickle_path) / "
                 f'"{model_file_name}", "rb") as pickle_model:\n    '
```

### Comparing `sasctl-1.9.0/src/sasctl/pzmm/zip_model.py` & `sasctl-1.9.1/src/sasctl/pzmm/zip_model.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.0/src/sasctl/services.py` & `sasctl-1.9.1/src/sasctl/services.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.0/src/sasctl/tasks.py` & `sasctl-1.9.1/src/sasctl/tasks.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.0/src/sasctl/utils/astore.py` & `sasctl-1.9.1/src/sasctl/utils/astore.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.0/src/sasctl/utils/cli.py` & `sasctl-1.9.1/src/sasctl/utils/cli.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.0/src/sasctl/utils/decorators.py` & `sasctl-1.9.1/src/sasctl/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.0/src/sasctl/utils/misc.py` & `sasctl-1.9.1/src/sasctl/utils/misc.py`

 * *Files 5% similar despite different names*

```diff
@@ -84,9 +84,9 @@
         shell = get_ipython().__class__.__name__
         if shell == "ZMQInteractiveShell":
             return True
         elif shell == "TerminalInteractiveShell":
             return False
         else:
             return False
-    except NameError:
+    except (ImportError, NameError):
         return False
```

### Comparing `sasctl-1.9.0/src/sasctl/utils/model_migration.py` & `sasctl-1.9.1/src/sasctl/utils/model_migration.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.0/src/sasctl/utils/pymas/core.py` & `sasctl-1.9.1/src/sasctl/utils/pymas/core.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.0/src/sasctl/utils/pymas/ds2.py` & `sasctl-1.9.1/src/sasctl/utils/pymas/ds2.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.0/src/sasctl/utils/pymas/python.py` & `sasctl-1.9.1/src/sasctl/utils/pymas/python.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.0/src/sasctl/utils/pyml2ds/basic/tree.py` & `sasctl-1.9.1/src/sasctl/utils/pyml2ds/basic/tree.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.0/src/sasctl/utils/pyml2ds/connectors/ensembles/core.py` & `sasctl-1.9.1/src/sasctl/utils/pyml2ds/connectors/ensembles/core.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.0/src/sasctl/utils/pyml2ds/connectors/ensembles/lgb.py` & `sasctl-1.9.1/src/sasctl/utils/pyml2ds/connectors/ensembles/lgb.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.0/src/sasctl/utils/pyml2ds/connectors/ensembles/pmml.py` & `sasctl-1.9.1/src/sasctl/utils/pyml2ds/connectors/ensembles/pmml.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.0/src/sasctl/utils/pyml2ds/connectors/ensembles/xgb.py` & `sasctl-1.9.1/src/sasctl/utils/pyml2ds/connectors/ensembles/xgb.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.0/src/sasctl/utils/pyml2ds/core.py` & `sasctl-1.9.1/src/sasctl/utils/pyml2ds/core.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.0/src/sasctl.egg-info/PKG-INFO` & `sasctl-1.9.1/src/sasctl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sasctl
-Version: 1.9.0
+Version: 1.9.1
 Summary: SAS Viya Python Client
 Home-page: https://github.com/sassoftware/python-sasctl/
 Author: SAS
 License: Apache v2.0
 Project-URL: Bug Tracker, https://github.com/sassoftware/python-sasctl/issues
 Project-URL: Documentation, https://sassoftware.github.io/python-sasctl/
 Project-URL: Source Code, https://github.com/sassoftware/python-sasctl
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sasctl Version: 1.9.0 Summary: SAS Viya Python
+Metadata-Version: 2.1 Name: sasctl Version: 1.9.1 Summary: SAS Viya Python
 Client Home-page: https://github.com/sassoftware/python-sasctl/ Author: SAS
 License: Apache v2.0 Project-URL: Bug Tracker, https://github.com/sassoftware/
 python-sasctl/issues Project-URL: Documentation, https://sassoftware.github.io/
 python-sasctl/ Project-URL: Source Code, https://github.com/sassoftware/python-
 sasctl Classifier: Development Status :: 5 - Production/Stable Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Environment ::
 Console Classifier: Intended Audience :: Science/Research Classifier: Intended
```

### Comparing `sasctl-1.9.0/src/sasctl.egg-info/SOURCES.txt` & `sasctl-1.9.1/src/sasctl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

