# Comparing `tmp/bomf-0.4.0.tar.gz` & `tmp/bomf-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bomf-0.4.0.tar", last modified: Thu May  4 07:42:05 2023, max compression
+gzip compressed data, was "bomf-0.4.1.tar", last modified: Thu May  4 07:55:32 2023, max compression
```

## Comparing `bomf-0.4.0.tar` & `bomf-0.4.1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:42:05.396305 bomf-0.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:42:05.392305 bomf-0.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-04 07:41:58.000000 bomf-0.4.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:42:05.392305 bomf-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-04 07:41:58.000000 bomf-0.4.0/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-05-04 07:41:58.000000 bomf-0.4.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-04 07:41:58.000000 bomf-0.4.0/.github/workflows/coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-04 07:41:58.000000 bomf-0.4.0/.github/workflows/no_byte_order_mark.yml
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-04 07:41:58.000000 bomf-0.4.0/.github/workflows/packaging_test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-04 07:41:58.000000 bomf-0.4.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-04 07:41:58.000000 bomf-0.4.0/.github/workflows/pythonlint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-04 07:41:58.000000 bomf-0.4.0/.github/workflows/unittests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-04 07:41:58.000000 bomf-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-04 07:41:58.000000 bomf-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-04 07:41:58.000000 bomf-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-05-04 07:42:05.396305 bomf-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-05-04 07:41:58.000000 bomf-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-04 07:41:58.000000 bomf-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-04 07:41:58.000000 bomf-0.4.0/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-04 07:41:58.000000 bomf-0.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-04 07:42:05.396305 bomf-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-04 07:41:58.000000 bomf-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:42:05.388305 bomf-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:42:05.392305 bomf-0.4.0/src/bomf/
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-05-04 07:41:58.000000 bomf-0.4.0/src/bomf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:42:05.392305 bomf-0.4.0/src/bomf/filter/
--rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-05-04 07:41:58.000000 bomf-0.4.0/src/bomf/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-05-04 07:41:58.000000 bomf-0.4.0/src/bomf/filter/sourcedataproviderfilter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:42:05.392305 bomf-0.4.0/src/bomf/loader/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-04 07:41:58.000000 bomf-0.4.0/src/bomf/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-05-04 07:41:58.000000 bomf-0.4.0/src/bomf/loader/entityloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:42:05.392305 bomf-0.4.0/src/bomf/mapper/
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-04 07:41:58.000000 bomf-0.4.0/src/bomf/mapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:42:05.392305 bomf-0.4.0/src/bomf/model/
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-05-04 07:41:58.000000 bomf-0.4.0/src/bomf/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:42:05.392305 bomf-0.4.0/src/bomf/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-05-04 07:41:58.000000 bomf-0.4.0/src/bomf/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-04 07:41:58.000000 bomf-0.4.0/src/bomf/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:42:05.392305 bomf-0.4.0/src/bomf/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-04 07:41:58.000000 bomf-0.4.0/src/bomf/validation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:42:05.392305 bomf-0.4.0/src/bomf/validation/core/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-04 07:41:58.000000 bomf-0.4.0/src/bomf/validation/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-05-04 07:41:58.000000 bomf-0.4.0/src/bomf/validation/core/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     7640 2023-05-04 07:41:58.000000 bomf-0.4.0/src/bomf/validation/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    17260 2023-05-04 07:41:58.000000 bomf-0.4.0/src/bomf/validation/core/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-04 07:41:58.000000 bomf-0.4.0/src/bomf/validation/core/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-04 07:41:58.000000 bomf-0.4.0/src/bomf/validation/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-05-04 07:41:58.000000 bomf-0.4.0/src/bomf/validation/core/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-05-04 07:41:58.000000 bomf-0.4.0/src/bomf/validation/path_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-05-04 07:41:58.000000 bomf-0.4.0/src/bomf/validation/query_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-04 07:41:58.000000 bomf-0.4.0/src/bomf/validation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:42:05.392305 bomf-0.4.0/src/bomf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-05-04 07:42:05.000000 bomf-0.4.0/src/bomf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-04 07:42:05.000000 bomf-0.4.0/src/bomf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 07:42:05.000000 bomf-0.4.0/src/bomf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 07:42:05.000000 bomf-0.4.0/src/bomf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-04 07:42:05.000000 bomf-0.4.0/src/bomf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-04 07:42:05.000000 bomf-0.4.0/src/bomf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-05-04 07:41:58.000000 bomf-0.4.0/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:42:05.396305 bomf-0.4.0/unittests/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-04 07:41:58.000000 bomf-0.4.0/unittests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-04 07:41:58.000000 bomf-0.4.0/unittests/example_source_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-04 07:41:58.000000 bomf-0.4.0/unittests/test_bo4e_data_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-05-04 07:41:58.000000 bomf-0.4.0/unittests/test_entity_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-05-04 07:41:58.000000 bomf-0.4.0/unittests/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-05-04 07:41:58.000000 bomf-0.4.0/unittests/test_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-05-04 07:41:58.000000 bomf-0.4.0/unittests/test_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-05-04 07:41:58.000000 bomf-0.4.0/unittests/test_source_data_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    21326 2023-05-04 07:41:58.000000 bomf-0.4.0/unittests/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:55:32.431872 bomf-0.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:55:32.427872 bomf-0.4.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-04 07:55:24.000000 bomf-0.4.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:55:32.427872 bomf-0.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-04 07:55:24.000000 bomf-0.4.1/.github/workflows/black.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-05-04 07:55:24.000000 bomf-0.4.1/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-04 07:55:24.000000 bomf-0.4.1/.github/workflows/coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-04 07:55:24.000000 bomf-0.4.1/.github/workflows/no_byte_order_mark.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-04 07:55:24.000000 bomf-0.4.1/.github/workflows/packaging_test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-04 07:55:24.000000 bomf-0.4.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-04 07:55:24.000000 bomf-0.4.1/.github/workflows/pythonlint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-04 07:55:24.000000 bomf-0.4.1/.github/workflows/unittests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-04 07:55:24.000000 bomf-0.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-04 07:55:24.000000 bomf-0.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-04 07:55:24.000000 bomf-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-05-04 07:55:32.431872 bomf-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-05-04 07:55:24.000000 bomf-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-04 07:55:24.000000 bomf-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-04 07:55:24.000000 bomf-0.4.1/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-04 07:55:24.000000 bomf-0.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-04 07:55:32.431872 bomf-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-04 07:55:24.000000 bomf-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:55:32.427872 bomf-0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:55:32.427872 bomf-0.4.1/src/bomf/
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-05-04 07:55:24.000000 bomf-0.4.1/src/bomf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:55:32.427872 bomf-0.4.1/src/bomf/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-05-04 07:55:24.000000 bomf-0.4.1/src/bomf/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-05-04 07:55:24.000000 bomf-0.4.1/src/bomf/filter/sourcedataproviderfilter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:55:32.427872 bomf-0.4.1/src/bomf/loader/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-04 07:55:24.000000 bomf-0.4.1/src/bomf/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7670 2023-05-04 07:55:24.000000 bomf-0.4.1/src/bomf/loader/entityloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:55:32.427872 bomf-0.4.1/src/bomf/mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-04 07:55:24.000000 bomf-0.4.1/src/bomf/mapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:55:32.427872 bomf-0.4.1/src/bomf/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-05-04 07:55:24.000000 bomf-0.4.1/src/bomf/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:55:32.427872 bomf-0.4.1/src/bomf/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-05-04 07:55:24.000000 bomf-0.4.1/src/bomf/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-04 07:55:24.000000 bomf-0.4.1/src/bomf/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:55:32.427872 bomf-0.4.1/src/bomf/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-04 07:55:24.000000 bomf-0.4.1/src/bomf/validation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:55:32.431872 bomf-0.4.1/src/bomf/validation/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-04 07:55:24.000000 bomf-0.4.1/src/bomf/validation/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-05-04 07:55:24.000000 bomf-0.4.1/src/bomf/validation/core/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7640 2023-05-04 07:55:24.000000 bomf-0.4.1/src/bomf/validation/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17260 2023-05-04 07:55:24.000000 bomf-0.4.1/src/bomf/validation/core/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-04 07:55:24.000000 bomf-0.4.1/src/bomf/validation/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-04 07:55:24.000000 bomf-0.4.1/src/bomf/validation/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-05-04 07:55:24.000000 bomf-0.4.1/src/bomf/validation/core/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-05-04 07:55:24.000000 bomf-0.4.1/src/bomf/validation/path_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-05-04 07:55:24.000000 bomf-0.4.1/src/bomf/validation/query_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-04 07:55:24.000000 bomf-0.4.1/src/bomf/validation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:55:32.427872 bomf-0.4.1/src/bomf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-05-04 07:55:32.000000 bomf-0.4.1/src/bomf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-04 07:55:32.000000 bomf-0.4.1/src/bomf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 07:55:32.000000 bomf-0.4.1/src/bomf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 07:55:32.000000 bomf-0.4.1/src/bomf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-04 07:55:32.000000 bomf-0.4.1/src/bomf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-04 07:55:32.000000 bomf-0.4.1/src/bomf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-05-04 07:55:24.000000 bomf-0.4.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:55:32.431872 bomf-0.4.1/unittests/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-04 07:55:24.000000 bomf-0.4.1/unittests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-04 07:55:24.000000 bomf-0.4.1/unittests/example_source_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-04 07:55:24.000000 bomf-0.4.1/unittests/test_bo4e_data_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-05-04 07:55:24.000000 bomf-0.4.1/unittests/test_entity_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-05-04 07:55:24.000000 bomf-0.4.1/unittests/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-04 07:55:24.000000 bomf-0.4.1/unittests/test_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-05-04 07:55:24.000000 bomf-0.4.1/unittests/test_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-05-04 07:55:24.000000 bomf-0.4.1/unittests/test_source_data_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21292 2023-05-04 07:55:24.000000 bomf-0.4.1/unittests/test_validation.py
```

### Comparing `bomf-0.4.0/.github/dependabot.yml` & `bomf-0.4.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.4.0/.github/workflows/black.yml` & `bomf-0.4.1/.github/workflows/black.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.4.0/.github/workflows/codeql-analysis.yml` & `bomf-0.4.1/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.4.0/.github/workflows/coverage.yml` & `bomf-0.4.1/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.4.0/.github/workflows/packaging_test.yml` & `bomf-0.4.1/.github/workflows/packaging_test.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.4.0/.github/workflows/python-publish.yml` & `bomf-0.4.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.4.0/.github/workflows/pythonlint.yml` & `bomf-0.4.1/.github/workflows/pythonlint.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.4.0/.github/workflows/unittests.yml` & `bomf-0.4.1/.github/workflows/unittests.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.4.0/.gitignore` & `bomf-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `bomf-0.4.0/.pre-commit-config.yaml` & `bomf-0.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bomf-0.4.0/LICENSE` & `bomf-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bomf-0.4.0/PKG-INFO` & `bomf-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bomf
-Version: 0.4.0
+Version: 0.4.1
 Summary: BO4E Migration Framework
 Home-page: https://github.com/Hochfrequenz/bo4e_migration_framework
 Author: Hochfrequenz Unternehmensberatung GmbH
 Author-email: info@hochfrequenz.de
 License: mit
 Project-URL: Documentation, https://github.com/Hochfrequenz/bo4e_migration_framework
 Project-URL: Code, https://github.com/Hochfrequenz/bo4e_migration_framework
```

