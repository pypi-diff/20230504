# Comparing `tmp/codecov-cli-0.1.4.tar.gz` & `tmp/codecov-cli-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codecov-cli-0.1.4.tar", last modified: Tue May  2 14:02:58 2023, max compression
+gzip compressed data, was "codecov-cli-0.1.7.tar", last modified: Thu May  4 14:42:13 2023, max compression
```

## Comparing `codecov-cli-0.1.4.tar` & `codecov-cli-0.1.7.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:02:58.710959 codecov-cli-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11545 2023-05-02 14:02:58.710959 codecov-cli-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:02:58.698959 codecov-cli-0.1.4/codecov_cli/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:02:58.698959 codecov-cli-0.1.4/codecov_cli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/commands/base_picking.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/commands/commit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/commands/create_report_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/commands/get_report_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/commands/labelanalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/commands/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/commands/staticanalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/commands/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/fallbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:02:58.702959 codecov-cli-0.1.4/codecov_cli/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/helpers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:02:58.702959 codecov-cli-0.1.4/codecov_cli/helpers/ci_adapters/
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/helpers/ci_adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/helpers/ci_adapters/appveyor_ci.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/helpers/ci_adapters/azure_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/helpers/ci_adapters/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/helpers/ci_adapters/bitbucket_ci.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/helpers/ci_adapters/bitrise_ci.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/helpers/ci_adapters/buildkite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/helpers/ci_adapters/circleci.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/helpers/ci_adapters/cirrus_ci.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/helpers/ci_adapters/codebuild.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/helpers/ci_adapters/droneci.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/helpers/ci_adapters/github_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/helpers/ci_adapters/gitlab_ci.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/helpers/ci_adapters/heroku.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/helpers/ci_adapters/jenkins.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/helpers/ci_adapters/local.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/helpers/ci_adapters/teamcity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/helpers/ci_adapters/travis_ci.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/helpers/ci_adapters/woodpeckerci.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/helpers/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/helpers/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/helpers/folder_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/helpers/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/helpers/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/helpers/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/helpers/versioning_systems.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:02:58.702959 codecov-cli-0.1.4/codecov_cli/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/plugins/gcov.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/plugins/pycoverage.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/plugins/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/plugins/xcode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:02:58.702959 codecov-cli-0.1.4/codecov_cli/runners/
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/runners/dan_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/runners/python_standard_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/runners/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:02:58.702959 codecov-cli-0.1.4/codecov_cli/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:02:58.702959 codecov-cli-0.1.4/codecov_cli/services/commit/
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/services/commit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/services/commit/base_picking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:02:58.702959 codecov-cli-0.1.4/codecov_cli/services/report/
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/services/report/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:02:58.702959 codecov-cli-0.1.4/codecov_cli/services/staticanalysis/
--rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/services/staticanalysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:02:58.702959 codecov-cli-0.1.4/codecov_cli/services/staticanalysis/analyzers/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/services/staticanalysis/analyzers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/services/staticanalysis/analyzers/ecmascriptsix.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/services/staticanalysis/analyzers/general.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:02:58.702959 codecov-cli-0.1.4/codecov_cli/services/staticanalysis/analyzers/python/
--rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/services/staticanalysis/analyzers/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/services/staticanalysis/analyzers/python/node_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/services/staticanalysis/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/services/staticanalysis/finders.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/services/staticanalysis/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:02:58.706959 codecov-cli-0.1.4/codecov_cli/services/upload/
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/services/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/services/upload/coverage_file_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/services/upload/legacy_upload_sender.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/services/upload/network_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5199 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/services/upload/upload_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/services/upload/upload_sender.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/codecov_cli/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:02:58.698959 codecov-cli-0.1.4/codecov_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11545 2023-05-02 14:02:58.000000 codecov-cli-0.1.4/codecov_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-05-02 14:02:58.000000 codecov-cli-0.1.4/codecov_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 14:02:58.000000 codecov-cli-0.1.4/codecov_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-02 14:02:58.000000 codecov-cli-0.1.4/codecov_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-02 14:02:58.000000 codecov-cli-0.1.4/codecov_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-02 14:02:58.000000 codecov-cli-0.1.4/codecov_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:02:58.706959 codecov-cli-0.1.4/languages/
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/languages/languages.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:02:58.698959 codecov-cli-0.1.4/languages/treesitterjavascript/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:02:58.706959 codecov-cli-0.1.4/languages/treesitterjavascript/src/
--rw-r--r--   0 runner    (1001) docker     (123)  2277994 2023-05-02 14:02:36.000000 codecov-cli-0.1.4/languages/treesitterjavascript/src/parser.c
--rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-05-02 14:02:36.000000 codecov-cli-0.1.4/languages/treesitterjavascript/src/scanner.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:02:58.706959 codecov-cli-0.1.4/languages/treesitterjavascript/src/tree_sitter/
--rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-05-02 14:02:36.000000 codecov-cli-0.1.4/languages/treesitterjavascript/src/tree_sitter/parser.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:02:58.698959 codecov-cli-0.1.4/languages/treesitterpython/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:02:58.710959 codecov-cli-0.1.4/languages/treesitterpython/src/
--rw-r--r--   0 runner    (1001) docker     (123)  2658198 2023-05-02 14:02:37.000000 codecov-cli-0.1.4/languages/treesitterpython/src/parser.c
--rw-r--r--   0 runner    (1001) docker     (123)    11117 2023-05-02 14:02:37.000000 codecov-cli-0.1.4/languages/treesitterpython/src/scanner.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:02:58.710959 codecov-cli-0.1.4/languages/treesitterpython/src/tree_sitter/
--rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-05-02 14:02:37.000000 codecov-cli-0.1.4/languages/treesitterpython/src/tree_sitter/parser.h
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 14:02:58.710959 codecov-cli-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-02 14:02:34.000000 codecov-cli-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:42:13.344343 codecov-cli-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11545 2023-05-04 14:42:13.344343 codecov-cli-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:42:13.332343 codecov-cli-0.1.7/codecov_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:42:13.332343 codecov-cli-0.1.7/codecov_cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/commands/base_picking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/commands/commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/commands/create_report_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/commands/get_report_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/commands/labelanalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/commands/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/commands/staticanalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/commands/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/fallbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:42:13.336343 codecov-cli-0.1.7/codecov_cli/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/helpers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:42:13.336343 codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/appveyor_ci.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/azure_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/bitbucket_ci.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/bitrise_ci.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/buildkite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/circleci.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/cirrus_ci.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/codebuild.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/droneci.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/github_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/gitlab_ci.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/heroku.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/jenkins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/teamcity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/travis_ci.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/woodpeckerci.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/helpers/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/helpers/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/helpers/folder_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/helpers/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/helpers/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/helpers/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/helpers/versioning_systems.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:42:13.336343 codecov-cli-0.1.7/codecov_cli/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/plugins/gcov.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/plugins/pycoverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/plugins/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/plugins/xcode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:42:13.336343 codecov-cli-0.1.7/codecov_cli/runners/
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/runners/dan_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5570 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/runners/python_standard_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/runners/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:42:13.336343 codecov-cli-0.1.7/codecov_cli/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:42:13.336343 codecov-cli-0.1.7/codecov_cli/services/commit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/services/commit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/services/commit/base_picking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:42:13.336343 codecov-cli-0.1.7/codecov_cli/services/report/
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/services/report/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:42:13.336343 codecov-cli-0.1.7/codecov_cli/services/staticanalysis/
+-rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/services/staticanalysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:42:13.336343 codecov-cli-0.1.7/codecov_cli/services/staticanalysis/analyzers/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/services/staticanalysis/analyzers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/services/staticanalysis/analyzers/ecmascriptsix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/services/staticanalysis/analyzers/general.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:42:13.336343 codecov-cli-0.1.7/codecov_cli/services/staticanalysis/analyzers/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/services/staticanalysis/analyzers/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/services/staticanalysis/analyzers/python/node_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/services/staticanalysis/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/services/staticanalysis/finders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/services/staticanalysis/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:42:13.340343 codecov-cli-0.1.7/codecov_cli/services/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/services/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/services/upload/coverage_file_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/services/upload/legacy_upload_sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/services/upload/network_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5199 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/services/upload/upload_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/services/upload/upload_sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:42:13.332343 codecov-cli-0.1.7/codecov_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11545 2023-05-04 14:42:13.000000 codecov-cli-0.1.7/codecov_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-05-04 14:42:13.000000 codecov-cli-0.1.7/codecov_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 14:42:13.000000 codecov-cli-0.1.7/codecov_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-04 14:42:13.000000 codecov-cli-0.1.7/codecov_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-04 14:42:13.000000 codecov-cli-0.1.7/codecov_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-04 14:42:13.000000 codecov-cli-0.1.7/codecov_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:42:13.340343 codecov-cli-0.1.7/languages/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/languages/languages.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:42:13.332343 codecov-cli-0.1.7/languages/treesitterjavascript/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:42:13.340343 codecov-cli-0.1.7/languages/treesitterjavascript/src/
+-rw-r--r--   0 runner    (1001) docker     (123)  2277994 2023-05-04 14:41:50.000000 codecov-cli-0.1.7/languages/treesitterjavascript/src/parser.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-05-04 14:41:50.000000 codecov-cli-0.1.7/languages/treesitterjavascript/src/scanner.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:42:13.340343 codecov-cli-0.1.7/languages/treesitterjavascript/src/tree_sitter/
+-rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-05-04 14:41:50.000000 codecov-cli-0.1.7/languages/treesitterjavascript/src/tree_sitter/parser.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:42:13.332343 codecov-cli-0.1.7/languages/treesitterpython/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:42:13.344343 codecov-cli-0.1.7/languages/treesitterpython/src/
+-rw-r--r--   0 runner    (1001) docker     (123)  2658198 2023-05-04 14:41:51.000000 codecov-cli-0.1.7/languages/treesitterpython/src/parser.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11117 2023-05-04 14:41:51.000000 codecov-cli-0.1.7/languages/treesitterpython/src/scanner.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:42:13.344343 codecov-cli-0.1.7/languages/treesitterpython/src/tree_sitter/
+-rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-05-04 14:41:51.000000 codecov-cli-0.1.7/languages/treesitterpython/src/tree_sitter/parser.h
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 14:42:13.344343 codecov-cli-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/setup.py
```

### Comparing `codecov-cli-0.1.4/LICENSE` & `codecov-cli-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/PKG-INFO` & `codecov-cli-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codecov-cli
-Version: 0.1.4
+Version: 0.1.7
 Summary: Codecov Command Line Interface
 Author: Codecov
 Author-email: support@codecov.io
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CodecovCLI
```

### Comparing `codecov-cli-0.1.4/README.md` & `codecov-cli-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/codecov_cli/commands/base_picking.py` & `codecov-cli-0.1.7/codecov_cli/commands/base_picking.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/codecov_cli/commands/commit.py` & `codecov-cli-0.1.7/codecov_cli/commands/commit.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/codecov_cli/commands/create_report_result.py` & `codecov-cli-0.1.7/codecov_cli/commands/create_report_result.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/codecov_cli/commands/get_report_results.py` & `codecov-cli-0.1.7/codecov_cli/commands/get_report_results.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/codecov_cli/commands/labelanalysis.py` & `codecov-cli-0.1.7/codecov_cli/commands/labelanalysis.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,25 +56,27 @@
     codecov_yaml = ctx.obj["codecov_yaml"] or {}
     cli_config = codecov_yaml.get("cli", {})
     runner = get_runner(cli_config, runner_name)
     logger.debug(
         f"Selected runner: {runner}",
         extra=dict(extra_log_attributes=dict(config=runner.params)),
     )
