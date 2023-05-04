# Comparing `tmp/bomf-0.3.1.tar.gz` & `tmp/bomf-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bomf-0.3.1.tar", last modified: Tue May  2 13:09:44 2023, max compression
+gzip compressed data, was "bomf-0.4.0.tar", last modified: Thu May  4 07:42:05 2023, max compression
```

## Comparing `bomf-0.3.1.tar` & `bomf-0.4.0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:09:44.324510 bomf-0.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:09:44.320510 bomf-0.3.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-02 13:09:37.000000 bomf-0.3.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:09:44.320510 bomf-0.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-02 13:09:37.000000 bomf-0.3.1/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-05-02 13:09:37.000000 bomf-0.3.1/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-02 13:09:37.000000 bomf-0.3.1/.github/workflows/coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-02 13:09:37.000000 bomf-0.3.1/.github/workflows/no_byte_order_mark.yml
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-02 13:09:37.000000 bomf-0.3.1/.github/workflows/packaging_test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-02 13:09:37.000000 bomf-0.3.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-02 13:09:37.000000 bomf-0.3.1/.github/workflows/pythonlint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-02 13:09:37.000000 bomf-0.3.1/.github/workflows/unittests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-02 13:09:37.000000 bomf-0.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-02 13:09:37.000000 bomf-0.3.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-02 13:09:37.000000 bomf-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-05-02 13:09:44.324510 bomf-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-05-02 13:09:37.000000 bomf-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-02 13:09:37.000000 bomf-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-02 13:09:37.000000 bomf-0.3.1/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-02 13:09:37.000000 bomf-0.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-02 13:09:44.324510 bomf-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-02 13:09:37.000000 bomf-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:09:44.316510 bomf-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:09:44.320510 bomf-0.3.1/src/bomf/
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-05-02 13:09:37.000000 bomf-0.3.1/src/bomf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:09:44.320510 bomf-0.3.1/src/bomf/filter/
--rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-05-02 13:09:37.000000 bomf-0.3.1/src/bomf/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-05-02 13:09:37.000000 bomf-0.3.1/src/bomf/filter/sourcedataproviderfilter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:09:44.320510 bomf-0.3.1/src/bomf/loader/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-02 13:09:37.000000 bomf-0.3.1/src/bomf/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-05-02 13:09:37.000000 bomf-0.3.1/src/bomf/loader/entityloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:09:44.320510 bomf-0.3.1/src/bomf/mapper/
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-02 13:09:37.000000 bomf-0.3.1/src/bomf/mapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:09:44.320510 bomf-0.3.1/src/bomf/model/
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-05-02 13:09:37.000000 bomf-0.3.1/src/bomf/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:09:44.320510 bomf-0.3.1/src/bomf/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-05-02 13:09:37.000000 bomf-0.3.1/src/bomf/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-02 13:09:37.000000 bomf-0.3.1/src/bomf/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:09:44.320510 bomf-0.3.1/src/bomf/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-02 13:09:37.000000 bomf-0.3.1/src/bomf/validation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:09:44.324510 bomf-0.3.1/src/bomf/validation/core/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-02 13:09:37.000000 bomf-0.3.1/src/bomf/validation/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-05-02 13:09:37.000000 bomf-0.3.1/src/bomf/validation/core/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     7640 2023-05-02 13:09:37.000000 bomf-0.3.1/src/bomf/validation/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    17260 2023-05-02 13:09:37.000000 bomf-0.3.1/src/bomf/validation/core/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-02 13:09:37.000000 bomf-0.3.1/src/bomf/validation/core/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-02 13:09:37.000000 bomf-0.3.1/src/bomf/validation/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-05-02 13:09:37.000000 bomf-0.3.1/src/bomf/validation/core/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-05-02 13:09:37.000000 bomf-0.3.1/src/bomf/validation/path_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-05-02 13:09:37.000000 bomf-0.3.1/src/bomf/validation/query_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-02 13:09:37.000000 bomf-0.3.1/src/bomf/validation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:09:44.320510 bomf-0.3.1/src/bomf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-05-02 13:09:44.000000 bomf-0.3.1/src/bomf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-02 13:09:44.000000 bomf-0.3.1/src/bomf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 13:09:44.000000 bomf-0.3.1/src/bomf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 13:09:44.000000 bomf-0.3.1/src/bomf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-02 13:09:44.000000 bomf-0.3.1/src/bomf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-02 13:09:44.000000 bomf-0.3.1/src/bomf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-05-02 13:09:37.000000 bomf-0.3.1/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:09:44.324510 bomf-0.3.1/unittests/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-02 13:09:37.000000 bomf-0.3.1/unittests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-02 13:09:37.000000 bomf-0.3.1/unittests/example_source_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-02 13:09:37.000000 bomf-0.3.1/unittests/test_bo4e_data_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-05-02 13:09:37.000000 bomf-0.3.1/unittests/test_entity_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-05-02 13:09:37.000000 bomf-0.3.1/unittests/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-05-02 13:09:37.000000 bomf-0.3.1/unittests/test_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-05-02 13:09:37.000000 bomf-0.3.1/unittests/test_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-05-02 13:09:37.000000 bomf-0.3.1/unittests/test_source_data_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    21326 2023-05-02 13:09:37.000000 bomf-0.3.1/unittests/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:42:05.396305 bomf-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:42:05.392305 bomf-0.4.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-04 07:41:58.000000 bomf-0.4.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:42:05.392305 bomf-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-04 07:41:58.000000 bomf-0.4.0/.github/workflows/black.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-05-04 07:41:58.000000 bomf-0.4.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-04 07:41:58.000000 bomf-0.4.0/.github/workflows/coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-04 07:41:58.000000 bomf-0.4.0/.github/workflows/no_byte_order_mark.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-04 07:41:58.000000 bomf-0.4.0/.github/workflows/packaging_test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-04 07:41:58.000000 bomf-0.4.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-04 07:41:58.000000 bomf-0.4.0/.github/workflows/pythonlint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-04 07:41:58.000000 bomf-0.4.0/.github/workflows/unittests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-04 07:41:58.000000 bomf-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-04 07:41:58.000000 bomf-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-04 07:41:58.000000 bomf-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-05-04 07:42:05.396305 bomf-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-05-04 07:41:58.000000 bomf-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-04 07:41:58.000000 bomf-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-04 07:41:58.000000 bomf-0.4.0/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-04 07:41:58.000000 bomf-0.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-04 07:42:05.396305 bomf-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-04 07:41:58.000000 bomf-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:42:05.388305 bomf-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:42:05.392305 bomf-0.4.0/src/bomf/
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-05-04 07:41:58.000000 bomf-0.4.0/src/bomf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:42:05.392305 bomf-0.4.0/src/bomf/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-05-04 07:41:58.000000 bomf-0.4.0/src/bomf/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-05-04 07:41:58.000000 bomf-0.4.0/src/bomf/filter/sourcedataproviderfilter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:42:05.392305 bomf-0.4.0/src/bomf/loader/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-04 07:41:58.000000 bomf-0.4.0/src/bomf/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-05-04 07:41:58.000000 bomf-0.4.0/src/bomf/loader/entityloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:42:05.392305 bomf-0.4.0/src/bomf/mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-04 07:41:58.000000 bomf-0.4.0/src/bomf/mapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:42:05.392305 bomf-0.4.0/src/bomf/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-05-04 07:41:58.000000 bomf-0.4.0/src/bomf/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:42:05.392305 bomf-0.4.0/src/bomf/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-05-04 07:41:58.000000 bomf-0.4.0/src/bomf/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-04 07:41:58.000000 bomf-0.4.0/src/bomf/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:42:05.392305 bomf-0.4.0/src/bomf/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-04 07:41:58.000000 bomf-0.4.0/src/bomf/validation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:42:05.392305 bomf-0.4.0/src/bomf/validation/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-04 07:41:58.000000 bomf-0.4.0/src/bomf/validation/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-05-04 07:41:58.000000 bomf-0.4.0/src/bomf/validation/core/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7640 2023-05-04 07:41:58.000000 bomf-0.4.0/src/bomf/validation/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17260 2023-05-04 07:41:58.000000 bomf-0.4.0/src/bomf/validation/core/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-04 07:41:58.000000 bomf-0.4.0/src/bomf/validation/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-04 07:41:58.000000 bomf-0.4.0/src/bomf/validation/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-05-04 07:41:58.000000 bomf-0.4.0/src/bomf/validation/core/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-05-04 07:41:58.000000 bomf-0.4.0/src/bomf/validation/path_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-05-04 07:41:58.000000 bomf-0.4.0/src/bomf/validation/query_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-04 07:41:58.000000 bomf-0.4.0/src/bomf/validation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:42:05.392305 bomf-0.4.0/src/bomf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-05-04 07:42:05.000000 bomf-0.4.0/src/bomf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-04 07:42:05.000000 bomf-0.4.0/src/bomf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 07:42:05.000000 bomf-0.4.0/src/bomf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 07:42:05.000000 bomf-0.4.0/src/bomf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-04 07:42:05.000000 bomf-0.4.0/src/bomf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-04 07:42:05.000000 bomf-0.4.0/src/bomf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-05-04 07:41:58.000000 bomf-0.4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:42:05.396305 bomf-0.4.0/unittests/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-04 07:41:58.000000 bomf-0.4.0/unittests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-04 07:41:58.000000 bomf-0.4.0/unittests/example_source_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-04 07:41:58.000000 bomf-0.4.0/unittests/test_bo4e_data_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-05-04 07:41:58.000000 bomf-0.4.0/unittests/test_entity_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-05-04 07:41:58.000000 bomf-0.4.0/unittests/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-05-04 07:41:58.000000 bomf-0.4.0/unittests/test_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-05-04 07:41:58.000000 bomf-0.4.0/unittests/test_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-05-04 07:41:58.000000 bomf-0.4.0/unittests/test_source_data_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21326 2023-05-04 07:41:58.000000 bomf-0.4.0/unittests/test_validation.py
```

### Comparing `bomf-0.3.1/.github/dependabot.yml` & `bomf-0.4.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.3.1/.github/workflows/black.yml` & `bomf-0.4.0/.github/workflows/black.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.3.1/.github/workflows/codeql-analysis.yml` & `bomf-0.4.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.3.1/.github/workflows/coverage.yml` & `bomf-0.4.0/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.3.1/.github/workflows/packaging_test.yml` & `bomf-0.4.0/.github/workflows/packaging_test.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.3.1/.github/workflows/python-publish.yml` & `bomf-0.4.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.3.1/.github/workflows/pythonlint.yml` & `bomf-0.4.0/.github/workflows/pythonlint.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.3.1/.github/workflows/unittests.yml` & `bomf-0.4.0/.github/workflows/unittests.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.3.1/.gitignore` & `bomf-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `bomf-0.3.1/.pre-commit-config.yaml` & `bomf-0.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bomf-0.3.1/LICENSE` & `bomf-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bomf-0.3.1/PKG-INFO` & `bomf-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bomf
-Version: 0.3.1
+Version: 0.4.0
 Summary: BO4E Migration Framework
 Home-page: https://github.com/Hochfrequenz/bo4e_migration_framework
 Author: Hochfrequenz Unternehmensberatung GmbH
 Author-email: info@hochfrequenz.de
 License: mit
 Project-URL: Documentation, https://github.com/Hochfrequenz/bo4e_migration_framework
 Project-URL: Code, https://github.com/Hochfrequenz/bo4e_migration_framework
```