### Comparing `bomf-0.4.0/README.md` & `bomf-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `bomf-0.4.0/pyproject.toml` & `bomf-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bomf-0.4.0/requirements.txt` & `bomf-0.4.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `bomf-0.4.0/setup.cfg` & `bomf-0.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `bomf-0.4.0/src/bomf/__init__.py` & `bomf-0.4.1/src/bomf/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 BOMF stands for BO4E Migration Framework.
 """
 from abc import ABC
-from typing import Generic, List
+from typing import Generic
 
 import attrs
 
 from bomf.filter import Filter
 from bomf.loader.entityloader import EntityLoader, LoadingSummary
 from bomf.mapper import Bo4eDataSetToTargetMapper, IntermediateDataSet, SourceToBo4eDataSetMapper, TargetDataModel
 from bomf.provider import KeyTyp, SourceDataProvider
@@ -33,15 +33,15 @@
     a mapper that transforms bo4e data sets to a structure that suits the target system
     """
     target_loader: EntityLoader[TargetDataModel]
     """
     The target loader moves the target entities into the actual target system.
     """
 
-    async def migrate(self) -> List[LoadingSummary]:
+    async def migrate(self) -> list[LoadingSummary]:
         """
         run the entire migration flow from source to target which includes:
         1. create bo4e data source using the source_data_set_to_bo4e_mapper
         2. checking that all the bo4e data sets obey the validation rules
         3. mapping from bo4e to the target data model
         4. loading the target data models into the target system.
         """
