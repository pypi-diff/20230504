# Comparing `tmp/pyfields-1.7.0.tar.gz` & `tmp/pyfields-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyfields-1.7.0.tar", last modified: Mon Jun 21 09:33:09 2021, max compression
+gzip compressed data, was "dist/pyfields-1.7.1.tar", last modified: Thu May  4 13:11:13 2023, max compression
```

## Comparing `pyfields-1.7.0.tar` & `pyfields-1.7.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-21 09:33:09.000000 pyfields-1.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-21 09:33:09.000000 pyfields-1.7.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-21 09:33:09.000000 pyfields-1.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     5585 2021-06-21 09:32:33.000000 pyfields-1.7.0/.github/workflows/base.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1941 2021-06-21 09:32:33.000000 pyfields-1.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1514 2021-06-21 09:32:33.000000 pyfields-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2670 2021-06-21 09:33:09.000000 pyfields-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5915 2021-06-21 09:32:33.000000 pyfields-1.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-21 09:33:09.000000 pyfields-1.7.0/ci_tools/
--rw-r--r--   0 runner    (1001) docker     (121)    17412 2021-06-21 09:32:33.000000 pyfields-1.7.0/ci_tools/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)     1274 2021-06-21 09:32:33.000000 pyfields-1.7.0/ci_tools/check_python_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     3708 2021-06-21 09:32:33.000000 pyfields-1.7.0/ci_tools/generate-junit-badge.py
--rw-r--r--   0 runner    (1001) docker     (121)     5749 2021-06-21 09:32:33.000000 pyfields-1.7.0/ci_tools/github_release.py
--rw-r--r--   0 runner    (1001) docker     (121)    29073 2021-06-21 09:32:33.000000 pyfields-1.7.0/ci_tools/nox_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-21 09:33:09.000000 pyfields-1.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)    29535 2021-06-21 09:32:33.000000 pyfields-1.7.0/docs/api_reference.md
--rw-r--r--   0 runner    (1001) docker     (121)    14294 2021-06-21 09:32:33.000000 pyfields-1.7.0/docs/changelog.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-21 09:33:09.000000 pyfields-1.7.0/docs/imgs/
--rw-r--r--   0 runner    (1001) docker     (121)     2329 2021-06-21 09:32:33.000000 pyfields-1.7.0/docs/imgs/autocomplete1.png
--rw-r--r--   0 runner    (1001) docker     (121)    35396 2021-06-21 09:32:33.000000 pyfields-1.7.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (121)     1443 2021-06-21 09:32:33.000000 pyfields-1.7.0/docs/long_description.md
--rw-r--r--   0 runner    (1001) docker     (121)      708 2021-06-21 09:32:33.000000 pyfields-1.7.0/docs/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     5114 2021-06-21 09:32:33.000000 pyfields-1.7.0/docs/why.md
--rw-r--r--   0 runner    (1001) docker     (121)       89 2021-06-21 09:32:33.000000 pyfields-1.7.0/noxfile-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)    12623 2021-06-21 09:32:33.000000 pyfields-1.7.0/noxfile.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-21 09:33:09.000000 pyfields-1.7.0/pyfields/
--rw-r--r--   0 runner    (1001) docker     (121)     1505 2021-06-21 09:32:33.000000 pyfields-1.7.0/pyfields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      142 2021-06-21 09:33:09.000000 pyfields-1.7.0/pyfields/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    27523 2021-06-21 09:32:33.000000 pyfields-1.7.0/pyfields/autofields_.py
--rw-r--r--   0 runner    (1001) docker     (121)    50040 2021-06-21 09:32:33.000000 pyfields-1.7.0/pyfields/core.py
--rw-r--r--   0 runner    (1001) docker     (121)    13008 2021-06-21 09:32:33.000000 pyfields-1.7.0/pyfields/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)    25393 2021-06-21 09:32:33.000000 pyfields-1.7.0/pyfields/init_makers.py
--rw-r--r--   0 runner    (1001) docker     (121)      899 2021-06-21 09:32:33.000000 pyfields-1.7.0/pyfields/init_makers.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-21 09:32:33.000000 pyfields-1.7.0/pyfields/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-21 09:33:09.000000 pyfields-1.7.0/pyfields/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      126 2021-06-21 09:32:33.000000 pyfields-1.7.0/pyfields/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2848 2021-06-21 09:32:33.000000 pyfields-1.7.0/pyfields/tests/_test_benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (121)     5906 2021-06-21 09:32:33.000000 pyfields-1.7.0/pyfields/tests/_test_py36.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-21 09:33:09.000000 pyfields-1.7.0/pyfields/tests/issues/
--rw-r--r--   0 runner    (1001) docker     (121)      126 2021-06-21 09:32:33.000000 pyfields-1.7.0/pyfields/tests/issues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1231 2021-06-21 09:32:33.000000 pyfields-1.7.0/pyfields/tests/issues/_test_py36.py
--rw-r--r--   0 runner    (1001) docker     (121)      590 2021-06-21 09:32:33.000000 pyfields-1.7.0/pyfields/tests/issues/_test_py36_pep563.py
--rw-r--r--   0 runner    (1001) docker     (121)      447 2021-06-21 09:32:33.000000 pyfields-1.7.0/pyfields/tests/issues/test_issue_12.py
--rw-r--r--   0 runner    (1001) docker     (121)      357 2021-06-21 09:32:33.000000 pyfields-1.7.0/pyfields/tests/issues/test_issue_51.py
--rw-r--r--   0 runner    (1001) docker     (121)      572 2021-06-21 09:32:33.000000 pyfields-1.7.0/pyfields/tests/issues/test_issue_53.py
--rw-r--r--   0 runner    (1001) docker     (121)      431 2021-06-21 09:32:33.000000 pyfields-1.7.0/pyfields/tests/issues/test_issue_67.py
--rw-r--r--   0 runner    (1001) docker     (121)     2988 2021-06-21 09:32:33.000000 pyfields-1.7.0/pyfields/tests/issues/test_issue_73.py
--rw-r--r--   0 runner    (1001) docker     (121)      786 2021-06-21 09:32:33.000000 pyfields-1.7.0/pyfields/tests/issues/test_issue_81.py
--rw-r--r--   0 runner    (1001) docker     (121)     2457 2021-06-21 09:32:33.000000 pyfields-1.7.0/pyfields/tests/issues/test_issue_84.py
--rw-r--r--   0 runner    (1001) docker     (121)     5055 2021-06-21 09:32:33.000000 pyfields-1.7.0/pyfields/tests/test_autofields.py
--rw-r--r--   0 runner    (1001) docker     (121)    26506 2021-06-21 09:32:33.000000 pyfields-1.7.0/pyfields/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (121)     1460 2021-06-21 09:32:33.000000 pyfields-1.7.0/pyfields/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     7878 2021-06-21 09:32:33.000000 pyfields-1.7.0/pyfields/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (121)    16554 2021-06-21 09:32:33.000000 pyfields-1.7.0/pyfields/tests/test_readme.py
--rw-r--r--   0 runner    (1001) docker     (121)     7606 2021-06-21 09:32:33.000000 pyfields-1.7.0/pyfields/tests/test_so.py
--rw-r--r--   0 runner    (1001) docker     (121)     6631 2021-06-21 09:32:33.000000 pyfields-1.7.0/pyfields/typing_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    27046 2021-06-21 09:32:33.000000 pyfields-1.7.0/pyfields/validate_n_convert.py
--rw-r--r--   0 runner    (1001) docker     (121)     6112 2021-06-21 09:32:33.000000 pyfields-1.7.0/pyfields/validate_n_convert.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-21 09:33:09.000000 pyfields-1.7.0/pyfields.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2670 2021-06-21 09:33:09.000000 pyfields-1.7.0/pyfields.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1496 2021-06-21 09:33:09.000000 pyfields-1.7.0/pyfields.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-21 09:33:09.000000 pyfields-1.7.0/pyfields.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-21 09:33:09.000000 pyfields-1.7.0/pyfields.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       90 2021-06-21 09:33:09.000000 pyfields-1.7.0/pyfields.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2021-06-21 09:33:09.000000 pyfields-1.7.0/pyfields.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      581 2021-06-21 09:32:33.000000 pyfields-1.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1842 2021-06-21 09:33:09.000000 pyfields-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1445 2021-06-21 09:32:33.000000 pyfields-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:11:13.000000 pyfields-1.7.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:11:13.000000 pyfields-1.7.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:11:13.000000 pyfields-1.7.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-05-04 13:10:10.000000 pyfields-1.7.1/.github/workflows/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-04 13:10:10.000000 pyfields-1.7.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-04 13:10:10.000000 pyfields-1.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-05-04 13:11:13.000000 pyfields-1.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-05-04 13:10:10.000000 pyfields-1.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:11:13.000000 pyfields-1.7.1/ci_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)    17412 2023-05-04 13:10:10.000000 pyfields-1.7.1/ci_tools/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-04 13:10:10.000000 pyfields-1.7.1/ci_tools/check_python_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-04 13:10:10.000000 pyfields-1.7.1/ci_tools/flake8-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-05-04 13:10:10.000000 pyfields-1.7.1/ci_tools/github_release.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29235 2023-05-04 13:10:10.000000 pyfields-1.7.1/ci_tools/nox_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:11:13.000000 pyfields-1.7.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    29535 2023-05-04 13:10:10.000000 pyfields-1.7.1/docs/api_reference.md
+-rw-r--r--   0 runner    (1001) docker     (123)    14569 2023-05-04 13:10:10.000000 pyfields-1.7.1/docs/changelog.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:11:13.000000 pyfields-1.7.1/docs/imgs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-05-04 13:10:10.000000 pyfields-1.7.1/docs/imgs/autocomplete1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    35598 2023-05-04 13:10:10.000000 pyfields-1.7.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-04 13:10:10.000000 pyfields-1.7.1/docs/long_description.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-05-04 13:10:10.000000 pyfields-1.7.1/docs/why.md
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-04 13:10:10.000000 pyfields-1.7.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-04 13:10:10.000000 pyfields-1.7.1/noxfile-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14464 2023-05-04 13:10:10.000000 pyfields-1.7.1/noxfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:11:13.000000 pyfields-1.7.1/pyfields/
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-04 13:10:10.000000 pyfields-1.7.1/pyfields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-04 13:11:13.000000 pyfields-1.7.1/pyfields/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27526 2023-05-04 13:10:10.000000 pyfields-1.7.1/pyfields/autofields_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50067 2023-05-04 13:10:10.000000 pyfields-1.7.1/pyfields/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13099 2023-05-04 13:10:10.000000 pyfields-1.7.1/pyfields/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25424 2023-05-04 13:10:10.000000 pyfields-1.7.1/pyfields/init_makers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-04 13:10:10.000000 pyfields-1.7.1/pyfields/init_makers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:10:10.000000 pyfields-1.7.1/pyfields/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:11:13.000000 pyfields-1.7.1/pyfields/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-04 13:10:10.000000 pyfields-1.7.1/pyfields/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-04 13:10:10.000000 pyfields-1.7.1/pyfields/tests/_test_benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-05-04 13:10:10.000000 pyfields-1.7.1/pyfields/tests/_test_py36.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:11:13.000000 pyfields-1.7.1/pyfields/tests/issues/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-04 13:10:10.000000 pyfields-1.7.1/pyfields/tests/issues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-04 13:10:10.000000 pyfields-1.7.1/pyfields/tests/issues/_test_py36.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-04 13:10:10.000000 pyfields-1.7.1/pyfields/tests/issues/_test_py36_pep563.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-04 13:10:10.000000 pyfields-1.7.1/pyfields/tests/issues/test_issue_12.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-04 13:10:10.000000 pyfields-1.7.1/pyfields/tests/issues/test_issue_51.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-04 13:10:10.000000 pyfields-1.7.1/pyfields/tests/issues/test_issue_53.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-04 13:10:10.000000 pyfields-1.7.1/pyfields/tests/issues/test_issue_67.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-05-04 13:10:10.000000 pyfields-1.7.1/pyfields/tests/issues/test_issue_73.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-04 13:10:10.000000 pyfields-1.7.1/pyfields/tests/issues/test_issue_81.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-04 13:10:10.000000 pyfields-1.7.1/pyfields/tests/issues/test_issue_84.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-05-04 13:10:10.000000 pyfields-1.7.1/pyfields/tests/test_autofields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26506 2023-05-04 13:10:10.000000 pyfields-1.7.1/pyfields/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-04 13:10:10.000000 pyfields-1.7.1/pyfields/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-05-04 13:10:10.000000 pyfields-1.7.1/pyfields/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16554 2023-05-04 13:10:10.000000 pyfields-1.7.1/pyfields/tests/test_readme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7606 2023-05-04 13:10:10.000000 pyfields-1.7.1/pyfields/tests/test_so.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-05-04 13:10:10.000000 pyfields-1.7.1/pyfields/typing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27164 2023-05-04 13:10:10.000000 pyfields-1.7.1/pyfields/validate_n_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-05-04 13:10:10.000000 pyfields-1.7.1/pyfields/validate_n_convert.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:11:13.000000 pyfields-1.7.1/pyfields.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-05-04 13:11:13.000000 pyfields-1.7.1/pyfields.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-04 13:11:13.000000 pyfields-1.7.1/pyfields.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 13:11:13.000000 pyfields-1.7.1/pyfields.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 13:11:13.000000 pyfields-1.7.1/pyfields.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-04 13:11:13.000000 pyfields-1.7.1/pyfields.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-04 13:11:13.000000 pyfields-1.7.1/pyfields.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-04 13:10:10.000000 pyfields-1.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-04 13:11:13.000000 pyfields-1.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-05-04 13:10:10.000000 pyfields-1.7.1/setup.py
```

### Comparing `pyfields-1.7.0/.github/workflows/base.yml` & `pyfields-1.7.1/.github/workflows/base.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 # .github/workflows/base.yml
 name: Build
 on:
+  # this one is to trigger the workflow manually from the interface
+  workflow_dispatch:
+
   push:
     tags:
       - '*'
     branches:
       - main
   pull_request:
     branches:
@@ -110,14 +113,18 @@
       # Nox install
       - name: Install noxfile requirements
         shell: bash -l {0}  # so that conda works
         run: pip install -r noxfile-requirements.txt
       - run: conda list
         shell: bash -l {0}  # so that conda works
 
+      # 5) Run the flake8 report and badge
+      - name: Run flake8 analysis and generate corresponding badge
+        shell: bash -l {0}  # so that conda works
+        run: nox -s flake8
 
       # -------------- only on Ubuntu + MAIN PUSH (no pull request, no tag) -----------
 
       # 5) Publish the doc and test reports
       - name: \[not on TAG\] Publish documentation, tests and coverage reports
         if: github.event_name == 'push' && startsWith(github.ref, 'refs/heads')  # startsWith(matrix.os,'ubuntu')
         shell: bash -l {0}  # so that conda works
```

### Comparing `pyfields-1.7.0/.gitignore` & `pyfields-1.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pyfields-1.7.0/LICENSE` & `pyfields-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfields-1.7.0/PKG-INFO` & `pyfields-1.7.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 Metadata-Version: 2.1
 Name: pyfields
-Version: 1.7.0
+Version: 1.7.1
 Summary: Define fields in python classes. Easily.
 Home-page: https://github.com/smarie/python-pyfields
+Download-URL: https://github.com/smarie/python-pyfields/tarball/1.7.1
 Author: Sylvain MARIE <sylvain.marie@se.com>
 Maintainer: Sylvain MARIE <sylvain.marie@se.com>
 License: BSD 3-Clause