### Comparing `bomf-0.3.1/README.md` & `bomf-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `bomf-0.3.1/pyproject.toml` & `bomf-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bomf-0.3.1/requirements.txt` & `bomf-0.4.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `bomf-0.3.1/setup.cfg` & `bomf-0.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `bomf-0.3.1/src/bomf/__init__.py` & `bomf-0.4.0/src/bomf/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.3.1/src/bomf/filter/__init__.py` & `bomf-0.4.0/src/bomf/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.3.1/src/bomf/filter/sourcedataproviderfilter.py` & `bomf-0.4.0/src/bomf/filter/sourcedataproviderfilter.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         data provider that only contains those entries that passed the filter (its predicate).
 
         If the provided source_data_provider is a JsonFileSourceDataProvider, then you don't have to provide a
         key_selector (let it default to None).
         However, in general, you have to specify how the data can be indexed using a key_selector which is not None.
         If you provide both a JsonFileSourceDataProvider AND a key_selector, the explicit key_selector will be used.
         """
-        survivors: List[Candidate] = await self._filter.apply(source_data_provider.get_data())
+        survivors: List[Candidate] = await self._filter.apply(await source_data_provider.get_data())
         key_selector_to_be_used: Callable[[Candidate], KeyTyp]
         if key_selector is not None:
             key_selector_to_be_used = key_selector
         else:
             key_selector_to_be_used = source_data_provider.key_selector  # type:ignore[attr-defined]
             # if this raises an attribute error you have to
             # * either provide a source_data_provider which has a key_selector attribute
```

### Comparing `bomf-0.3.1/src/bomf/loader/entityloader.py` & `bomf-0.4.0/src/bomf/loader/entityloader.py`

 * *Files identical despite different names*

### Comparing `bomf-0.3.1/src/bomf/mapper/__init__.py` & `bomf-0.4.0/src/bomf/mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.3.1/src/bomf/model/__init__.py` & `bomf-0.4.0/src/bomf/model/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.3.1/src/bomf/provider/__init__.py` & `bomf-0.4.0/src/bomf/provider/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,22 +23,22 @@
 class SourceDataProvider(ABC, Generic[SourceDataModel, KeyTyp]):
     """
     A source data provider provides entities from the source data system.
     The source data provider is thought to encapsulate data access behind a unified interface.
     """
 
     @abstractmethod
-    def get_data(self) -> List[SourceDataModel]:
+    async def get_data(self) -> List[SourceDataModel]:
         """
         Returns all available entities from the source data model.
         They will be filtered in a SourceDataModel Filter ("Preselect")
         """
 
     @abstractmethod
-    def get_entry(self, key: KeyTyp) -> SourceDataModel:
+    async def get_entry(self, key: KeyTyp) -> SourceDataModel:
         """
         returns the source data model which has key as key.
         raises an error if the key is unknown
         """
 
 
 class ListBasedSourceDataProvider(SourceDataProvider[SourceDataModel, KeyTyp]):
@@ -62,18 +62,18 @@
                 )
         self._models_dict: Mapping[KeyTyp, SourceDataModel] = {key_selector(m): m for m in source_data_models}
         logging.getLogger(self.__module__).info(
             "Read %i records from %s", len(self._models_dict), str(source_data_models)
         )
         self.key_selector = key_selector
 
-    def get_entry(self, key: KeyTyp) -> SourceDataModel:
+    async def get_entry(self, key: KeyTyp) -> SourceDataModel:
         return self._models_dict[key]
 
-    def get_data(self) -> List[SourceDataModel]:
+    async def get_data(self) -> List[SourceDataModel]:
         return self._models
 
 
 class JsonFileSourceDataProvider(SourceDataProvider[SourceDataModel, KeyTyp], Generic[SourceDataModel, KeyTyp]):
     """
     a source data model provider that is based on a JSON file
     """
@@ -93,12 +93,12 @@
             raw_data = json.load(json_file)
         self._source_data_models: List[SourceDataModel] = data_selector(raw_data)
         self._key_to_data_model_mapping: Mapping[KeyTyp, SourceDataModel] = {
             key_selector(sdm): sdm for sdm in self._source_data_models
         }
         self.key_selector = key_selector
 
-    def get_data(self) -> List[SourceDataModel]:
+    async def get_data(self) -> List[SourceDataModel]:
         return self._source_data_models
 
-    def get_entry(self, key: KeyTyp) -> SourceDataModel:
+    async def get_entry(self, key: KeyTyp) -> SourceDataModel:
         return self._key_to_data_model_mapping[key]
```

### Comparing `bomf-0.3.1/src/bomf/validation/core/__init__.py` & `bomf-0.4.0/src/bomf/validation/core/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.3.1/src/bomf/validation/core/analysis.py` & `bomf-0.4.0/src/bomf/validation/core/analysis.py`

 * *Files identical despite different names*

### Comparing `bomf-0.3.1/src/bomf/validation/core/errors.py` & `bomf-0.4.0/src/bomf/validation/core/errors.py`

 * *Files identical despite different names*

### Comparing `bomf-0.3.1/src/bomf/validation/core/execution.py` & `bomf-0.4.0/src/bomf/validation/core/execution.py`

 * *Files identical despite different names*

### Comparing `bomf-0.3.1/src/bomf/validation/core/types.py` & `bomf-0.4.0/src/bomf/validation/core/types.py`

 * *Files identical despite different names*

### Comparing `bomf-0.3.1/src/bomf/validation/core/utils.py` & `bomf-0.4.0/src/bomf/validation/core/utils.py`

 * *Files identical despite different names*

### Comparing `bomf-0.3.1/src/bomf/validation/core/validator.py` & `bomf-0.4.0/src/bomf/validation/core/validator.py`

 * *Files identical despite different names*

### Comparing `bomf-0.3.1/src/bomf/validation/path_map.py` & `bomf-0.4.0/src/bomf/validation/path_map.py`

 * *Files identical despite different names*

### Comparing `bomf-0.3.1/src/bomf/validation/query_map.py` & `bomf-0.4.0/src/bomf/validation/query_map.py`

 * *Files identical despite different names*

### Comparing `bomf-0.3.1/src/bomf/validation/utils.py` & `bomf-0.4.0/src/bomf/validation/utils.py`

 * *Files identical despite different names*

### Comparing `bomf-0.3.1/src/bomf.egg-info/PKG-INFO` & `bomf-0.4.0/src/bomf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bomf
-Version: 0.3.1
+Version: 0.4.0
 Summary: BO4E Migration Framework
 Home-page: https://github.com/Hochfrequenz/bo4e_migration_framework
 Author: Hochfrequenz Unternehmensberatung GmbH
 Author-email: info@hochfrequenz.de
 License: mit
 Project-URL: Documentation, https://github.com/Hochfrequenz/bo4e_migration_framework
 Project-URL: Code, https://github.com/Hochfrequenz/bo4e_migration_framework
```

### Comparing `bomf-0.3.1/src/bomf.egg-info/SOURCES.txt` & `bomf-0.4.0/src/bomf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bomf-0.3.1/tox.ini` & `bomf-0.4.0/tox.ini`

 * *Files identical despite different names*

### Comparing `bomf-0.3.1/unittests/test_bo4e_data_set.py` & `bomf-0.4.0/unittests/test_bo4e_data_set.py`

 * *Files identical despite different names*

### Comparing `bomf-0.3.1/unittests/test_entity_loader.py` & `bomf-0.4.0/unittests/test_entity_loader.py`

 * *Files identical despite different names*

### Comparing `bomf-0.3.1/unittests/test_filter.py` & `bomf-0.4.0/unittests/test_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,15 +144,15 @@
         my_provider: ListBasedSourceDataProvider[_MyCandidate, int] = ListBasedSourceDataProvider(
             candidates, key_selector=lambda mc: mc.number
         )
         sdp_filter: SourceDataProviderFilter[_MyCandidate, int] = SourceDataProviderFilter(candidate_filter)
         caplog.set_level(logging.DEBUG, logger=self.__module__)
         filtered_provider = await sdp_filter.apply(my_provider)
         assert isinstance(filtered_provider, SourceDataProvider)
-        actual = filtered_provider.get_data()
+        actual = await filtered_provider.get_data()
         assert actual == survivors
         assert "There are 4 candidates and 4 aggregates" in caplog.messages
         assert "There are 2 filtered aggregates left" in caplog.messages
 
     async def test_source_data_provider_filter_error(self):
         my_provider: ListBasedSourceDataProvider[dict, str] = ListBasedSourceDataProvider(
             [{"foo": "bar"}, {"foo": "notbar"}], key_selector=lambda d: d["foo"]
```

### Comparing `bomf-0.3.1/unittests/test_mapper.py` & `bomf-0.4.0/unittests/test_mapper.py`

 * *Files identical despite different names*

### Comparing `bomf-0.3.1/unittests/test_migration.py` & `bomf-0.4.0/unittests/test_migration.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,18 +31,18 @@
     data: Dict[str, str]
 
     def get_id(self) -> str:
         return "12345"
 
 
 class _MySourceDataProvider(SourceDataProvider[_MySourceDataModel, _MyKeyTyp]):
-    def get_entry(self, key: KeyTyp) -> _MySourceDataModel:
+    async def get_entry(self, key: KeyTyp) -> _MySourceDataModel:
         raise NotImplementedError("Not relevant for the test")
 
-    def get_data(self) -> List[_MySourceDataModel]:
+    async def get_data(self) -> List[_MySourceDataModel]:
         return [
             {"foo": "bar"},
             {"FOO": "BAR"},
             {"Foo": "Bar"},
             {"remove by filter": "should not pass the filter"},
             # {"invalid": "doesn't matter"},
         ]
@@ -100,15 +100,15 @@
 class TestMigrationStrategy:
     """
     This is more of an integration than a unit test. All the single components come together here.
     """
 
     async def test_happy_path(self):
         # here's some pre-processing, you can read some data, you can create relations, whatever
-        raw_data = _MySourceDataProvider().get_data()
+        raw_data = await _MySourceDataProvider().get_data()
         survivors = await _MyFilter().apply(raw_data)
         to_bo4e_mapper = _MyToBo4eMapper(what_ever_you_like=survivors)
         strategy = MyMigrationStrategy(
             source_data_set_to_bo4e_mapper=to_bo4e_mapper,
             validation=_my_validation,
             bo4e_to_target_mapper=_MyToTargetMapper(),
             target_loader=_MyTargetLoader(),
```

### Comparing `bomf-0.3.1/unittests/test_source_data_provider.py` & `bomf-0.4.0/unittests/test_source_data_provider.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,53 +8,53 @@
 
 
 class LegacyDataSystemDataProvider(SourceDataProvider):
     """
     a dummy for access to a legacy system from which we want to migrate data
     """
 
-    def get_entry(self, key: KeyTyp) -> str:
+    async def get_entry(self, key: KeyTyp) -> str:
         raise NotImplementedError("Not relevant for this test")
 
-    def get_data(self) -> List[str]:
+    async def get_data(self) -> List[str]:
         return ["foo", "bar", "baz"]
 
 
 class TestSourceDataProvider:
-    def test_provider(self):
+    async def test_provider(self):
         # this is a pretty dumb test
         provider_under_test = LegacyDataSystemDataProvider()
-        assert isinstance(provider_under_test.get_data(), list)
+        assert isinstance(await provider_under_test.get_data(), list)
 
     @pytest.mark.datafiles("./unittests/example_source_data.json")
-    def test_json_file_provider(self, datafiles):
+    async def test_json_file_provider(self, datafiles):
         file_path = datafiles / Path("example_source_data.json")
         example_json_data_provider = JsonFileSourceDataProvider(
             file_path,
             data_selector=lambda d: d["data"],  # type:ignore[call-overload]
             key_selector=lambda d: d["myKey"],  # type:ignore[index]
         )
-        assert example_json_data_provider.get_data() == [
+        assert await example_json_data_provider.get_data() == [
             {"myKey": "hello", "asd": "fgh"},
             {"myKey": "world", "qwe": "rtz"},
         ]
-        assert example_json_data_provider.get_entry("world") == {"myKey": "world", "qwe": "rtz"}
+        assert await example_json_data_provider.get_entry("world") == {"myKey": "world", "qwe": "rtz"}
         with pytest.raises(KeyError):
-            _ = example_json_data_provider.get_entry("something unknown")
+            _ = await example_json_data_provider.get_entry("something unknown")
 
 
 class TestListBasedSourceDataProvider:
-    def test_list_based_provider(self, caplog):
+    async def test_list_based_provider(self, caplog):
         caplog.set_level(logging.DEBUG, logger=ListBasedSourceDataProvider.__module__)
         my_provider = ListBasedSourceDataProvider(["foo", "bar", "baz"], key_selector=lambda x: x)
-        assert len(my_provider.get_data()) == 3
-        assert my_provider.get_entry("bar") == "bar"
+        assert len(await my_provider.get_data()) == 3
+        assert await my_provider.get_entry("bar") == "bar"
         assert "Read 3 records from ['foo', 'bar', 'baz']" in caplog.messages
 
-    def test_list_based_provider_key_warning(self, caplog):
+    async def test_list_based_provider_key_warning(self, caplog):
         caplog.set_level(logging.WARNING, logger=ListBasedSourceDataProvider.__module__)
         my_provider = ListBasedSourceDataProvider(["fooy", "fooz" "bar", "baz"], key_selector=lambda x: x[0:3])
-        assert len(my_provider.get_data()) == 3
+        assert len(await my_provider.get_data()) == 3
         assert (
             "There are 2>1 entries for the key 'foo'. You might miss entries because the key is not unique."
             in caplog.messages
         )
```

### Comparing `bomf-0.3.1/unittests/test_validation.py` & `bomf-0.4.0/unittests/test_validation.py`

 * *Files identical despite different names*