```

### Comparing `bomf-0.4.0/src/bomf/filter/__init__.py` & `bomf-0.4.1/src/bomf/filter/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 # pylint:disable=too-few-public-methods
 
 import asyncio
 import logging
 from abc import ABC, abstractmethod
-from typing import Awaitable, Callable, Generic, List, Set, TypeVar
+from typing import Awaitable, Callable, Generic, TypeVar
 
 Candidate = TypeVar("Candidate")  #: an arbitrary but fixed type on which the filter operates
 
 
 class Filter(ABC, Generic[Candidate]):
     """
     A filter takes objects from candidates and returns only those that are relevant for its use case.
@@ -30,19 +30,19 @@
         depend on the data that you want to filter itself but on other things as well. The most obvious "other thing"
         is the data situation in the target system to which we migrate.
         If we migrate from system A to system B, then one possible filter is to check "does system B know my record"?
         These kind of questions are generally answered in an async way.
         """
         raise NotImplementedError("The inheriting class has to implement this method")
 
-    async def apply(self, candidates: List[Candidate]) -> List[Candidate]:
+    async def apply(self, candidates: list[Candidate]) -> list[Candidate]:
         """
         apply this filter on the candidates
         """
-        tasks: List[Awaitable[bool]] = [self.predicate(c) for c in candidates]
+        tasks: list[Awaitable[bool]] = [self.predicate(c) for c in candidates]
         self._logger.info("%s created %i predicate tasks; Awaiting them all", str(self), len(tasks))
         predicate_results = await asyncio.gather(*tasks)
         self._logger.info("%s awaited %i tasks", str(self), len(tasks))
         result = [
             c for c, predicate_match in zip(candidates, predicate_results, strict=True) if predicate_match is True
         ]
         candidates_removed = sum(1 for pr in predicate_results if pr is False)
@@ -71,29 +71,29 @@
         """
         Instantiate by providing a filter that is applied on the aggregate
         """
         self._logger = logging.getLogger(self.__module__)
         self._base_filter = base_filter
 
     @abstractmethod
-    async def aggregate(self, candidates: List[Candidate]) -> List[Aggregate]:
+    async def aggregate(self, candidates: list[Candidate]) -> list[Aggregate]:
         """
         Create aggregates which are then passed to the base filter that works on the aggregate.
         The method is async so that you can do complex (and e.g. network based) aggregations.
         """
         raise NotImplementedError("The inheriting class has to implement this method")
 
     @abstractmethod
     def disaggregate(self, aggregate: Aggregate) -> Candidate:
         """
         extract a single candidate from the aggregate that passed the filter
         """
         raise NotImplementedError("The inheriting class has to implement this method")
 