+    logger.info("Collecting labels...")
     requested_labels = runner.collect_tests()
     logger.info(f"Collected {len(requested_labels)} tests")
     logger.debug(
         "Labels collected.",
         extra=dict(extra_log_attributes=dict(labels_collected=requested_labels)),
     )
     payload = {
         "base_commit": base_commit_sha,
         "head_commit": head_commit_sha,
         "requested_labels": requested_labels,
     }
+    logger.info("Requesting set of labels to run...")
     try:
         response = requests.post(
             url, json=payload, headers={"Authorization": token_header}
         )
         if response.status_code >= 500:
             logger.warning(
                 "Sorry. Codecov is having problems",
@@ -104,15 +106,15 @@
             raise click.ClickException(
                 "There is some problem with the submitted information"
             )
     except requests.RequestException:
         raise click.ClickException(click.style("Unable to reach Codecov", fg="red"))
     eid = response.json()["external_id"]
     has_result = False
-    logger.info("Label request sent")
+    logger.info("Label request sent. Waiting for result.")
     time.sleep(2)
     while not has_result:
         resp_data = requests.get(
             f"https://api.codecov.io/labels/labels-analysis/{eid}",
             headers={"Authorization": token_header},
         )
         resp_json = resp_data.json()
```

### Comparing `codecov-cli-0.1.4/codecov_cli/commands/report.py` & `codecov-cli-0.1.7/codecov_cli/commands/report.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/codecov_cli/commands/staticanalysis.py` & `codecov-cli-0.1.7/codecov_cli/commands/staticanalysis.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/codecov_cli/commands/upload.py` & `codecov-cli-0.1.7/codecov_cli/commands/upload.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/codecov_cli/fallbacks.py` & `codecov-cli-0.1.7/codecov_cli/fallbacks.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/codecov_cli/helpers/ci_adapters/__init__.py` & `codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/codecov_cli/helpers/ci_adapters/appveyor_ci.py` & `codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/appveyor_ci.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/codecov_cli/helpers/ci_adapters/azure_pipelines.py` & `codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/azure_pipelines.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/codecov_cli/helpers/ci_adapters/base.py` & `codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/base.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/codecov_cli/helpers/ci_adapters/bitbucket_ci.py` & `codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/bitbucket_ci.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/codecov_cli/helpers/ci_adapters/bitrise_ci.py` & `codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/bitrise_ci.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/codecov_cli/helpers/ci_adapters/buildkite.py` & `codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/buildkite.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/codecov_cli/helpers/ci_adapters/circleci.py` & `codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/circleci.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/codecov_cli/helpers/ci_adapters/cirrus_ci.py` & `codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/cirrus_ci.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/codecov_cli/helpers/ci_adapters/codebuild.py` & `codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/codebuild.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/codecov_cli/helpers/ci_adapters/droneci.py` & `codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/droneci.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/codecov_cli/helpers/ci_adapters/github_actions.py` & `codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/github_actions.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/codecov_cli/helpers/ci_adapters/gitlab_ci.py` & `codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/gitlab_ci.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/codecov_cli/helpers/ci_adapters/heroku.py` & `codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/heroku.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/codecov_cli/helpers/ci_adapters/jenkins.py` & `codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/jenkins.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/codecov_cli/helpers/ci_adapters/local.py` & `codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/local.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/codecov_cli/helpers/ci_adapters/teamcity.py` & `codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/teamcity.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/codecov_cli/helpers/ci_adapters/travis_ci.py` & `codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/travis_ci.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/codecov_cli/helpers/ci_adapters/woodpeckerci.py` & `codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/woodpeckerci.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/codecov_cli/helpers/encoder.py` & `codecov-cli-0.1.7/codecov_cli/helpers/encoder.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/codecov_cli/helpers/folder_searcher.py` & `codecov-cli-0.1.7/codecov_cli/helpers/folder_searcher.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/codecov_cli/helpers/git.py` & `codecov-cli-0.1.7/codecov_cli/helpers/git.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/codecov_cli/helpers/logging_utils.py` & `codecov-cli-0.1.7/codecov_cli/helpers/logging_utils.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/codecov_cli/helpers/request.py` & `codecov-cli-0.1.7/codecov_cli/helpers/request.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/codecov_cli/helpers/versioning_systems.py` & `codecov-cli-0.1.7/codecov_cli/helpers/versioning_systems.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/codecov_cli/main.py` & `codecov-cli-0.1.7/codecov_cli/main.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/codecov_cli/plugins/__init__.py` & `codecov-cli-0.1.7/codecov_cli/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/codecov_cli/plugins/gcov.py` & `codecov-cli-0.1.7/codecov_cli/plugins/gcov.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/codecov_cli/plugins/pycoverage.py` & `codecov-cli-0.1.7/codecov_cli/plugins/pycoverage.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/codecov_cli/plugins/xcode.py` & `codecov-cli-0.1.7/codecov_cli/plugins/xcode.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/codecov_cli/runners/__init__.py` & `codecov-cli-0.1.7/codecov_cli/runners/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/codecov_cli/runners/dan_runner.py` & `codecov-cli-0.1.7/codecov_cli/runners/dan_runner.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/codecov_cli/runners/python_standard_runner.py` & `codecov-cli-0.1.7/codecov_cli/runners/python_standard_runner.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
-import subprocess
 from contextlib import redirect_stdout
-from io import StringIO
+from io import StringIO, TextIOWrapper
+from multiprocessing import Queue, get_context
 from os import getcwd
-from sys import path
+from sys import path, stdout
 from typing import List, TypedDict
 
 import pytest
 
 from codecov_cli.runners.types import (
     LabelAnalysisRequestResult,
     LabelAnalysisRunnerInterface,
@@ -33,55 +33,91 @@
         if include_curr_dir:
             path.remove(curr_dir)
         return result
 
     return call_method
 
 
+def _execute_pytest_subprocess(
+    pytest_args: List[str],
+    queue: Queue,
+    parent_stdout: TextIOWrapper,
+    capture_output: bool = True,
+):
+    """Runs pytest from python in a subprocess.
+    This is because we call it twice in the label-analysis process,
+    so we might have import errors if calling it directly.
+    Check the warning: https://docs.pytest.org/en/7.1.x/how-to/usage.html#calling-pytest-from-python-code
+
+    Returns the output value and pytest exit code via queue
+    """
+    subproces_stdout = parent_stdout
+    if capture_output:
+        subproces_stdout = StringIO()
+    with redirect_stdout(subproces_stdout):
+        result = pytest.main(pytest_args)
+    if capture_output:
+        queue.put(subproces_stdout.getvalue())
+    queue.put(result)
+
+
 class PythonStandardRunner(LabelAnalysisRunnerInterface):
     def __init__(self, config_params: PythonStandardRunnerConfigParams = None) -> None:
         super().__init__()
         default_config: PythonStandardRunnerConfigParams = {
             "collect_tests_options": [],
             "include_curr_dir": True,
         }
         if config_params is None:
             config_params = PythonStandardRunnerConfigParams()
         self.params = {**default_config, **config_params}
 
     @_include_curr_dir
-    def _execute_pytest(self, pytest_args: List[str]) -> str:
-        with StringIO() as fd:
-            with redirect_stdout(fd):
-                result = pytest.main(pytest_args)
-            output = fd.getvalue()
-            if result != pytest.ExitCode.OK and result != 0:
-                logger.error(
-                    "Pytest did not run correctly",
-                    extra=dict(
-                        extra_log_attributes=dict(exit_code=result, output=output)
-                    ),
-                )
-                raise Exception("Pytest did not run correctly")
+    def _execute_pytest(
+        self, pytest_args: List[str], capture_output: bool = True, numprocess: int = 1
+    ) -> str:
+        """Handles calling pytest from Python in a subprocess.
+        Raises Exception if pytest fails
+        Returns the complete pytest output
+        """
+        ctx = get_context("fork")
+        output = None
+        queue = ctx.Queue(2)
+        p = ctx.Process(
+            target=_execute_pytest_subprocess,
+            args=[pytest_args, queue, stdout, capture_output],
+        )
+        p.start()
+        if capture_output:
+            output = queue.get()  # Output from pytest emitted by subprocess
+        result = queue.get()  # Pytest exit code emitted by subprocess
+        p.join()
+
+        if p.exitcode != 0 or (result != pytest.ExitCode.OK and result != 0):
+            logger.error(
+                "Pytest did not run correctly",
+                extra=dict(extra_log_attributes=dict(exit_code=result, output=output)),
+            )
+            raise Exception("Pytest did not run correctly")
         return output
 
     def collect_tests(self):
         default_options = ["-q", "--collect-only"]
         extra_args = self.params["collect_tests_options"]
         options_to_use = default_options + extra_args
         logger.debug(
             "Collecting tests",
             extra=dict(
                 extra_log_attributes=dict(options=options_to_use),
             ),
         )
 
         output = self._execute_pytest(options_to_use)
-        lines = output.split()
-        test_names = list(line for line in lines if "::" in line)
+        lines = output.split(sep="\n")
+        test_names = list(line for line in lines if ("::" in line and "test" in line))
         return test_names
 
     def process_labelanalysis_result(self, result: LabelAnalysisRequestResult):
         default_options = ["--cov=./", "--cov-context=test"]
         logger.info(
             "Received information about tests to run",
             extra=dict(
@@ -89,33 +125,32 @@
                     absent_labels=len(result["absent_labels"] or []),
                     present_diff_labels=len(result["present_diff_labels"] or []),
                     global_level_labels=len(result["global_level_labels"] or []),
                     present_report_labels=len(result["present_report_labels"] or []),
                 )
             ),
         )
-        all_labels = (
+        all_labels = set(
             result["absent_labels"]
             + result["present_diff_labels"]
             + result["global_level_labels"]
         )
-        skipped_tests = set(result["present_report_labels"]) - set(all_labels)
+        skipped_tests = set(result["present_report_labels"]) - all_labels
         if skipped_tests:
             logger.info(
                 "Some tests are being skipped",
                 extra=dict(
                     extra_log_attributes=dict(skipped_tests=sorted(skipped_tests))
                 ),
             )
-        all_labels = set(all_labels)
-        all_labels = [x.rsplit("[", 1)[0] if "[" in x else x for x in all_labels]
-        # Not safe from the customer perspective, in general, probably.
-        # This is just to check it working
-        command_array = default_options + all_labels
+
+        command_array = default_options + [
+            label.split("[")[0] if "[" in label else label for label in all_labels
+        ]
         logger.info("Running tests")
         logger.debug(
             "Pytest command",
             extra=dict(extra_log_attributes=dict(command_array=command_array)),
         )
-        output = self._execute_pytest(command_array)
+        output = self._execute_pytest(command_array, capture_output=False)
         logger.info("Finished running tests successfully")
         logger.debug(output)
```

### Comparing `codecov-cli-0.1.4/codecov_cli/services/commit/__init__.py` & `codecov-cli-0.1.7/codecov_cli/services/commit/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/codecov_cli/services/commit/base_picking.py` & `codecov-cli-0.1.7/codecov_cli/services/commit/base_picking.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/codecov_cli/services/report/__init__.py` & `codecov-cli-0.1.7/codecov_cli/services/report/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/codecov_cli/services/staticanalysis/__init__.py` & `codecov-cli-0.1.7/codecov_cli/services/staticanalysis/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/codecov_cli/services/staticanalysis/analyzers/ecmascriptsix.py` & `codecov-cli-0.1.7/codecov_cli/services/staticanalysis/analyzers/ecmascriptsix.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/codecov_cli/services/staticanalysis/analyzers/python/__init__.py` & `codecov-cli-0.1.7/codecov_cli/services/staticanalysis/analyzers/python/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/codecov_cli/services/staticanalysis/analyzers/python/node_wrappers.py` & `codecov-cli-0.1.7/codecov_cli/services/staticanalysis/analyzers/python/node_wrappers.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/codecov_cli/services/staticanalysis/finders.py` & `codecov-cli-0.1.7/codecov_cli/services/staticanalysis/finders.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/codecov_cli/services/upload/__init__.py` & `codecov-cli-0.1.7/codecov_cli/services/upload/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/codecov_cli/services/upload/coverage_file_finder.py` & `codecov-cli-0.1.7/codecov_cli/services/upload/coverage_file_finder.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/codecov_cli/services/upload/legacy_upload_sender.py` & `codecov-cli-0.1.7/codecov_cli/services/upload/legacy_upload_sender.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/codecov_cli/services/upload/network_finder.py` & `codecov-cli-0.1.7/codecov_cli/services/upload/network_finder.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/codecov_cli/services/upload/upload_collector.py` & `codecov-cli-0.1.7/codecov_cli/services/upload/upload_collector.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/codecov_cli/services/upload/upload_sender.py` & `codecov-cli-0.1.7/codecov_cli/services/upload/upload_sender.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/codecov_cli/types.py` & `codecov-cli-0.1.7/codecov_cli/types.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/codecov_cli.egg-info/PKG-INFO` & `codecov-cli-0.1.7/codecov_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codecov-cli
-Version: 0.1.4
+Version: 0.1.7
 Summary: Codecov Command Line Interface
 Author: Codecov
 Author-email: support@codecov.io
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CodecovCLI
```

### Comparing `codecov-cli-0.1.4/codecov_cli.egg-info/SOURCES.txt` & `codecov-cli-0.1.7/codecov_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/languages/treesitterjavascript/src/parser.c` & `codecov-cli-0.1.7/languages/treesitterjavascript/src/parser.c`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/languages/treesitterjavascript/src/scanner.c` & `codecov-cli-0.1.7/languages/treesitterjavascript/src/scanner.c`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/languages/treesitterjavascript/src/tree_sitter/parser.h` & `codecov-cli-0.1.7/languages/treesitterjavascript/src/tree_sitter/parser.h`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/languages/treesitterpython/src/parser.c` & `codecov-cli-0.1.7/languages/treesitterpython/src/parser.c`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/languages/treesitterpython/src/scanner.cc` & `codecov-cli-0.1.7/languages/treesitterpython/src/scanner.cc`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/languages/treesitterpython/src/tree_sitter/parser.h` & `codecov-cli-0.1.7/languages/treesitterpython/src/tree_sitter/parser.h`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.4/setup.py` & `codecov-cli-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="codecov-cli",
-    version="0.1.4",
+    version="0.1.7",
     packages=find_packages(exclude=["contrib", "docs", "tests*"]),
     description="Codecov Command Line Interface",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Codecov",
     author_email="support@codecov.io",
     install_requires=["click", "requests", "PyYAML", "tree_sitter", "httpx"],
```