-Download-URL: https://github.com/smarie/python-pyfields/tarball/1.7.0
-Description: # python-pyfields
-        
-        *Define fields in python classes. Easily.*
-        
-        [![Python versions](https://img.shields.io/pypi/pyversions/pyfields.svg)](https://pypi.python.org/pypi/pyfields/) [![Build Status](https://github.com/smarie/python-pyfields/actions/workflows/base.yml/badge.svg)](https://github.com/smarie/python-pyfields/actions/workflows/base.yml) [![Tests Status](https://smarie.github.io/python-pyfields/reports/junit/junit-badge.svg?dummy=8484744)](https://smarie.github.io/python-pyfields/reports/junit/report.html) [![codecov](https://codecov.io/gh/smarie/python-pyfields/branch/main/graph/badge.svg)](https://codecov.io/gh/smarie/python-pyfields)
-        
-        [![Documentation](https://img.shields.io/badge/doc-latest-blue.svg)](https://smarie.github.io/python-pyfields/) [![PyPI](https://img.shields.io/pypi/v/pyfields.svg)](https://pypi.python.org/pypi/pyfields/) [![Downloads](https://pepy.tech/badge/pyfields)](https://pepy.tech/project/pyfields) [![Downloads per week](https://pepy.tech/badge/pyfields/week)](https://pepy.tech/project/pyfields) [![GitHub stars](https://img.shields.io/github/stars/smarie/python-pyfields.svg)](https://github.com/smarie/python-pyfields/stargazers)
-        
-        The documentation for users is available here: [https://smarie.github.io/python-pyfields/](https://smarie.github.io/python-pyfields/)
-        
-        A readme for developers is available here: [https://github.com/smarie/python-pyfields](https://github.com/smarie/python-pyfields)
-        
 Keywords: object class boilerplate oop field attr member descriptor attribute mix-in mixin validation type-check
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# python-pyfields
+
+*Define fields in python classes. Easily.*
+
+[![Python versions](https://img.shields.io/pypi/pyversions/pyfields.svg)](https://pypi.python.org/pypi/pyfields/) [![Build Status](https://github.com/smarie/python-pyfields/actions/workflows/base.yml/badge.svg)](https://github.com/smarie/python-pyfields/actions/workflows/base.yml) [![Tests Status](https://smarie.github.io/python-pyfields/reports/junit/junit-badge.svg?dummy=8484744)](https://smarie.github.io/python-pyfields/reports/junit/report.html) [![Coverage Status](https://smarie.github.io/python-pyfields/reports/coverage/coverage-badge.svg?dummy=8484744)](https://smarie.github.io/python-pyfields/reports/coverage/index.html) [![codecov](https://codecov.io/gh/smarie/python-pyfields/branch/main/graph/badge.svg)](https://codecov.io/gh/smarie/python-pyfields) [![Flake8 Status](https://smarie.github.io/python-pyfields/reports/flake8/flake8-badge.svg?dummy=8484744)](https://smarie.github.io/python-pyfields/reports/flake8/index.html)
+
+[![Documentation](https://img.shields.io/badge/doc-latest-blue.svg)](https://smarie.github.io/python-pyfields/) [![PyPI](https://img.shields.io/pypi/v/pyfields.svg)](https://pypi.python.org/pypi/pyfields/) [![Downloads](https://pepy.tech/badge/pyfields)](https://pepy.tech/project/pyfields) [![Downloads per week](https://pepy.tech/badge/pyfields/week)](https://pepy.tech/project/pyfields) [![GitHub stars](https://img.shields.io/github/stars/smarie/python-pyfields.svg)](https://github.com/smarie/python-pyfields/stargazers)
+
+The documentation for users is available here: [https://smarie.github.io/python-pyfields/](https://smarie.github.io/python-pyfields/)
+
+A readme for developers is available here: [https://github.com/smarie/python-pyfields](https://github.com/smarie/python-pyfields)
```

### Comparing `pyfields-1.7.0/README.md` & `pyfields-1.7.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # python-pyfields
 
 *Define fields in python classes. Easily.*
 
-[![Python versions](https://img.shields.io/pypi/pyversions/pyfields.svg)](https://pypi.python.org/pypi/pyfields/) [![Build Status](https://github.com/smarie/python-pyfields/actions/workflows/base.yml/badge.svg)](https://github.com/smarie/python-pyfields/actions/workflows/base.yml) [![Tests Status](https://smarie.github.io/python-pyfields/reports/junit/junit-badge.svg?dummy=8484744)](https://smarie.github.io/python-pyfields/reports/junit/report.html) [![codecov](https://codecov.io/gh/smarie/python-pyfields/branch/main/graph/badge.svg)](https://codecov.io/gh/smarie/python-pyfields)
+[![Python versions](https://img.shields.io/pypi/pyversions/pyfields.svg)](https://pypi.python.org/pypi/pyfields/) [![Build Status](https://github.com/smarie/python-pyfields/actions/workflows/base.yml/badge.svg)](https://github.com/smarie/python-pyfields/actions/workflows/base.yml) [![Tests Status](https://smarie.github.io/python-pyfields/reports/junit/junit-badge.svg?dummy=8484744)](https://smarie.github.io/python-pyfields/reports/junit/report.html) [![Coverage Status](https://smarie.github.io/python-pyfields/reports/coverage/coverage-badge.svg?dummy=8484744)](https://smarie.github.io/python-pyfields/reports/coverage/index.html) [![codecov](https://codecov.io/gh/smarie/python-pyfields/branch/main/graph/badge.svg)](https://codecov.io/gh/smarie/python-pyfields) [![Flake8 Status](https://smarie.github.io/python-pyfields/reports/flake8/flake8-badge.svg?dummy=8484744)](https://smarie.github.io/python-pyfields/reports/flake8/index.html)
 
 [![Documentation](https://img.shields.io/badge/doc-latest-blue.svg)](https://smarie.github.io/python-pyfields/) [![PyPI](https://img.shields.io/pypi/v/pyfields.svg)](https://pypi.python.org/pypi/pyfields/) [![Downloads](https://pepy.tech/badge/pyfields)](https://pepy.tech/project/pyfields) [![Downloads per week](https://pepy.tech/badge/pyfields/week)](https://pepy.tech/project/pyfields) [![GitHub stars](https://img.shields.io/github/stars/smarie/python-pyfields.svg)](https://github.com/smarie/python-pyfields/stargazers)
 
 **This is the readme for developers.** The documentation for users is available here: [https://smarie.github.io/python-pyfields/](https://smarie.github.io/python-pyfields/)
 
 ## Want to contribute ?
```

### Comparing `pyfields-1.7.0/ci_tools/.pylintrc` & `pyfields-1.7.1/ci_tools/.pylintrc`

 * *Files identical despite different names*

### Comparing `pyfields-1.7.0/ci_tools/check_python_version.py` & `pyfields-1.7.1/ci_tools/check_python_version.py`

 * *Files identical despite different names*

### Comparing `pyfields-1.7.0/ci_tools/github_release.py` & `pyfields-1.7.1/ci_tools/github_release.py`

 * *Files identical despite different names*

### Comparing `pyfields-1.7.0/ci_tools/nox_utils.py` & `pyfields-1.7.1/ci_tools/nox_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import nox
 from nox.sessions import Session
 
 
 nox_logger = logging.getLogger("nox")
 
 
-PY27, PY35, PY36, PY37, PY38 = "2.7", "3.5", "3.6", "3.7", "3.8"
+PY27, PY35, PY36, PY37, PY38, PY39, PY310 = "2.7", "3.5", "3.6", "3.7", "3.8", "3.9", "3.10"
 DONT_INSTALL = "dont_install"
 
 
 def power_session(
         func=None,
         envs=None,
         grid_param_name="env",
@@ -145,26 +145,28 @@
 
     def install_reqs(
             self,
             # pre wired phases
             setup=False,
             install=False,
             tests=False,
+            extras=(),
             # custom phase
             phase=None,
             phase_reqs=None,
             versions_dct=None
     ):
         """
         A high-level helper to install requirements from the various project files
 
          - pyproject.toml "[build-system] requires" (if setup=True)
          - setup.cfg "[options] setup_requires" (if setup=True)
          - setup.cfg "[options] install_requires" (if install=True)
          - setup.cfg "[options] test_requires" (if tests=True)
+         - setup.cfg "[options.extras_require] <...>" (if extras=(a tuple of extras))
 
         Two additional mechanisms are provided in order to customize how packages are installed.
 
         Conda packages
         --------------
         If the session runs on a conda environment, you can add a [tool.conda] section to your pyproject.toml. This
         section should contain a `conda_packages` entry containing the list of package names that should be installed
@@ -204,14 +206,18 @@
         if install:
             self.install_any("setup.cfg#install_requires", setup_cfg.install_requires,
                              use_conda_for=toml_use_conda_for, versions_dct=versions_dct)
         if tests:
             self.install_any("setup.cfg#tests_requires", setup_cfg.tests_requires,
                              use_conda_for=toml_use_conda_for, versions_dct=versions_dct)
 
+        for extra in extras:
+            self.install_any("setup.cfg#extras_require#%s" % extra, setup_cfg.extras_require[extra],
+                             use_conda_for=toml_use_conda_for, versions_dct=versions_dct)
+
         if phase is not None:
             self.install_any(phase, phase_reqs, use_conda_for=toml_use_conda_for, versions_dct=versions_dct)
 
     def install_any(self,
                     phase_name: str,
                     pkgs: Sequence[str],
                     use_conda_for: Sequence[str] = (),
@@ -317,35 +323,29 @@
         requires = pyproject['build-system']['requires']
         conda_pkgs = pyproject['tool']['conda']['conda_packages']
         return requires, conda_pkgs
     else:
         raise FileNotFoundError("No `pyproject.toml` file exists. No dependency will be installed ...")
 
 
-SetupCfg = namedtuple('SetupCfg', ('setup_requires', 'install_requires', 'tests_requires'))
+SetupCfg = namedtuple('SetupCfg', ('setup_requires', 'install_requires', 'tests_requires', 'extras_require'))
 
 
 def read_setuptools_cfg():
     """
     Reads the `setup.cfg` file and extracts the various requirements lists
     """
     # see https://stackoverflow.com/a/30679041/7262247
     from setuptools import Distribution
     dist = Distribution()
     dist.parse_config_files()
-
-    # standard requirements
-    options_dct = dist.get_option_dict('options')
-    setup_reqs = options_dct['setup_requires'][1].strip().splitlines()
-    install_reqs = options_dct['install_requires'][1].strip().splitlines()
-    tests_reqs = options_dct['tests_require'][1].strip().splitlines()
-
-    return SetupCfg(setup_requires=setup_reqs,
-                    install_requires=install_reqs,
-                    tests_requires=tests_reqs)
+    return SetupCfg(setup_requires=dist.setup_requires,
+                    install_requires=dist.install_requires,
+                    tests_requires=dist.tests_require,
+                    extras_require=dist.extras_require)
 
 
 def get_req_pkg_name(r):
     """Return the package name part of a python package requirement.
 
     For example
     "funcsigs;python<'3.5'" will return "funcsigs"
```

### Comparing `pyfields-1.7.0/docs/api_reference.md` & `pyfields-1.7.1/docs/api_reference.md`

 * *Files identical despite different names*

### Comparing `pyfields-1.7.0/docs/changelog.md` & `pyfields-1.7.1/docs/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Changelog
 
+### 1.7.1 - Compatibility fix for typeguard `3.0.0`
+
+ - Fixed `TypeError: check_type() takes 2 positional arguments but 3 were given` triggering erroneous `FieldTypeError` 
+   when `typeguard>=3.0.0` is used. Fixed [#87](https://github.com/smarie/python-pyfields/issues/87)
+
 ### 1.7.0 - Better support for non-deep-copiable default values in `@autofields`
 
  - `@autofields` and `@autoclass` now raise an error when a field definition can not be valid, because the default value can not be deep-copied. This will help users detect issues such as [#84](https://github.com/smarie/python-pyfields/issues/84) earlier. Implementation is done through a new `autocheck` option in the `copy_value` factory.
 
  - `@autofields` and `@autoclass` now provide an `exclude` (resp. `af_exclude`) list, to list names for fields that should not be created. By default this contains a reserved name from `abc.ABCMeta`, for convenience. Fixes [#84](https://github.com/smarie/python-pyfields/issues/84).
```

### Comparing `pyfields-1.7.0/docs/imgs/autocomplete1.png` & `pyfields-1.7.1/docs/imgs/autocomplete1.png`

 * *Files identical despite different names*

### Comparing `pyfields-1.7.0/docs/index.md` & `pyfields-1.7.1/docs/index.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # pyfields
 
 *Define fields in python classes. Easily.*
 
-[![Python versions](https://img.shields.io/pypi/pyversions/pyfields.svg)](https://pypi.python.org/pypi/pyfields/) [![Build Status](https://github.com/smarie/python-pyfields/actions/workflows/base.yml/badge.svg)](https://github.com/smarie/python-pyfields/actions/workflows/base.yml) [![Tests Status](./reports/junit/junit-badge.svg?dummy=8484744)](./reports/junit/report.html) [![codecov](https://codecov.io/gh/smarie/python-pyfields/branch/main/graph/badge.svg)](https://codecov.io/gh/smarie/python-pyfields)
+[![Python versions](https://img.shields.io/pypi/pyversions/pyfields.svg)](https://pypi.python.org/pypi/pyfields/) [![Build Status](https://github.com/smarie/python-pyfields/actions/workflows/base.yml/badge.svg)](https://github.com/smarie/python-pyfields/actions/workflows/base.yml) [![Tests Status](./reports/junit/junit-badge.svg?dummy=8484744)](./reports/junit/report.html) [![Coverage Status](./reports/coverage/coverage-badge.svg?dummy=8484744)](./reports/coverage/index.html) [![codecov](https://codecov.io/gh/smarie/python-pyfields/branch/main/graph/badge.svg)](https://codecov.io/gh/smarie/python-pyfields) [![Flake8 Status](./reports/flake8/flake8-badge.svg?dummy=8484744)](./reports/flake8/index.html)
 
 [![Documentation](https://img.shields.io/badge/doc-latest-blue.svg)](https://smarie.github.io/python-pyfields/) [![PyPI](https://img.shields.io/pypi/v/pyfields.svg)](https://pypi.python.org/pypi/pyfields/) [![Downloads](https://pepy.tech/badge/pyfields)](https://pepy.tech/project/pyfields) [![Downloads per week](https://pepy.tech/badge/pyfields/week)](https://pepy.tech/project/pyfields) [![GitHub stars](https://img.shields.io/github/stars/smarie/python-pyfields.svg)](https://github.com/smarie/python-pyfields/stargazers)
 
 !!! success "`pyfields` now has its own [`@autoclass`](#b-autoclass) with sensible defaults, to complement the existing [`@autofields`](#a-autofields) feature! No need to import it from `autoclass` anymore."
 
 !!! success "New [`marshmallow-pyfields`](https://smarie.github.io/python-marshmallow-pyfields/) project brings `pyfields` to the famous [`marshmallow`](https://marshmallow.readthedocs.io/en/stable/) ORM ecosystem!"
```

### Comparing `pyfields-1.7.0/docs/long_description.md` & `pyfields-1.7.1/docs/long_description.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # python-pyfields
 
 *Define fields in python classes. Easily.*
 
-[![Python versions](https://img.shields.io/pypi/pyversions/pyfields.svg)](https://pypi.python.org/pypi/pyfields/) [![Build Status](https://github.com/smarie/python-pyfields/actions/workflows/base.yml/badge.svg)](https://github.com/smarie/python-pyfields/actions/workflows/base.yml) [![Tests Status](https://smarie.github.io/python-pyfields/reports/junit/junit-badge.svg?dummy=8484744)](https://smarie.github.io/python-pyfields/reports/junit/report.html) [![codecov](https://codecov.io/gh/smarie/python-pyfields/branch/main/graph/badge.svg)](https://codecov.io/gh/smarie/python-pyfields)
+[![Python versions](https://img.shields.io/pypi/pyversions/pyfields.svg)](https://pypi.python.org/pypi/pyfields/) [![Build Status](https://github.com/smarie/python-pyfields/actions/workflows/base.yml/badge.svg)](https://github.com/smarie/python-pyfields/actions/workflows/base.yml) [![Tests Status](https://smarie.github.io/python-pyfields/reports/junit/junit-badge.svg?dummy=8484744)](https://smarie.github.io/python-pyfields/reports/junit/report.html) [![Coverage Status](https://smarie.github.io/python-pyfields/reports/coverage/coverage-badge.svg?dummy=8484744)](https://smarie.github.io/python-pyfields/reports/coverage/index.html) [![codecov](https://codecov.io/gh/smarie/python-pyfields/branch/main/graph/badge.svg)](https://codecov.io/gh/smarie/python-pyfields) [![Flake8 Status](https://smarie.github.io/python-pyfields/reports/flake8/flake8-badge.svg?dummy=8484744)](https://smarie.github.io/python-pyfields/reports/flake8/index.html)
 
 [![Documentation](https://img.shields.io/badge/doc-latest-blue.svg)](https://smarie.github.io/python-pyfields/) [![PyPI](https://img.shields.io/pypi/v/pyfields.svg)](https://pypi.python.org/pypi/pyfields/) [![Downloads](https://pepy.tech/badge/pyfields)](https://pepy.tech/project/pyfields) [![Downloads per week](https://pepy.tech/badge/pyfields/week)](https://pepy.tech/project/pyfields) [![GitHub stars](https://img.shields.io/github/stars/smarie/python-pyfields.svg)](https://github.com/smarie/python-pyfields/stargazers)
 
 The documentation for users is available here: [https://smarie.github.io/python-pyfields/](https://smarie.github.io/python-pyfields/)
 
 A readme for developers is available here: [https://github.com/smarie/python-pyfields](https://github.com/smarie/python-pyfields)
```

### Comparing `pyfields-1.7.0/docs/mkdocs.yml` & `pyfields-1.7.1/mkdocs.yml`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 site_name: pyfields
 # site_description: 'A short description of my project'
 repo_url: https://github.com/smarie/python-pyfields
-docs_dir: .
-site_dir: ../site
+#docs_dir: .
+#site_dir: ../site
+# default branch is main instead of master now on github
+edit_uri : ./edit/main/docs
 nav:
     - Home: index.md
     - Why fields: why.md
     - API reference: api_reference.md
     - Changelog: changelog.md
 
 theme: material  # readthedocs  mkdocs
```

### Comparing `pyfields-1.7.0/docs/why.md` & `pyfields-1.7.1/docs/why.md`

 * *Files identical despite different names*

### Comparing `pyfields-1.7.0/noxfile.py` & `pyfields-1.7.1/noxfile.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 from itertools import product
 from json import dumps
-
 import logging
 
 import nox  # noqa
 from pathlib import Path  # noqa
 import sys
 
 # add parent folder to python path so that we can import noxfile_utils.py
 # note that you need to "pip install -r noxfile-requiterements.txt" for this file to work.
 sys.path.append(str(Path(__file__).parent / "ci_tools"))
-from nox_utils import PY27, PY37, PY36, PY35, PY38, power_session, rm_folder, rm_file, PowerSession  # noqa
+from nox_utils import PY27, PY37, PY36, PY35, PY38, PY39, PY310, power_session, rm_folder, rm_file, PowerSession  # noqa
 
 
 pkg_name = "pyfields"
 gh_org = "smarie"
 gh_repo = "python-pyfields"
 
 ENVS = {
-    # --- python 3.8 - first in list to catch obvious bugs on local executions
+    # --- python 3.9 - first in list to catch obvious bugs on local executions
+    (PY39, "no-typechecker"): {"coverage": False, "type_checker": None, "pkg_specs": {"pip": ">19"}},
+    # (PY38, "pytypes"): {"coverage": False, "type_checker": "pytypes", "pkg_specs": {"pip": ">19"}},
+    (PY39, "typeguard"): {"coverage": False, "type_checker": "typeguard", "pkg_specs": {"pip": ">19"}},
+    # --- python 3.8
     (PY38, "no-typechecker"): {"coverage": False, "type_checker": None, "pkg_specs": {"pip": ">19"}},
     # (PY38, "pytypes"): {"coverage": False, "type_checker": "pytypes", "pkg_specs": {"pip": ">19"}},
     (PY38, "typeguard"): {"coverage": False, "type_checker": "typeguard", "pkg_specs": {"pip": ">19"}},
     # --- python 2.7
     (PY27, "no-typechecker"): {"coverage": False, "type_checker": None, "pkg_specs": {"pip": ">19"}},
     (PY27, "pytypes"): {"coverage": False, "type_checker": "pytypes", "pkg_specs": {"pip": ">19"}},
     # --- python 3.5.3 > requires free channel > hard to make it work on GHA
@@ -40,48 +43,58 @@
     # --- python 3.7
     (PY37, "no-typechecker"): {"coverage": False, "type_checker": None, "pkg_specs": {"pip": ">19"}},
     #(PY37, "pytypes"): {"coverage": False, "type_checker": "pytypes", "pkg_specs": {"pip": ">19"}},
     # IMPORTANT: this should be last so that the folder docs/reports is not deleted afterwards
     (PY37, "typeguard"): {"coverage": True, "type_checker": "typeguard", "pkg_specs": {"pip": ">19"}}
 }
 
+
 # set the default activated sessions, minimal for CI
-nox.options.sessions = ["tests"]  # , "docs", "gh_pages"
+nox.options.sessions = ["tests", "flake8"]  # , "docs", "gh_pages"
 nox.options.reuse_existing_virtualenvs = True  # this can be done using -r
 # if platform.system() == "Windows":  >> always use this for better control
 nox.options.default_venv_backend = "conda"
 # os.environ["NO_COLOR"] = "True"  # nox.options.nocolor = True does not work
 # nox.options.verbose = True
 
 nox_logger = logging.getLogger("nox")
 # nox_logger.setLevel(logging.INFO)  NO !!!! this prevents the "verbose" nox flag to work !
 
 
 class Folders:
     root = Path(__file__).parent
+    ci_tools = root / "ci_tools"
     runlogs = root / Path(nox.options.envdir or ".nox") / "_runlogs"
     runlogs.mkdir(parents=True, exist_ok=True)
     dist = root / "dist"
     site = root / "site"
     site_reports = site / "reports"
     reports_root = root / "docs" / "reports"
     test_reports = reports_root / "junit"
+    test_xml = test_reports / "junit.xml"
+    test_html = test_reports / "report.html"
+    test_badge = test_reports / "junit-badge.svg"
     coverage_reports = reports_root / "coverage"
     coverage_xml = coverage_reports / "coverage.xml"
+    coverage_intermediate_file = root / ".coverage"
+    coverage_badge = coverage_reports / "coverage-badge.svg"
+    flake8_reports = reports_root / "flake8"
+    flake8_intermediate_file = root / "flake8stats.txt"
+    flake8_badge = flake8_reports / "flake8-badge.svg"
 
 
 @power_session(envs=ENVS, logsdir=Folders.runlogs)
 def tests(session: PowerSession, coverage, type_checker, pkg_specs):
     """Run the test suite, including test reports generation and coverage reports. """
 
     # As soon as this runs, we delete the target site and coverage files to avoid reporting wrong coverage/etc.
     rm_folder(Folders.site)
     rm_folder(Folders.reports_root)
     # delete the .coverage files if any (they are not supposed to be any, but just in case)
-    rm_file(Folders.root / ".coverage")
+    rm_file(Folders.coverage_intermediate_file)
     rm_file(Folders.root / "coverage.xml")
 
     # CI-only dependencies
     # Did we receive a flag through positional arguments ? (nox -s tests -- <flag>)
     # install_ci_deps = False
     # if len(session.posargs) == 1:
     #     assert session.posargs[0] == "keyrings.alt"
@@ -111,70 +124,95 @@
     session.run2("conda list", env={"CONDA_PREFIX": str(conda_prefix), "CONDA_DEFAULT_ENV": session.get_session_id()})
 
     # Fail if the assumed python version is not the actual one
     session.run2("python ci_tools/check_python_version.py %s" % session.python)
 
     # install self so that it is recognized by pytest
     session.run2("pip install -e . --no-deps")
+    # session.install("-e", ".", "--no-deps")
 
     # check that it can be imported even from a different folder
-    session.run2(['python', '-c', '"import os; os.chdir(\'./docs/\'); import %s"' % pkg_name])
+    # Important: do not surround the command into double quotes as in the shell !
+    session.run('python', '-c', 'import os; os.chdir(\'./docs/\'); import %s' % pkg_name)
 
     # finally run all tests
     if not coverage:
         # simple: pytest only
-        session.run2("python -m pytest -v %s/tests/" % pkg_name)
+        session.run2("python -m pytest --cache-clear -v %s/tests/" % pkg_name)
     else:
         # coverage + junit html reports + badge generation
-        session.install_reqs(phase="coverage", phase_reqs=["coverage", "pytest-html", "requests", "xunitparser"],
+        session.install_reqs(phase="coverage",
+                             phase_reqs=["coverage", "pytest-html", "genbadge[tests,coverage]"],
                              versions_dct=pkg_specs)
 
         # --coverage + junit html reports
         session.run2("coverage run --source {pkg_name} "
-                     "-m pytest --junitxml={dst}/junit.xml --html={dst}/report.html -v {pkg_name}/tests/"
-                     "".format(pkg_name=pkg_name, dst=Folders.test_reports))
-        # session.run2("coverage report")  # this shows in terminal + fails under XX%, same as --cov-report term --cov-fail-under=70  # noqa
+                     "-m pytest --cache-clear --junitxml={test_xml} --html={test_html} -v {pkg_name}/tests/"
+                     "".format(pkg_name=pkg_name, test_xml=Folders.test_xml, test_html=Folders.test_html))
+        session.run2("coverage report")
         session.run2("coverage xml -o {covxml}".format(covxml=Folders.coverage_xml))
         session.run2("coverage html -d {dst}".format(dst=Folders.coverage_reports))
         # delete this intermediate file, it is not needed anymore
-        rm_file(Folders.root / ".coverage")
+        rm_file(Folders.coverage_intermediate_file)
 
         # --generates the badge for the test results and fail build if less than x% tests pass
         nox_logger.info("Generating badge for tests coverage")
-        session.run2("python ci_tools/generate-junit-badge.py 100 %s" % Folders.test_reports)
+        # Use our own package to generate the badge
+        session.run2("genbadge tests -i %s -o %s -t 100" % (Folders.test_xml, Folders.test_badge))
+        session.run2("genbadge coverage -i %s -o %s" % (Folders.coverage_xml, Folders.coverage_badge))
+
+
+@power_session(python=PY38, logsdir=Folders.runlogs)
+def flake8(session: PowerSession):
+    """Launch flake8 qualimetry."""
+
+    session.install("-r", str(Folders.ci_tools / "flake8-requirements.txt"))
+    session.install("genbadge[flake8]")
+    session.run2("pip install -e .[flake8]")
+
+    rm_folder(Folders.flake8_reports)
+    Folders.flake8_reports.mkdir(parents=True, exist_ok=True)
+    rm_file(Folders.flake8_intermediate_file)
+
+    # Options are set in `setup.cfg` file
+    session.run("flake8", pkg_name, "--exit-zero", "--format=html", "--htmldir", str(Folders.flake8_reports),
+                "--statistics", "--tee", "--output-file", str(Folders.flake8_intermediate_file))
+    # generate our badge
+    session.run2("genbadge flake8 -i %s -o %s" % (Folders.flake8_intermediate_file, Folders.flake8_badge))
+    rm_file(Folders.flake8_intermediate_file)
 
 
 @power_session(python=[PY37])
 def docs(session: PowerSession):
     """Generates the doc and serves it on a local http server. Pass '-- build' to build statically instead."""
 
     session.install_reqs(phase="docs", phase_reqs=["mkdocs-material", "mkdocs", "pymdown-extensions", "pygments"])
 
     if session.posargs:
         # use posargs instead of "serve"
-        session.run2("mkdocs -f ./docs/mkdocs.yml %s" % " ".join(session.posargs))
+        session.run2("mkdocs %s" % " ".join(session.posargs))
     else:
-        session.run2("mkdocs serve -f ./docs/mkdocs.yml")
+        session.run2("mkdocs serve")
 
 
 @power_session(python=[PY37])
 def publish(session: PowerSession):
     """Deploy the docs+reports on github pages. Note: this rebuilds the docs"""
 
     session.install_reqs(phase="mkdocs", phase_reqs=["mkdocs-material", "mkdocs", "pymdown-extensions", "pygments"])
 
     # possibly rebuild the docs in a static way (mkdocs serve does not build locally)
-    session.run2("mkdocs build -f ./docs/mkdocs.yml")
+    session.run2("mkdocs build")
 
     # check that the doc has been generated with coverage
     if not Folders.site_reports.exists():
         raise ValueError("Test reports have not been built yet. Please run 'nox -s tests-3.7' first")
 
     # publish the docs
-    session.run2("mkdocs gh-deploy -f ./docs/mkdocs.yml")
+    session.run2("mkdocs gh-deploy")
 
     # publish the coverage - now in github actions only
     # session.install_reqs(phase="codecov", phase_reqs=["codecov", "keyring"])
     # # keyring set https://app.codecov.io/gh/<org>/<repo> token
     # import keyring  # (note that this import is not from the session env but the main nox env)
     # codecov_token = keyring.get_password("https://app.codecov.io/gh/<org>/<repo>>", "token")
     # # note: do not use --root nor -f ! otherwise "There was an error processing coverage reports"
@@ -228,15 +266,15 @@
         session.install_reqs(phase="PyPi", phase_reqs=["twine"])
         session.run2("twine upload dist/* -u smarie")  # -r testpypi
 
     # create the github release
     session.install_reqs(phase="release", phase_reqs=["click", "PyGithub"])
     session.run2("python ci_tools/github_release.py -s {gh_token} "
                  "--repo-slug {gh_org}/{gh_repo} -cf ./docs/changelog.md "
-                 "-d https://{gh_org}.github.io/{gh_repo}/changelog.html {tag}"
+                 "-d https://{gh_org}.github.io/{gh_repo}/changelog {tag}"
                  "".format(gh_token=gh_token, gh_org=gh_org, gh_repo=gh_repo, tag=current_tag))
 
 
 @nox.session(python=False)
 def gha_list(session):
     """(mandatory arg: <base_session_name>) Prints all sessions available for <base_session_name>, for GithubActions."""
```

### Comparing `pyfields-1.7.0/pyfields/__init__.py` & `pyfields-1.7.1/pyfields/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Authors: Sylvain MARIE <sylvain.marie@se.com>
+#          + All contributors to <https://github.com/smarie/python-pyfields>
+#
+# License: 3-clause BSD, <https://github.com/smarie/python-pyfields/blob/master/LICENSE>
 from .typing_utils import FieldTypeError
 from .core import field, Field, FieldError, MandatoryFieldInitError, UnsupportedOnNativeFieldError, \
     ReadOnlyFieldError, NoneError
 from .validate_n_convert import Converter, ConversionError, DetailedConversionResults, trace_convert
 from .init_makers import inject_fields, make_init, init_fields
 from .helpers import copy_value, copy_field, copy_attr, has_fields, get_fields, yield_fields, get_field, \
     get_field_values
```

### Comparing `pyfields-1.7.0/pyfields/autofields_.py` & `pyfields-1.7.1/pyfields/autofields_.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-#  Authors: Sylvain Marie <sylvain.marie@se.com>
+# Authors: Sylvain MARIE <sylvain.marie@se.com>
+#          + All contributors to <https://github.com/smarie/python-pyfields>
 #
-#  Copyright (c) Schneider Electric Industries, 2019. All right reserved.
+# License: 3-clause BSD, <https://github.com/smarie/python-pyfields/blob/master/LICENSE>
 import sys
 from copy import deepcopy
 from inspect import isdatadescriptor, ismethoddescriptor
 
 try:
     from typing import Union, Callable, Type, Any, TypeVar, Tuple, Iterable
     DecoratedClass = TypeVar("DecoratedClass", bound=Type[Any])
@@ -253,36 +254,36 @@
 
 
 _dict, _hash = dict, hash
 """Aliases for autoclass body"""
 
 
 def autoclass(
-        # --- autofields
-        fields=True,                  # type: Union[bool, DecoratedClass]
-        typecheck=False,              # type: bool
-        # --- constructor
-        init=True,                    # type: bool
-        # --- class methods
-        dict=True,                    # type: bool
-        dict_public_only=True,        # type: bool
-        repr=True,                    # type: bool
-        repr_curly_mode=False,        # type: bool
-        repr_public_only=True,        # type: bool
-        eq=True,                      # type: bool
-        eq_public_only=False,         # type: bool
-        hash=True,                    # type: bool
-        hash_public_only=False,       # type: bool
-        # --- advanced
-        af_include_upper=False,       # type: bool
-        af_include_dunder=False,      # type: bool
-        af_exclude=DEFAULT_EXCLUDED,  # type: Iterable[str]
-        ac_include=None,              # type: Union[str, Tuple[str]]
-        ac_exclude=None,              # type: Union[str, Tuple[str]]
-    ):
+    # --- autofields
+    fields=True,                  # type: Union[bool, DecoratedClass]
+    typecheck=False,              # type: bool
+    # --- constructor
+    init=True,                    # type: bool
+    # --- class methods
+    dict=True,                    # type: bool
+    dict_public_only=True,        # type: bool
+    repr=True,                    # type: bool
+    repr_curly_mode=False,        # type: bool
+    repr_public_only=True,        # type: bool
+    eq=True,                      # type: bool
+    eq_public_only=False,         # type: bool
+    hash=True,                    # type: bool
+    hash_public_only=False,       # type: bool
+    # --- advanced
+    af_include_upper=False,       # type: bool
+    af_include_dunder=False,      # type: bool
+    af_exclude=DEFAULT_EXCLUDED,  # type: Iterable[str]
+    ac_include=None,              # type: Union[str, Tuple[str]]
+    ac_exclude=None,              # type: Union[str, Tuple[str]]
+):
     """
     A decorator to automate many things at once for your class.
 
     First if `fields=True` (default) it executes `@autofields` to generate fields from attribute defined at class
     level.
 
      - you can include attributes with dunder names or uppercase names with `af_include_dunder` and
@@ -402,29 +403,30 @@
         if repr:
             repr_names = public_selected_names if repr_public_only else selected_names
             if not repr_curly_mode:  # default
 
                 def __repr__(self):
                     """ Generated by @pyfields.autoclass based on the class fields """
                     return '%s(%s)' % (self.__class__.__name__,
-                                       ', '.join('%s=%r' % (k, getattr(self, k))  for k in repr_names))
+                                       ', '.join('%s=%r' % (k, getattr(self, k)) for k in repr_names))
             else:
                 def __repr__(self):
                     """ Generated by @pyfields.autoclass based on the class fields """
                     return '%s(**{%s})' % (self.__class__.__name__,
                                            ', '.join('%r: %r' % (k, getattr(self, k)) for k in repr_names))
 
             if "__repr__" not in cls.__dict__:
                 cls.__repr__ = __repr__
             if "__str__" not in cls.__dict__:
                 cls.__str__ = __repr__
 
         # __eq__
         if eq:
             eq_names = public_selected_names if eq_public_only else selected_names
+
             def __eq__(self, other):
                 """ Generated by @pyfields.autoclass based on the class fields """
                 if isinstance(other, dict):
                     # comparison with dicts only when a to_dict method is available
                     try:
                         _self_to_dict = self.to_dict
                     except AttributeError:
@@ -527,16 +529,16 @@
 
 # def method_already_there(cls,
 #                          method_name,           # type: str
 #                          this_class_only=False  # type: bool
 #                          ):
 #     # type: (...) -> bool
 #     """
-#     Returns True if method `method_name` is already implemented by object_type, that is, its implementation differs from
-#     the one in `object`.
+#     Returns True if method `method_name` is already implemented by object_type, that is, its implementation differs
+#     from the one in `object`.
 #
 #     :param cls:
 #     :param method_name:
 #     :param this_class_only:
 #     :return:
 #     """
 #     if this_class_only:
```

### Comparing `pyfields-1.7.0/pyfields/core.py` & `pyfields-1.7.1/pyfields/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-#  Authors: Sylvain Marie <sylvain.marie@se.com>
+# Authors: Sylvain MARIE <sylvain.marie@se.com>
+#          + All contributors to <https://github.com/smarie/python-pyfields>
 #
-#  Copyright (c) Schneider Electric Industries, 2019. All right reserved.
-
+# License: 3-clause BSD, <https://github.com/smarie/python-pyfields/blob/master/LICENSE>
 import sys
 from enum import Enum
 from textwrap import dedent
 from inspect import getmro
 
 try:
     from inspect import signature, Parameter
 except ImportError:
     # noinspection PyUnresolvedReferences,PyPackageRequirements
-    from funcsigs import signature, Parameter
+    from funcsigs import signature, Parameter  # noqa
 
 from valid8 import ValidationFailure, is_pep484_nonable
 
 from pyfields.typing_utils import assert_is_of_type, FieldTypeError, get_type_hints
 from pyfields.validate_n_convert import FieldValidator, make_converters_list, trace_convert
 
 try:  # python 3.5+
     # noinspection PyUnresolvedReferences
-    from typing import List, Callable, Type, Any, Union, Iterable, Tuple, TypeVar
+    from typing import Callable, Type, Any, Union, Iterable, Tuple, TypeVar
     _NoneType = type(None)
     use_type_hints = sys.version_info > (3, 0)
     if use_type_hints:
         T = TypeVar('T')
         # noinspection PyUnresolvedReferences
         from pyfields.validate_n_convert import ValidatorDef, Validators, Converters, ConverterFuncDefinition,\
             DetailedConversionResults, ValidationFuncOrLambda, ValidType
@@ -704,26 +704,26 @@
 
     Inspired by
     -----------
     This method was inspired by
 
      - @lazy_attribute (sagemath)
      - @cached_property (werkzeug) and https://stackoverflow.com/questions/24704147/python-what-is-a-lazy-property
-     - https://stackoverflow.com/questions/42023852/how-can-i-get-the-attribute-name-when-working-with-descriptor-protocol-in-python
+     - https://stackoverflow.com/q/42023852/7262247
      - attrs / dataclasses
 
     :param type_hint: an optional explicit type hint for the field, to override the type hint defined by PEP484
         especially on old python versions because type comments can not be captured. Both a single type or an iterable
         of alternate types (e.g. `(int, str)`) are supported. By default the type hint is just a
         hint and does not contribute to validation. To enable type validation, set `check_type` to `True`.
     :param nonable: a boolean that can be used to explicitly declare that a field can contain `None`. When this is set
         to an explicit `True` or `False` value, usual type checking and validation (*if any*) are not anymore executed
         on `None` values. Instead ; if this is `True`, type checking and validation will be *deactivated* when the field
-        is set to `None` so as to always accept the value. If this is `False`, an `None`error will be raised when `None` is
-        set on the field.
+        is set to `None` so as to always accept the value. If this is `False`, an `None`error will be raised when `None`
+        is set on the field.
         When this is left as `GUESS` (default), the behaviour is "automatic". This means that
          - if the field (a) is optional with default value `None` or (b) has type hint `typing.Optional[]`, the
            behaviour will be the same as with `nonable=True`.
          - otherwise, the value will be the same as `nonable=UNKNOWN` and no special behaviour is put in place. `None`
            values will be treated as any other value. This can be particularly handy if a field accepts `None` ONLY IF
            another field is set to a special value. This can be done in a custom validator.
     :param check_type: by default (`check_type=False`), the type of a field, provided using PEP484 type hints or
@@ -1078,23 +1078,23 @@
         if self.converters is not None:
             # this is an inlined version of `trace_convert` with no capture of details
             for converter in self.converters:
                 # noinspection PyBroadException
                 try:
                     # does the converter accept this input ?
                     accepted = converter.accepts(obj, self, value)
-                except Exception:
+                except Exception:  # noqa
                     # ignore all exceptions from converters
                     continue
                 else:
                     if accepted is None or accepted:
                         # if so, let's try to convert
                         try:
                             converted_value = converter.convert(obj, self, value)
-                        except Exception:
+                        except Exception:  # noqa
                             # ignore all exceptions from converters
                             continue
                         else:
                             # successful conversion: use the converted value
                             value = converted_value
                             break
                     else:
```

### Comparing `pyfields-1.7.0/pyfields/helpers.py` & `pyfields-1.7.1/pyfields/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-#  Authors: Sylvain Marie <sylvain.marie@se.com>
+# Authors: Sylvain MARIE <sylvain.marie@se.com>
+#          + All contributors to <https://github.com/smarie/python-pyfields>
 #
-#  Copyright (c) Schneider Electric Industries, 2019. All right reserved.
+# License: 3-clause BSD, <https://github.com/smarie/python-pyfields/blob/master/LICENSE>
 import sys
 from copy import copy, deepcopy
 from inspect import getmro, isclass
 
 try:
     from typing import Union, Type, TypeVar
     T = TypeVar('T')
```

### Comparing `pyfields-1.7.0/pyfields/init_makers.py` & `pyfields-1.7.1/pyfields/init_makers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-#  Authors: Sylvain Marie <sylvain.marie@se.com>
+# Authors: Sylvain MARIE <sylvain.marie@se.com>
+#          + All contributors to <https://github.com/smarie/python-pyfields>
 #
-#  Copyright (c) Schneider Electric Industries, 2019. All right reserved.
+# License: 3-clause BSD, <https://github.com/smarie/python-pyfields/blob/master/LICENSE>
 import sys
 from inspect import isfunction, getmro
 from itertools import islice
 
 try:
     from inspect import signature, Parameter, Signature
 except ImportError:
     from funcsigs import signature, Parameter, Signature
 
 
 try:  # python 3.5+
-    from typing import Optional, Set, List, Callable, Dict, Type, Any, TypeVar, Union, Iterable, Tuple, Mapping
-    from valid8.common_syntax import ValidationFuncs
+    from typing import List, Callable, Any, Union, Iterable, Tuple
     use_type_hints = sys.version_info > (3, 0)
 except ImportError:
     use_type_hints = False
 
 
 from makefun import wraps, with_signature
 
@@ -325,15 +325,16 @@
                        _auto_fix_fields=True)
 
         # create the init method
         new_init = create_init(fields=fields, inject_fields=self.user_init_is_injected,
                                user_init_fun=self.user_init_fun, user_init_args_before=self.user_init_args_before)
 
         # replace it forever in the class
-        setattr(objtype, '__init__', new_init)
+        # setattr(objtype, '__init__', new_init)
+        objtype.__init__ = new_init
 
         # return the new init
         return new_init.__get__(obj, objtype)
 
 
 class InjectedInitFieldsArg(object):
     """
```

### Comparing `pyfields-1.7.0/pyfields/tests/_test_benchmarks.py` & `pyfields-1.7.1/pyfields/tests/_test_benchmarks.py`

 * *Files identical despite different names*

### Comparing `pyfields-1.7.0/pyfields/tests/_test_py36.py` & `pyfields-1.7.1/pyfields/tests/_test_py36.py`

 * *Files identical despite different names*

### Comparing `pyfields-1.7.0/pyfields/tests/issues/_test_py36.py` & `pyfields-1.7.1/pyfields/tests/issues/_test_py36.py`

 * *Files identical despite different names*

### Comparing `pyfields-1.7.0/pyfields/tests/issues/_test_py36_pep563.py` & `pyfields-1.7.1/pyfields/tests/issues/_test_py36_pep563.py`

 * *Files identical despite different names*

### Comparing `pyfields-1.7.0/pyfields/tests/issues/test_issue_53.py` & `pyfields-1.7.1/pyfields/tests/issues/test_issue_53.py`

 * *Files identical despite different names*

### Comparing `pyfields-1.7.0/pyfields/tests/issues/test_issue_73.py` & `pyfields-1.7.1/pyfields/tests/issues/test_issue_73.py`

 * *Files identical despite different names*

### Comparing `pyfields-1.7.0/pyfields/tests/issues/test_issue_81.py` & `pyfields-1.7.1/pyfields/tests/issues/test_issue_81.py`

 * *Files identical despite different names*

### Comparing `pyfields-1.7.0/pyfields/tests/issues/test_issue_84.py` & `pyfields-1.7.1/pyfields/tests/issues/test_issue_84.py`

 * *Files identical despite different names*

### Comparing `pyfields-1.7.0/pyfields/tests/test_autofields.py` & `pyfields-1.7.1/pyfields/tests/test_autofields.py`

 * *Files identical despite different names*

### Comparing `pyfields-1.7.0/pyfields/tests/test_core.py` & `pyfields-1.7.1/pyfields/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `pyfields-1.7.0/pyfields/tests/test_helpers.py` & `pyfields-1.7.1/pyfields/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `pyfields-1.7.0/pyfields/tests/test_init.py` & `pyfields-1.7.1/pyfields/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `pyfields-1.7.0/pyfields/tests/test_readme.py` & `pyfields-1.7.1/pyfields/tests/test_readme.py`

 * *Files identical despite different names*

### Comparing `pyfields-1.7.0/pyfields/tests/test_so.py` & `pyfields-1.7.1/pyfields/tests/test_so.py`

 * *Files identical despite different names*

### Comparing `pyfields-1.7.0/pyfields/typing_utils.py` & `pyfields-1.7.1/pyfields/typing_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,30 @@
-#  Authors: Sylvain Marie <sylvain.marie@se.com>
+# Authors: Sylvain MARIE <sylvain.marie@se.com>
+#          + All contributors to <https://github.com/smarie/python-pyfields>
 #
-#  Copyright (c) Schneider Electric Industries, 2019. All right reserved.
+# License: 3-clause BSD, <https://github.com/smarie/python-pyfields/blob/master/LICENSE>
 import sys
 
+from pkg_resources import get_distribution
+
 
 class FieldTypeError(TypeError):  # FieldError
     """
     Error raised when the type of a field does not match expected type(s).
     """
     __slots__ = ('field', 'value', 'expected_types')
 
     def __init__(self, field, value, expected_types):
         self.field = field
         self.value = value
         # noinspection PyBroadException
         try:
             if len(expected_types) == 1:
                 expected_types = expected_types[0]
-        except:
+        except BaseException:
             pass
         self.expected_types = expected_types
 
     def __str__(self):
         # representing the object might fail, protect ourselves
         # noinspection PyBroadException
         try:
@@ -40,15 +43,27 @@
 
         return "Invalid value type provided for '%s'. %s. Instead, received a '%s': %s"\
                % (self.field.qualname, sub_msg, self.value.__class__.__name__, val_repr)
 
 
 def _make_assert_is_of_type():
     try:
-        from typeguard import check_type
+        from typeguard import check_type as ct
+        from packaging.version import parse as parse_version
+
+        # Note: only do this when we are sure that typeguard can be imported, otherwise this is slow
+        # see https://github.com/smarie/python-getversion/blob/ee495acf6cf06c5e860713edeee396206368e458/getversion/main.py#L84
+        typeguard_version = get_distribution("typeguard").version
+        if parse_version(typeguard_version) < parse_version("3.0.0"):
+            check_type = ct
+        else:
+            # Name has disappeared from 3.0.0
+            def check_type(name, value, typ):
+                ct(value, typ)
+
         try:
             from typing import Union
         except ImportError:
             # (a) typing is not available, transform iterables of types into several calls
             def assert_is_of_type(field, value, typ):
                 """
                 Type checker relying on `typeguard` (python 3.5+)
@@ -69,20 +84,20 @@
                         # raise from
                         new_e = FieldTypeError(field, value, typ)
                         new_e.__cause__ = e
                         raise new_e
                 else:
                     # iterate and try them all
                     e = None
-                    for t in t_gen:
+                    for _t in t_gen:
                         try:
                             check_type(field.qualname, value, typ)
                             return  # success !!!!
-                        except Exception as e:
-                            pass    # failed: lets try another one
+                        except Exception as e1:
+                            e = e1  # failed: lets try another one
 
                     # raise from
                     if e is not None:
                         new_e = FieldTypeError(field, value, typ)
                         new_e.__cause__ = e
                         raise new_e
 
@@ -126,15 +141,15 @@
                     new_e.__cause__ = e
                     raise new_e
                 else:
                     if not valid:
                         raise FieldTypeError(field, value, typ)
 
         except ImportError:
-            from valid8.utils.typing_inspect import is_typevar, is_union_type, get_args
+            # from valid8.utils.typing_inspect import is_typevar, is_union_type, get_args
             from valid8.utils.typing_tools import resolve_union_and_typevar
 
             def assert_is_of_type(field, value, typ):
                 """
                 Neither `typeguard` nor `pytypes` are available on this platform.
 
                 This is a "light" implementation that basically resolves all `Union` and `TypeVar` into a flat list and
@@ -159,15 +174,15 @@
                         raise FieldTypeError(field, value, typ)
 
     return assert_is_of_type
 
 
 try:  # very minimal way to check if typing it available, for runtime type checking
     # noinspection PyUnresolvedReferences
-    from typing import Tuple
+    from typing import Tuple  # noqa
     assert_is_of_type = _make_assert_is_of_type()
 except ImportError:
     assert_is_of_type = None
 
 
 PY36 = sys.version_info >= (3, 6)
 get_type_hints = None
```

### Comparing `pyfields-1.7.0/pyfields/validate_n_convert.py` & `pyfields-1.7.1/pyfields/validate_n_convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,40 @@
-#  Authors: Sylvain Marie <sylvain.marie@se.com>
+# Authors: Sylvain MARIE <sylvain.marie@se.com>
+#          + All contributors to <https://github.com/smarie/python-pyfields>
 #
-#  Copyright (c) Schneider Electric Industries, 2019. All right reserved.
+# License: 3-clause BSD, <https://github.com/smarie/python-pyfields/blob/master/LICENSE>
 import sys
 from collections import OrderedDict
 
 from valid8 import Validator, failure_raiser, ValidationError, ValidationFailure
 from valid8.base import getfullargspec as v8_getfullargspec, get_callable_name, is_mini_lambda
 from valid8.common_syntax import FunctionDefinitionError, make_validation_func_callables
 from valid8.composition import _and_
 from valid8.entry_points import _add_none_handler
 from valid8.utils.signature_tools import IsBuiltInError
 from valid8.validation_lib import instance_of
 
 try:  # python 3.5+
     # noinspection PyUnresolvedReferences
     from typing import Callable, Type, Any, TypeVar, Union, Iterable, Tuple, Mapping, Optional, Dict, Literal
-    from valid8.common_syntax import ValidationFuncs
+    # from valid8.common_syntax import ValidationFuncs
     use_type_hints = sys.version_info > (3, 0)
 except ImportError:
     use_type_hints = False
 
 
 if use_type_hints:
     T = TypeVar('T')
 
     # ------------- validator type hints -----------
     # 1. the lowest-level user or 3d party-provided validation functions
     ValidationFunc = Union[Callable[[Any], Any],
                            Callable[[Any, Any], Any],
                            Callable[[Any, Any, Any], Any]]
-    """A validation function is a callable with signature (val), (obj, val) or (obj, field, val), returning `True` 
+    """A validation function is a callable with signature (val), (obj, val) or (obj, field, val), returning `True`
     or `None` in case of success"""
 
     try:
         # noinspection PyUnresolvedReferences
         from mini_lambda import y
         ValidationFuncOrLambda = Union[ValidationFunc, type(y)]
     except ImportError:
@@ -51,16 +52,16 @@
     VFDefinitionElement = Union[str, Type[ValidationFailure], ValidationFuncOrLambda]
     """This type represents one of the elements that can define a checker: help msg, failure type, callable"""
 
     OneOrSeveralVFDefinitions = Union[ValidatorDef,
                                       Iterable[ValidatorDef],
                                       Mapping[VFDefinitionElement, Union[VFDefinitionElement,
                                                                          Tuple[VFDefinitionElement, ...]]]]
-    """Several validators can be provided as a singleton, iterable, or dict-like. In that case the value can be a 
-    single variable or a tuple, and it will be combined with the key to form the validator. So you can use any of 
+    """Several validators can be provided as a singleton, iterable, or dict-like. In that case the value can be a
+    single variable or a tuple, and it will be combined with the key to form the validator. So you can use any of
     the elements defining a validators as the key."""
 
     # shortcut name used everywhere. Less explicit
     Validators = OneOrSeveralVFDefinitions
 
 
 class FieldValidator(Validator):
@@ -167,15 +168,15 @@
                 # nbkwargs = 0
                 # nbdefaults = 0
 
             if nb_args == 0 and nbvarargs == 0:
                 raise ValueError(
                     "validation function should accept 1, 2, or 3 arguments at least. `f(val)`, `f(obj, val)` or "
                     "`f(obj, field, val)`")
-            elif nb_args == 1 or (nb_args == 0 and nbvarargs >= 1):  # varargs default to one argument (compliance with old mini lambda)
+            elif nb_args == 1 or (nb_args == 0 and nbvarargs >= 1):  # varargs default to one argument (compliance with old mini lambda)  # noqa
                 # `f(val)`
                 def new_validation_callable(val, **ctx):
                     return validation_callable(val)
             elif nb_args == 2:
                 # `f(obj, val)`
                 def new_validation_callable(val, **ctx):
                     return validation_callable(ctx['obj'], val)
@@ -333,15 +334,15 @@
 
 if use_type_hints:
     # --------------converter type hints
     # 1. the lowest-level user or 3d party-provided validation functions
     ConverterFunc = Union[Callable[[Any], Any],
                           Callable[[Any, Any], Any],
                           Callable[[Any, Any, Any], Any]]
-    """A converter function is a callable with signature (val), (obj, val) or (obj, field, val), returning the 
+    """A converter function is a callable with signature (val), (obj, val) or (obj, field, val), returning the
     converted value in case of success"""
 
     try:
         # noinspection PyUnresolvedReferences
         from mini_lambda import y
 
         ConverterFuncOrLambda = Union[ConverterFunc, type(y)]
@@ -360,23 +361,24 @@
     OneOrSeveralConverterDefinitions = Union[Converter,
                                              ConverterFuncOrLambda,
                                              Iterable[Tuple[TypeDef, ConverterFuncOrLambda]],
                                              Mapping[TypeDef, ConverterFuncOrLambda]]
     Converters = OneOrSeveralConverterDefinitions
 
 
-def make_3params_callable(f,                    # Union[ValidationFunc, ConverterFunc]
+def make_3params_callable(f,                    # type: Union[ValidationFunc, ConverterFunc]
                           is_mini_lambda=False  # type: bool
                           ):
     # type: (...) -> Callable[[Any, 'Field', Any], Any]
     """
     Transforms the provided validation or conversion callable into a callable with 3 arguments (obj, field, val).
 
     :param f:
-    :param is_mini_lambda: a boolean indicating if the function comes from a mini lambda. In which case we know the signature has one param only (x)
+    :param is_mini_lambda: a boolean indicating if the function comes from a mini lambda. In which case we know the
+        signature has one param only (x)
     :return:
     """
     # support several cases for the function signature
     # `f(val)`, `f(obj, val)` or `f(obj, field, val)`
     if is_mini_lambda:
         nbargs = 1
         nbvarargs = 0
@@ -596,15 +598,15 @@
         super(ConversionError, self).__init__()
 
     def __str__(self):
         return "Unable to convert value %r. Results:\n%s" \
                % (self.value_to_convert, err_dct_to_str(self.err_dct))
 
 
-def err_dct_to_str(err_dct  # Dict[Converter, str]
+def err_dct_to_str(err_dct  # type: Dict[Converter, str]
                    ):
     # type: (...) -> str
     msg = ""
     for converter, err in err_dct.items():
         msg += " - Converter '%s': %s\n" % (converter, err)
 
     return msg
@@ -613,15 +615,15 @@
 class DetailedConversionResults(object):
     """
     Returned by `trace_convert` for detailed results about which converter failed before the winning one.
     """
     __slots__ = 'value_to_convert', 'field', 'obj', 'err_dct', 'winning_converter', 'converted_value'
 
     def __init__(self, value_to_convert, field, obj, err_dct, winning_converter, converted_value):
-        self.value_to_convert= value_to_convert
+        self.value_to_convert = value_to_convert
         self.field = field
         self.obj = obj
         self.err_dct = err_dct
         self.winning_converter = winning_converter
         self.converted_value = converted_value
 
     def __str__(self):
```

### Comparing `pyfields-1.7.0/pyfields/validate_n_convert.pyi` & `pyfields-1.7.1/pyfields/validate_n_convert.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-#  Authors: Sylvain Marie <sylvain.marie@se.com>
+# Authors: Sylvain MARIE <sylvain.marie@se.com>
+#          + All contributors to <https://github.com/smarie/python-pyfields>
 #
-#  Copyright (c) Schneider Electric Industries, 2019. All right reserved.
-
+# License: 3-clause BSD, <https://github.com/smarie/python-pyfields/blob/master/LICENSE>
 from valid8 import Validator, ValidationError, ValidationFailure
 from valid8.base import getfullargspec as v8_getfullargspec, get_callable_name, is_mini_lambda
 
 from typing import Callable, Type, Any, TypeVar, Union, Iterable, Tuple, Mapping, Optional, Dict, Literal
 
 
 T = TypeVar('T')
```

### Comparing `pyfields-1.7.0/pyfields.egg-info/PKG-INFO` & `pyfields-1.7.1/pyfields.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 Metadata-Version: 2.1
 Name: pyfields
-Version: 1.7.0
+Version: 1.7.1
 Summary: Define fields in python classes. Easily.
 Home-page: https://github.com/smarie/python-pyfields
+Download-URL: https://github.com/smarie/python-pyfields/tarball/1.7.1
 Author: Sylvain MARIE <sylvain.marie@se.com>
 Maintainer: Sylvain MARIE <sylvain.marie@se.com>
 License: BSD 3-Clause
-Download-URL: https://github.com/smarie/python-pyfields/tarball/1.7.0
-Description: # python-pyfields
-        
-        *Define fields in python classes. Easily.*
-        
-        [![Python versions](https://img.shields.io/pypi/pyversions/pyfields.svg)](https://pypi.python.org/pypi/pyfields/) [![Build Status](https://github.com/smarie/python-pyfields/actions/workflows/base.yml/badge.svg)](https://github.com/smarie/python-pyfields/actions/workflows/base.yml) [![Tests Status](https://smarie.github.io/python-pyfields/reports/junit/junit-badge.svg?dummy=8484744)](https://smarie.github.io/python-pyfields/reports/junit/report.html) [![codecov](https://codecov.io/gh/smarie/python-pyfields/branch/main/graph/badge.svg)](https://codecov.io/gh/smarie/python-pyfields)
-        
-        [![Documentation](https://img.shields.io/badge/doc-latest-blue.svg)](https://smarie.github.io/python-pyfields/) [![PyPI](https://img.shields.io/pypi/v/pyfields.svg)](https://pypi.python.org/pypi/pyfields/) [![Downloads](https://pepy.tech/badge/pyfields)](https://pepy.tech/project/pyfields) [![Downloads per week](https://pepy.tech/badge/pyfields/week)](https://pepy.tech/project/pyfields) [![GitHub stars](https://img.shields.io/github/stars/smarie/python-pyfields.svg)](https://github.com/smarie/python-pyfields/stargazers)
-        
-        The documentation for users is available here: [https://smarie.github.io/python-pyfields/](https://smarie.github.io/python-pyfields/)
-        
-        A readme for developers is available here: [https://github.com/smarie/python-pyfields](https://github.com/smarie/python-pyfields)
-        
 Keywords: object class boilerplate oop field attr member descriptor attribute mix-in mixin validation type-check
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# python-pyfields
+
+*Define fields in python classes. Easily.*
+
+[![Python versions](https://img.shields.io/pypi/pyversions/pyfields.svg)](https://pypi.python.org/pypi/pyfields/) [![Build Status](https://github.com/smarie/python-pyfields/actions/workflows/base.yml/badge.svg)](https://github.com/smarie/python-pyfields/actions/workflows/base.yml) [![Tests Status](https://smarie.github.io/python-pyfields/reports/junit/junit-badge.svg?dummy=8484744)](https://smarie.github.io/python-pyfields/reports/junit/report.html) [![Coverage Status](https://smarie.github.io/python-pyfields/reports/coverage/coverage-badge.svg?dummy=8484744)](https://smarie.github.io/python-pyfields/reports/coverage/index.html) [![codecov](https://codecov.io/gh/smarie/python-pyfields/branch/main/graph/badge.svg)](https://codecov.io/gh/smarie/python-pyfields) [![Flake8 Status](https://smarie.github.io/python-pyfields/reports/flake8/flake8-badge.svg?dummy=8484744)](https://smarie.github.io/python-pyfields/reports/flake8/index.html)
+
+[![Documentation](https://img.shields.io/badge/doc-latest-blue.svg)](https://smarie.github.io/python-pyfields/) [![PyPI](https://img.shields.io/pypi/v/pyfields.svg)](https://pypi.python.org/pypi/pyfields/) [![Downloads](https://pepy.tech/badge/pyfields)](https://pepy.tech/project/pyfields) [![Downloads per week](https://pepy.tech/badge/pyfields/week)](https://pepy.tech/project/pyfields) [![GitHub stars](https://img.shields.io/github/stars/smarie/python-pyfields.svg)](https://github.com/smarie/python-pyfields/stargazers)
+
+The documentation for users is available here: [https://smarie.github.io/python-pyfields/](https://smarie.github.io/python-pyfields/)
+
+A readme for developers is available here: [https://github.com/smarie/python-pyfields](https://github.com/smarie/python-pyfields)
```

### Comparing `pyfields-1.7.0/pyfields.egg-info/SOURCES.txt` & `pyfields-1.7.1/pyfields.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 .gitignore
 LICENSE
 README.md
+mkdocs.yml
 noxfile-requirements.txt
 noxfile.py
 pyproject.toml
 setup.cfg
 setup.py
 .github/workflows/base.yml
 ci_tools/.pylintrc
 ci_tools/check_python_version.py
-ci_tools/generate-junit-badge.py
+ci_tools/flake8-requirements.txt
 ci_tools/github_release.py
 ci_tools/nox_utils.py
 docs/api_reference.md
 docs/changelog.md
 docs/index.md
 docs/long_description.md
-docs/mkdocs.yml
 docs/why.md
 docs/imgs/autocomplete1.png
 pyfields/__init__.py
 pyfields/_version.py
 pyfields/autofields_.py
 pyfields/core.py
 pyfields/helpers.py
```

### Comparing `pyfields-1.7.0/pyproject.toml` & `pyfields-1.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyfields-1.7.0/setup.cfg` & `pyfields-1.7.1/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 	Programming Language :: Python :: 2
 	Programming Language :: Python :: 2.7
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.5
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
+	Programming Language :: Python :: 3.9
 
 [options]
 setup_requires = 
 	setuptools_scm
 	pytest-runner
 install_requires = 
 	valid8>=5.0
@@ -75,11 +76,28 @@
 [coverage:report]
 fail_under = 70
 show_missing = True
 exclude_lines = 
 	except ImportError:
 	pragma: no cover
 
+[flake8]
+max-line-length = 120
+extend-ignore = D, E203  # D: Docstring errors, E203: see https://github.com/PyCQA/pycodestyle/issues/373
+copyright-check = True
+copyright-regexp = ^\#\s+Authors:\s+Sylvain MARIE <sylvain\.marie@se\.com>\n\#\s+\+\sAll\scontributors\sto\s<https://github\.com/smarie/python\-pyfields>\n\#\n\#\s+License:\s3\-clause\sBSD,\s<https://github\.com/smarie/python\-pyfields/blob/master/LICENSE>
+exclude = 
+	.git
+	.github
+	.nox
+	.pytest_cache
+	ci_tools
+	docs
+	*/tests
+	noxfile.py
+	setup.py
+	*/_version.py
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `pyfields-1.7.0/setup.py` & `pyfields-1.7.1/setup.py`

 * *Files identical despite different names*