-    async def apply(self, candidates: List[Candidate]) -> List[Candidate]:
+    async def apply(self, candidates: list[Candidate]) -> list[Candidate]:
         """
         If aggregate and disaggregate and the base_filter are properly setup, then apply will filter the list of
         candidates based on the aggregate base filter.
         """
         aggregates = await self.aggregate(candidates)
         self._logger.info("There are %i candidates and %i aggregates", len(candidates), len(aggregates))
         filtered_aggregates = await self._base_filter.apply(aggregates)
@@ -105,15 +105,15 @@
 
 
 class HardcodedFilter(Filter[Candidate], ABC, Generic[Candidate, CandidateProperty]):
     """
     a harcoded filter filters on a hardcoded list of allowed/blocked values (formerly known as white- and blacklist)
     """
 
-    def __init__(self, criteria_selector: Callable[[Candidate], CandidateProperty], values: Set[CandidateProperty]):
+    def __init__(self, criteria_selector: Callable[[Candidate], CandidateProperty], values: set[CandidateProperty]):
         """
         instantiate by providing a criteria selector that returns a property on which we can filter and a set of values.
         Whether the values are used as allowed or not allowed (block) depends on the inheriting class
         """
         super().__init__()
         self._criteria_selector = criteria_selector
         self._values = values
```

### Comparing `bomf-0.4.0/src/bomf/filter/sourcedataproviderfilter.py` & `bomf-0.4.1/src/bomf/filter/sourcedataproviderfilter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Source Data Provider Filters combine the features of a filter with the features of a Source Data Provider.
 """
 
-from typing import Callable, Generic, List, Literal, Optional, overload
+from typing import Callable, Generic, Literal, Optional, overload
 
 from bomf import KeyTyp, SourceDataProvider
 from bomf.filter import Candidate, Filter
 from bomf.provider import JsonFileSourceDataProvider, ListBasedSourceDataProvider
 
 ASourceDataProvider = SourceDataProvider[Candidate, KeyTyp]
 
@@ -73,15 +73,15 @@
         data provider that only contains those entries that passed the filter (its predicate).
 
         If the provided source_data_provider is a JsonFileSourceDataProvider, then you don't have to provide a
         key_selector (let it default to None).
         However, in general, you have to specify how the data can be indexed using a key_selector which is not None.
         If you provide both a JsonFileSourceDataProvider AND a key_selector, the explicit key_selector will be used.
         """
-        survivors: List[Candidate] = await self._filter.apply(await source_data_provider.get_data())
+        survivors: list[Candidate] = await self._filter.apply(await source_data_provider.get_data())
         key_selector_to_be_used: Callable[[Candidate], KeyTyp]
         if key_selector is not None:
             key_selector_to_be_used = key_selector
         else:
             key_selector_to_be_used = source_data_provider.key_selector  # type:ignore[attr-defined]
             # if this raises an attribute error you have to
             # * either provide a source_data_provider which has a key_selector attribute
```

### Comparing `bomf-0.4.0/src/bomf/loader/entityloader.py` & `bomf-0.4.1/src/bomf/loader/entityloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 entity loaders load entities into the target system
 """
 import asyncio
 import json
 from abc import ABC, abstractmethod
 from datetime import datetime
 from pathlib import Path
-from typing import Awaitable, Callable, Generic, List, Optional, TypeVar
+from typing import Awaitable, Callable, Generic, Optional, TypeVar
 
 import attrs
 from pydantic import BaseModel  # pylint:disable=no-name-in-module
 
 _TargetEntity = TypeVar("_TargetEntity")
 
 
@@ -127,58 +127,58 @@
         return LoadingSummary(
             was_loaded_successfully=verification_result,
             verified_at=datetime.utcnow(),
             loaded_at=loaded_at,
             loading_error=None,
         )
 
-    async def load_entities(self, entities: List[_TargetEntity]) -> List[LoadingSummary]:
+    async def load_entities(self, entities: list[_TargetEntity]) -> list[LoadingSummary]:
         """
         load all the given entities into the target system
         """
         # here we could use some error handling in the future
-        tasks: List[Awaitable[LoadingSummary]] = [self.load(entity) for entity in entities]
+        tasks: list[Awaitable[LoadingSummary]] = [self.load(entity) for entity in entities]
         result = await asyncio.gather(*tasks)
         return result
 
 
 class JsonFileEntityLoader(EntityLoader[_TargetEntity], Generic[_TargetEntity]):
     """
     an entity loader that produces a json file as result. This is specifically useful in unit tests
     """
 
     async def verify(self, entity: _TargetEntity, id_in_target_system: Optional[str] = None) -> bool:
         return True
 
-    def __init__(self, file_path: Path, list_encoder: Callable[[List[_TargetEntity]], List[dict]]):
+    def __init__(self, file_path: Path, list_encoder: Callable[[list[_TargetEntity]], list[dict]]):
         """provide a path to a json file (will be created if not exists and overwritten if exists)"""
         self._file_path = file_path
         self._list_encoder = list_encoder
-        self._entities: List[_TargetEntity] = []
+        self._entities: list[_TargetEntity] = []
 
     async def load_entity(self, entity: _TargetEntity) -> Optional[EntityLoadingResult]:
         self._entities.append(entity)
         return None
 
-    async def load_entities(self, entities: List[_TargetEntity]) -> List[LoadingSummary]:
+    async def load_entities(self, entities: list[_TargetEntity]) -> list[LoadingSummary]:
         base_result = await super().load_entities(entities)
         dict_list = self._list_encoder(self._entities)
         with open(self._file_path, "w+", encoding="utf-8") as outfile:
             json.dump(dict_list, outfile, ensure_ascii=False, indent=2)
         return base_result
 
 
 _PydanticTargetModel = TypeVar("_PydanticTargetModel", bound=BaseModel)
 
 
 # pylint:disable=too-few-public-methods
 class _ListOfPydanticModels(BaseModel, Generic[_PydanticTargetModel]):
     # https://stackoverflow.com/a/58641115/10009545
     # for the instantiation see the serialization unit test
-    __root__: List[_PydanticTargetModel]
+    __root__: list[_PydanticTargetModel]
 
 
 class PydanticJsonFileEntityLoader(JsonFileEntityLoader[_PydanticTargetModel], Generic[_PydanticTargetModel]):
     """
     A json file entity loader specifically for pydantic models
     """
```

### Comparing `bomf-0.4.0/src/bomf/mapper/__init__.py` & `bomf-0.4.1/src/bomf/mapper/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 mappers convert from source data model to BO4E and from BO4E to a target data model
 """
 import asyncio
 from abc import ABC, abstractmethod
-from typing import Generic, List, TypeVar
+from typing import Generic, TypeVar
 
 from bomf.model import Bo4eDataSet
 
 TargetDataModel = TypeVar("TargetDataModel")
 """
 Target data model is the data model of the target (meaning: the data model of the system to which you'd like to migrate)
 """
@@ -25,15 +25,15 @@
     A mapper that maps one or multiple sources into Bo4eDataSets
     """
 
     # the inheriting class is free to combine and bundle the source data as it wants.
     # the only thing it has to provide is a method to create_data_sets (in bo4e).
     # we don't care from where it gets them in the first place
 
-    async def create_data_sets(self) -> List[IntermediateDataSet]:
+    async def create_data_sets(self) -> list[IntermediateDataSet]:
         """
         apply the mapping to all the provided source data sets.
 
         """
         raise NotImplementedError("The inheriting class has to implement this method")
 
 
@@ -45,14 +45,14 @@
 
     @abstractmethod
     async def create_target_model(self, dataset: IntermediateDataSet) -> TargetDataModel:
         """
         maps the given source data model into an intermediate data set
         """
 
-    async def create_target_models(self, datasets: List[IntermediateDataSet]) -> List[TargetDataModel]:
+    async def create_target_models(self, datasets: list[IntermediateDataSet]) -> list[TargetDataModel]:
         """
         apply the mapping to all the provided dataset
         """
         # here we could use some error handling in the future
         tasks = [self.create_target_model(dataset=dataset) for dataset in datasets]
         return await asyncio.gather(*tasks)
```

### Comparing `bomf-0.4.0/src/bomf/model/__init__.py` & `bomf-0.4.1/src/bomf/model/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.4.0/src/bomf/provider/__init__.py` & `bomf-0.4.1/src/bomf/provider/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 providers provide data
 """
 import json
 import logging
 from abc import ABC, abstractmethod
 from itertools import groupby
 from pathlib import Path
-from typing import Callable, Generic, List, Mapping, Optional, Protocol, TypeVar, Union
+from typing import Callable, Generic, Mapping, TypeVar, Union
 
 SourceDataModel = TypeVar("SourceDataModel")
 """
 Source data model is the data model of the source (meaning: the data model of the system from which the data originate).
 """
 
 KeyTyp = TypeVar("KeyTyp")
@@ -23,15 +23,15 @@
 class SourceDataProvider(ABC, Generic[SourceDataModel, KeyTyp]):
     """
     A source data provider provides entities from the source data system.
     The source data provider is thought to encapsulate data access behind a unified interface.
     """
 
     @abstractmethod
-    async def get_data(self) -> List[SourceDataModel]:
+    async def get_data(self) -> list[SourceDataModel]:
         """
         Returns all available entities from the source data model.
         They will be filtered in a SourceDataModel Filter ("Preselect")
         """
 
     @abstractmethod
     async def get_entry(self, key: KeyTyp) -> SourceDataModel:
@@ -42,19 +42,19 @@
 
 
 class ListBasedSourceDataProvider(SourceDataProvider[SourceDataModel, KeyTyp]):
     """
     A source data provider that is instantiated with a list of source data models
     """
 
-    def __init__(self, source_data_models: List[SourceDataModel], key_selector: Callable[[SourceDataModel], KeyTyp]):
+    def __init__(self, source_data_models: list[SourceDataModel], key_selector: Callable[[SourceDataModel], KeyTyp]):
         """
         instantiate it by providing a list of source data models
         """
-        self._models: List[SourceDataModel] = source_data_models
+        self._models: list[SourceDataModel] = source_data_models
         logger = logging.getLogger(self.__module__)
         for key, key_models in groupby(source_data_models, key=key_selector):
             affected_entries_count = len(list(key_models))
             if affected_entries_count > 1:
                 logger.warning(
                     "There are %i>1 entries for the key '%s'. You might miss entries because the key is not unique.",
                     affected_entries_count,
@@ -65,40 +65,40 @@
             "Read %i records from %s", len(self._models_dict), str(source_data_models)
         )
         self.key_selector = key_selector
 
     async def get_entry(self, key: KeyTyp) -> SourceDataModel:
         return self._models_dict[key]
 
-    async def get_data(self) -> List[SourceDataModel]:
+    async def get_data(self) -> list[SourceDataModel]:
         return self._models
 
 
 class JsonFileSourceDataProvider(SourceDataProvider[SourceDataModel, KeyTyp], Generic[SourceDataModel, KeyTyp]):
     """
     a source data model provider that is based on a JSON file
     """
 
     def __init__(
         self,
         json_file_path: Path,
-        data_selector: Callable[[Union[dict, list]], List[SourceDataModel]],
+        data_selector: Callable[[Union[dict, list]], list[SourceDataModel]],
         key_selector: Callable[[SourceDataModel], KeyTyp],
         encoding="utf-8",
     ):
         """
         initialize by providing a filepath to the json file and an accessor that describes the position of the data
         within the file.
         """
         with open(json_file_path, "r", encoding=encoding) as json_file:
             raw_data = json.load(json_file)
-        self._source_data_models: List[SourceDataModel] = data_selector(raw_data)
+        self._source_data_models: list[SourceDataModel] = data_selector(raw_data)
         self._key_to_data_model_mapping: Mapping[KeyTyp, SourceDataModel] = {
             key_selector(sdm): sdm for sdm in self._source_data_models
         }
         self.key_selector = key_selector
 
-    async def get_data(self) -> List[SourceDataModel]:
+    async def get_data(self) -> list[SourceDataModel]:
         return self._source_data_models
 
     async def get_entry(self, key: KeyTyp) -> SourceDataModel:
         return self._key_to_data_model_mapping[key]
```

### Comparing `bomf-0.4.0/src/bomf/validation/core/analysis.py` & `bomf-0.4.1/src/bomf/validation/core/analysis.py`

 * *Files identical despite different names*

### Comparing `bomf-0.4.0/src/bomf/validation/core/errors.py` & `bomf-0.4.1/src/bomf/validation/core/errors.py`

 * *Files identical despite different names*

### Comparing `bomf-0.4.0/src/bomf/validation/core/execution.py` & `bomf-0.4.1/src/bomf/validation/core/execution.py`

 * *Files identical despite different names*

### Comparing `bomf-0.4.0/src/bomf/validation/core/types.py` & `bomf-0.4.1/src/bomf/validation/core/types.py`

 * *Files identical despite different names*

### Comparing `bomf-0.4.0/src/bomf/validation/core/utils.py` & `bomf-0.4.1/src/bomf/validation/core/utils.py`

 * *Files identical despite different names*

### Comparing `bomf-0.4.0/src/bomf/validation/core/validator.py` & `bomf-0.4.1/src/bomf/validation/core/validator.py`

 * *Files identical despite different names*

### Comparing `bomf-0.4.0/src/bomf/validation/path_map.py` & `bomf-0.4.1/src/bomf/validation/path_map.py`

 * *Files identical despite different names*

### Comparing `bomf-0.4.0/src/bomf/validation/query_map.py` & `bomf-0.4.1/src/bomf/validation/query_map.py`

 * *Files identical despite different names*

### Comparing `bomf-0.4.0/src/bomf/validation/utils.py` & `bomf-0.4.1/src/bomf/validation/utils.py`

 * *Files identical despite different names*

### Comparing `bomf-0.4.0/src/bomf.egg-info/PKG-INFO` & `bomf-0.4.1/src/bomf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bomf
-Version: 0.4.0
+Version: 0.4.1
 Summary: BO4E Migration Framework
 Home-page: https://github.com/Hochfrequenz/bo4e_migration_framework
 Author: Hochfrequenz Unternehmensberatung GmbH
 Author-email: info@hochfrequenz.de
 License: mit
 Project-URL: Documentation, https://github.com/Hochfrequenz/bo4e_migration_framework
 Project-URL: Code, https://github.com/Hochfrequenz/bo4e_migration_framework
```

### Comparing `bomf-0.4.0/src/bomf.egg-info/SOURCES.txt` & `bomf-0.4.1/src/bomf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bomf-0.4.0/tox.ini` & `bomf-0.4.1/tox.ini`

 * *Files identical despite different names*

### Comparing `bomf-0.4.0/unittests/test_bo4e_data_set.py` & `bomf-0.4.1/unittests/test_bo4e_data_set.py`

 * *Files identical despite different names*

### Comparing `bomf-0.4.0/unittests/test_entity_loader.py` & `bomf-0.4.1/unittests/test_entity_loader.py`

 * *Files identical despite different names*

### Comparing `bomf-0.4.0/unittests/test_filter.py` & `bomf-0.4.1/unittests/test_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import dataclasses
 import logging
 from itertools import groupby
-from typing import List
 
 import pytest  # type:ignore[import]
 
 from bomf.filter import AggregateFilter, AllowlistFilter, BlocklistFilter, Filter
 from bomf.filter.sourcedataproviderfilter import SourceDataProviderFilter
 from bomf.provider import ListBasedSourceDataProvider, SourceDataProvider
 
@@ -22,15 +21,15 @@
             pytest.param(
                 _FooFilter(),
                 [{"foo": "baz"}, {"foo": "bar"}],
                 [{"foo": "bar"}],
             ),
         ],
     )
-    async def test_filter(self, filter_under_test: Filter, candidates: List[dict], survivors: List[dict], caplog):
+    async def test_filter(self, filter_under_test: Filter, candidates: list[dict], survivors: list[dict], caplog):
         caplog.set_level(logging.DEBUG, logger=self.__module__)
         actual = await filter_under_test.apply(candidates)
         assert actual == survivors
         assert "1 out of 2 candidates have been removed by the filter" in caplog.messages
 
 
 @dataclasses.dataclass
@@ -57,16 +56,16 @@
         class _BaseFilter(Filter[_MyAggregate]):
             async def predicate(self, candidate: _MyAggregate) -> bool:
                 return candidate.max_number_for_key == candidate.candidate.number
 
         base_filter = _BaseFilter()
         super(_BarFilter, self).__init__(base_filter)
 
-    async def aggregate(self, candidates: List[_MyCandidate]) -> List[_MyAggregate]:
-        result: List[_MyAggregate] = []
+    async def aggregate(self, candidates: list[_MyCandidate]) -> list[_MyAggregate]:
+        result: list[_MyAggregate] = []
         for group_key, group in groupby(sorted(candidates, key=lambda c: c.string), lambda c: c.string):
             group_items = list(group)
             max_number_in_group = max(group_item.number for group_item in group_items)
             for group_item in group_items:
                 result.append(
                     _MyAggregate(group_key=group_key, max_number_for_key=max_number_in_group, candidate=group_item)
                 )
@@ -89,34 +88,34 @@
                     _MyCandidate(number=17, string="bar"),
                 ],
                 [_MyCandidate(number=19, string="bar"), _MyCandidate(number=2, string="foo")],
             ),
         ],
     )
     async def test_aggregate_filter(
-        self, filter_under_test: AggregateFilter, candidates: List[dict], survivors: List[dict], caplog
+        self, filter_under_test: AggregateFilter, candidates: list[dict], survivors: list[dict], caplog
     ):
         caplog.set_level(logging.DEBUG, logger=self.__module__)
         actual = await filter_under_test.apply(candidates)
         assert actual == survivors
         assert "There are 4 candidates and 4 aggregates" in caplog.messages
         assert "There are 2 filtered aggregates left" in caplog.messages
 
 
 class TestBlockAndAllowlistFilter:
     async def test_allowlist_filter(self):
         allowlist = {"A", "B", "C"}
-        candidates: List[dict[str, str]] = [{"foo": "A"}, {"foo": "B"}, {"foo": "Z"}]
+        candidates: list[dict[str, str]] = [{"foo": "A"}, {"foo": "B"}, {"foo": "Z"}]
         allowlist_filter: AllowlistFilter[dict[str, str], str] = AllowlistFilter(lambda c: c["foo"], allowlist)
         actual = await allowlist_filter.apply(candidates)
         assert actual == [{"foo": "A"}, {"foo": "B"}]
 
     async def test_blocklist_filter(self):
         blocklist = {"A", "B", "C"}
-        candidates: List[dict[str, str]] = [{"foo": "A"}, {"foo": "B"}, {"foo": "Z"}]
+        candidates: list[dict[str, str]] = [{"foo": "A"}, {"foo": "B"}, {"foo": "Z"}]
         blocklist_filter: BlocklistFilter[dict[str, str], str] = BlocklistFilter(lambda c: c["foo"], blocklist)
         actual = await blocklist_filter.apply(candidates)
         assert actual == [{"foo": "Z"}]
 
 
 class TestSourceDataProviderFilter:
     @pytest.mark.parametrize(
@@ -133,16 +132,16 @@
                 [_MyCandidate(number=19, string="bar"), _MyCandidate(number=2, string="foo")],
             ),
         ],
     )
     async def test_source_data_provider_filter(
         self,
         candidate_filter: Filter[_MyCandidate],
-        candidates: List[_MyCandidate],
-        survivors: List[_MyCandidate],
+        candidates: list[_MyCandidate],
+        survivors: list[_MyCandidate],
         caplog,
     ):
         my_provider: ListBasedSourceDataProvider[_MyCandidate, int] = ListBasedSourceDataProvider(
             candidates, key_selector=lambda mc: mc.number
         )
         sdp_filter: SourceDataProviderFilter[_MyCandidate, int] = SourceDataProviderFilter(candidate_filter)
         caplog.set_level(logging.DEBUG, logger=self.__module__)
```

### Comparing `bomf-0.4.0/unittests/test_mapper.py` & `bomf-0.4.1/unittests/test_mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Optional, Type
+from typing import Optional, Type
 
 import attrs
 import pytest  # type:ignore[import]
 from bo4e.bo.marktlokation import Marktlokation
 from bo4e.bo.messlokation import Messlokation
 
 from bomf.mapper import Bo4eDataSetToTargetMapper, SourceToBo4eDataSetMapper
@@ -34,26 +34,26 @@
 # - the source data model is a dictionary
 # - the intermediate data model are BO4E MaLo and MeLo
 # - the target data model is a list of string
 # This is just to demonstrate the mapping structures.
 
 
 class _DictToMaLoMeLoMapper(SourceToBo4eDataSetMapper):
-    async def create_data_sets(self) -> List[_MaLoAndMeLo]:
+    async def create_data_sets(self) -> list[_MaLoAndMeLo]:
         return [
             _MaLoAndMeLo(
                 melo=Messlokation.construct(messlokations_id=source["meloId"]),
                 malo=Marktlokation.construct(marktlokations_id=source["maloId"]),
             )
             for source in [{"maloId": "54321012345", "meloId": "DE000111222333"}]
         ]
 
 
 class _MaLoMeLoToListMapper(Bo4eDataSetToTargetMapper):
-    async def create_target_model(self, dataset: _MaLoAndMeLo) -> List[str]:
+    async def create_target_model(self, dataset: _MaLoAndMeLo) -> list[str]:
         return [
             dataset.get_business_object(Marktlokation).marktlokations_id,
             dataset.get_business_object(Messlokation).messlokations_id,
         ]
 
 
 class TestMapper:
```

### Comparing `bomf-0.4.0/unittests/test_migration.py` & `bomf-0.4.1/unittests/test_migration.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 """
 Tests the overall data flow using bomf.
 """
-import asyncio
-from typing import Dict, List, Optional
-
-import attrs
+from typing import Optional
 
 from bomf import (
     Bo4eDataSetToTargetMapper,
     EntityLoader,
     Filter,
     MigrationStrategy,
     SourceDataProvider,
@@ -18,31 +15,31 @@
 from bomf.loader.entityloader import EntityLoadingResult
 from bomf.model import Bo4eDataSet
 from bomf.provider import KeyTyp
 from bomf.validation import Validator
 from bomf.validation.core import SyncValidatorFunction
 from bomf.validation.path_map import PathMappedValidator
 
-_MySourceDataModel = Dict[str, str]
+_MySourceDataModel = dict[str, str]
 _MyKeyTyp = str
-_MyTargetDataModel = List[str]
+_MyTargetDataModel = list[str]
 
 
 class _MyIntermediateDataModel(Bo4eDataSet):
-    data: Dict[str, str]
+    data: dict[str, str]
 
     def get_id(self) -> str:
         return "12345"
 
 
 class _MySourceDataProvider(SourceDataProvider[_MySourceDataModel, _MyKeyTyp]):
     async def get_entry(self, key: KeyTyp) -> _MySourceDataModel:
         raise NotImplementedError("Not relevant for the test")
 
-    async def get_data(self) -> List[_MySourceDataModel]:
+    async def get_data(self) -> list[_MySourceDataModel]:
         return [
             {"foo": "bar"},
             {"FOO": "BAR"},
             {"Foo": "Bar"},
             {"remove by filter": "should not pass the filter"},
             # {"invalid": "doesn't matter"},
         ]
@@ -50,19 +47,19 @@
 
 class _MyFilter(Filter[_MySourceDataModel]):
     async def predicate(self, candidate: _MySourceDataModel) -> bool:
         return "remove by filter" not in candidate
 
 
 class _MyToBo4eMapper(SourceToBo4eDataSetMapper[_MyIntermediateDataModel]):
-    def __init__(self, what_ever_you_like: List[_MySourceDataModel]):
+    def __init__(self, what_ever_you_like: list[_MySourceDataModel]):
         # what_ever_you_like is a place holde for all the relation magic that may happen
         self._source_models = what_ever_you_like
 
-    async def create_data_sets(self) -> List[_MyIntermediateDataModel]:
+    async def create_data_sets(self) -> list[_MyIntermediateDataModel]:
         return [_MyIntermediateDataModel(data=source) for source in self._source_models]
 
 
 def _my_rule(data: dict[str, str]):
     if "invalid" in data:
         raise ValueError("'invalid' in data")
```

### Comparing `bomf-0.4.0/unittests/test_source_data_provider.py` & `bomf-0.4.1/unittests/test_source_data_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import logging
 from pathlib import Path
-from typing import List
 
 import pytest  # type:ignore[import]
 
 from bomf.provider import JsonFileSourceDataProvider, KeyTyp, ListBasedSourceDataProvider, SourceDataProvider
 
 
 class LegacyDataSystemDataProvider(SourceDataProvider):
     """
     a dummy for access to a legacy system from which we want to migrate data
     """
 
     async def get_entry(self, key: KeyTyp) -> str:
         raise NotImplementedError("Not relevant for this test")
 
-    async def get_data(self) -> List[str]:
+    async def get_data(self) -> list[str]:
         return ["foo", "bar", "baz"]
 
 
 class TestSourceDataProvider:
     async def test_provider(self):
         # this is a pretty dumb test
         provider_under_test = LegacyDataSystemDataProvider()
```

### Comparing `bomf-0.4.0/unittests/test_validation.py` & `bomf-0.4.1/unittests/test_validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import asyncio
 import re
 from datetime import timedelta
 from typing import Any, Iterator, Optional
 
 import pytest
-from frozendict import frozendict
 from pydantic import BaseModel, Required
 
 from bomf import ValidationManager
 from bomf.model import Bo4eDataSet
 from bomf.validation import Query, QueryMappedValidator, Validator, optional_field, param, required_field
 from bomf.validation.core import ValidationError, ValidatorFunctionT
 from bomf.validation.core.types import (
```

