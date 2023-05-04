# Comparing `tmp/demes-0.2.2.tar.gz` & `tmp/demes-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "demes-0.2.2.tar", last modified: Thu Apr 28 13:45:22 2022, max compression
+gzip compressed data, was "demes-0.2.3.tar", last modified: Thu May  4 19:30:44 2023, max compression
```

## Comparing `demes-0.2.2.tar` & `demes-0.2.3.tar`

### file list

```diff
@@ -1,78 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 13:45:22.149172 demes-0.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 13:45:22.141172 demes-0.2.2/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      221 2022-04-28 13:45:07.000000 demes-0.2.2/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1301 2022-04-28 13:45:07.000000 demes-0.2.2/.github/mergify.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 13:45:22.141172 demes-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      605 2022-04-28 13:45:07.000000 demes-0.2.2/.github/workflows/dev.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2390 2022-04-28 13:45:07.000000 demes-0.2.2/.github/workflows/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      793 2022-04-28 13:45:07.000000 demes-0.2.2/.github/workflows/lint.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1492 2022-04-28 13:45:07.000000 demes-0.2.2/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2244 2022-04-28 13:45:07.000000 demes-0.2.2/.github/workflows/wheel.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-04-28 13:45:07.000000 demes-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-04-28 13:45:07.000000 demes-0.2.2/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (121)      805 2022-04-28 13:45:07.000000 demes-0.2.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     7120 2022-04-28 13:45:07.000000 demes-0.2.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)      732 2022-04-28 13:45:07.000000 demes-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2083 2022-04-28 13:45:22.149172 demes-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      989 2022-04-28 13:45:07.000000 demes-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 13:45:22.145172 demes-0.2.2/demes/
--rw-r--r--   0 runner    (1001) docker     (121)     1171 2022-04-28 13:45:07.000000 demes-0.2.2/demes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7961 2022-04-28 13:45:07.000000 demes-0.2.2/demes/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-04-28 13:45:21.000000 demes-0.2.2/demes/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)   109310 2022-04-28 13:45:07.000000 demes-0.2.2/demes/demes.py
--rw-r--r--   0 runner    (1001) docker     (121)    11792 2022-04-28 13:45:07.000000 demes-0.2.2/demes/load_dump.py
--rw-r--r--   0 runner    (1001) docker     (121)    37805 2022-04-28 13:45:07.000000 demes-0.2.2/demes/ms.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-28 13:45:07.000000 demes-0.2.2/demes/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 13:45:22.145172 demes-0.2.2/demes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2083 2022-04-28 13:45:21.000000 demes-0.2.2/demes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1452 2022-04-28 13:45:22.000000 demes-0.2.2/demes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-28 13:45:21.000000 demes-0.2.2/demes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-04-28 13:45:21.000000 demes-0.2.2/demes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-28 13:45:21.000000 demes-0.2.2/demes.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-04-28 13:45:22.000000 demes-0.2.2/demes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-04-28 13:45:22.000000 demes-0.2.2/demes.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 13:45:22.145172 demes-0.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     7120 2022-04-28 13:45:07.000000 demes-0.2.2/docs/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)      395 2022-04-28 13:45:07.000000 demes-0.2.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     1376 2022-04-28 13:45:07.000000 demes-0.2.2/docs/_config.yml
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-04-28 13:45:07.000000 demes-0.2.2/docs/_toc.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1161 2022-04-28 13:45:07.000000 demes-0.2.2/docs/api.md
--rwxr-xr-x   0 runner    (1001) docker     (121)      502 2022-04-28 13:45:07.000000 demes-0.2.2/docs/build.sh
--rw-r--r--   0 runner    (1001) docker     (121)      196 2022-04-28 13:45:07.000000 demes-0.2.2/docs/cli.md
--rw-r--r--   0 runner    (1001) docker     (121)      796 2022-04-28 13:45:07.000000 demes-0.2.2/docs/convert_changelog.py
--rw-r--r--   0 runner    (1001) docker     (121)     5761 2022-04-28 13:45:07.000000 demes-0.2.2/docs/development.md
--rw-r--r--   0 runner    (1001) docker     (121)      222 2022-04-28 13:45:07.000000 demes-0.2.2/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (121)     2494 2022-04-28 13:45:07.000000 demes-0.2.2/docs/introduction.md
--rw-r--r--   0 runner    (1001) docker     (121)      914 2022-04-28 13:45:07.000000 demes-0.2.2/docs/is_new_stable.py
--rw-r--r--   0 runner    (1001) docker     (121)     5127 2022-04-28 13:45:07.000000 demes-0.2.2/docs/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (121)     1456 2022-04-28 13:45:07.000000 demes-0.2.2/docs/release.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 13:45:22.149172 demes-0.2.2/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      314 2022-04-28 13:45:07.000000 demes-0.2.2/examples/bottleneck.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1368 2022-04-28 13:45:07.000000 demes-0.2.2/examples/browning_america.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      801 2022-04-28 13:45:07.000000 demes-0.2.2/examples/cloning_example.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-04-28 13:45:07.000000 demes-0.2.2/examples/gutenkunst_ooa.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2784 2022-04-28 13:45:07.000000 demes-0.2.2/examples/jacobs_papuans.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      699 2022-04-28 13:45:07.000000 demes-0.2.2/examples/linear_size_function_example.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      912 2022-04-28 13:45:07.000000 demes-0.2.2/examples/offshoots.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      812 2022-04-28 13:45:07.000000 demes-0.2.2/examples/selfing_example.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      256 2022-04-28 13:45:07.000000 demes-0.2.2/examples/two_epoch.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      692 2022-04-28 13:45:07.000000 demes-0.2.2/examples/zigzag.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      144 2022-04-28 13:45:07.000000 demes-0.2.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 13:45:22.149172 demes-0.2.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)      107 2022-04-28 13:45:07.000000 demes-0.2.2/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-04-28 13:45:07.000000 demes-0.2.2/requirements/lint.txt
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-04-28 13:45:07.000000 demes-0.2.2/requirements/minimal.txt
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-04-28 13:45:07.000000 demes-0.2.2/requirements/tests.txt
--rw-r--r--   0 runner    (1001) docker     (121)      135 2022-04-28 13:45:07.000000 demes-0.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2210 2022-04-28 13:45:22.149172 demes-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      283 2022-04-28 13:45:07.000000 demes-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 13:45:22.149172 demes-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      521 2022-04-28 13:45:07.000000 demes-0.2.2/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3348 2022-04-28 13:45:07.000000 demes-0.2.2/tests/ms_asymmetric_migration.sh
--rw-r--r--   0 runner    (1001) docker     (121)     7746 2022-04-28 13:45:07.000000 demes-0.2.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)   151028 2022-04-28 13:45:07.000000 demes-0.2.2/tests/test_demes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1709 2022-04-28 13:45:07.000000 demes-0.2.2/tests/test_import_visibility.py
--rw-r--r--   0 runner    (1001) docker     (121)    27662 2022-04-28 13:45:07.000000 demes-0.2.2/tests/test_load_dump.py
--rw-r--r--   0 runner    (1001) docker     (121)    88516 2022-04-28 13:45:07.000000 demes-0.2.2/tests/test_ms.py
--rw-r--r--   0 runner    (1001) docker     (121)     3146 2022-04-28 13:45:07.000000 demes-0.2.2/tests/test_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)    13625 2022-04-28 13:45:07.000000 demes-0.2.2/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 19:30:44.009119 demes-0.2.3/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 19:30:43.993119 demes-0.2.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (122)      221 2023-05-04 19:30:30.000000 demes-0.2.3/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1301 2023-05-04 19:30:30.000000 demes-0.2.3/.github/mergify.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 19:30:43.993119 demes-0.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      651 2023-05-04 19:30:30.000000 demes-0.2.3/.github/workflows/dev.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     2421 2023-05-04 19:30:30.000000 demes-0.2.3/.github/workflows/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      793 2023-05-04 19:30:30.000000 demes-0.2.3/.github/workflows/lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1493 2023-05-04 19:30:30.000000 demes-0.2.3/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     2244 2023-05-04 19:30:30.000000 demes-0.2.3/.github/workflows/wheel.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-05-04 19:30:30.000000 demes-0.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-05-04 19:30:30.000000 demes-0.2.3/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (122)      758 2023-05-04 19:30:30.000000 demes-0.2.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     7370 2023-05-04 19:30:30.000000 demes-0.2.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)      710 2023-05-04 19:30:30.000000 demes-0.2.3/CITATION.md
+-rw-r--r--   0 runner    (1001) docker     (122)      732 2023-05-04 19:30:30.000000 demes-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1862 2023-05-04 19:30:44.009119 demes-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      989 2023-05-04 19:30:30.000000 demes-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 19:30:43.997119 demes-0.2.3/demes/
+-rw-r--r--   0 runner    (1001) docker     (122)     1171 2023-05-04 19:30:30.000000 demes-0.2.3/demes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7913 2023-05-04 19:30:30.000000 demes-0.2.3/demes/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-05-04 19:30:43.000000 demes-0.2.3/demes/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)   113924 2023-05-04 19:30:30.000000 demes-0.2.3/demes/demes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12678 2023-05-04 19:30:30.000000 demes-0.2.3/demes/load_dump.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38354 2023-05-04 19:30:30.000000 demes-0.2.3/demes/ms.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-04 19:30:30.000000 demes-0.2.3/demes/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 19:30:43.997119 demes-0.2.3/demes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1862 2023-05-04 19:30:43.000000 demes-0.2.3/demes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1519 2023-05-04 19:30:43.000000 demes-0.2.3/demes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-04 19:30:43.000000 demes-0.2.3/demes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       45 2023-05-04 19:30:43.000000 demes-0.2.3/demes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-04 19:30:43.000000 demes-0.2.3/demes.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       35 2023-05-04 19:30:43.000000 demes-0.2.3/demes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-04 19:30:43.000000 demes-0.2.3/demes.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 19:30:44.001119 demes-0.2.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     7370 2023-05-04 19:30:30.000000 demes-0.2.3/docs/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)      710 2023-05-04 19:30:30.000000 demes-0.2.3/docs/CITATION.md
+-rw-r--r--   0 runner    (1001) docker     (122)      253 2023-05-04 19:30:30.000000 demes-0.2.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-05-04 19:30:30.000000 demes-0.2.3/docs/_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 19:30:44.001119 demes-0.2.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (122)      566 2023-05-04 19:30:30.000000 demes-0.2.3/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (122)      181 2023-05-04 19:30:30.000000 demes-0.2.3/docs/_toc.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1192 2023-05-04 19:30:30.000000 demes-0.2.3/docs/api.md
+-rwxr-xr-x   0 runner    (1001) docker     (122)      502 2023-05-04 19:30:30.000000 demes-0.2.3/docs/build.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      237 2023-05-04 19:30:30.000000 demes-0.2.3/docs/cli.md
+-rw-r--r--   0 runner    (1001) docker     (122)      796 2023-05-04 19:30:30.000000 demes-0.2.3/docs/convert_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5761 2023-05-04 19:30:30.000000 demes-0.2.3/docs/development.md
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-05-04 19:30:30.000000 demes-0.2.3/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (122)      222 2023-05-04 19:30:30.000000 demes-0.2.3/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (122)     2478 2023-05-04 19:30:30.000000 demes-0.2.3/docs/introduction.md
+-rw-r--r--   0 runner    (1001) docker     (122)      914 2023-05-04 19:30:30.000000 demes-0.2.3/docs/is_new_stable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4901 2023-05-04 19:30:30.000000 demes-0.2.3/docs/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1456 2023-05-04 19:30:30.000000 demes-0.2.3/docs/release.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 19:30:44.009119 demes-0.2.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (122)      314 2023-05-04 19:30:30.000000 demes-0.2.3/examples/bottleneck.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1368 2023-05-04 19:30:30.000000 demes-0.2.3/examples/browning_america.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      801 2023-05-04 19:30:30.000000 demes-0.2.3/examples/cloning_example.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1070 2023-05-04 19:30:30.000000 demes-0.2.3/examples/gutenkunst_ooa.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     2784 2023-05-04 19:30:30.000000 demes-0.2.3/examples/jacobs_papuans.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      699 2023-05-04 19:30:30.000000 demes-0.2.3/examples/linear_size_function_example.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      912 2023-05-04 19:30:30.000000 demes-0.2.3/examples/offshoots.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      812 2023-05-04 19:30:30.000000 demes-0.2.3/examples/selfing_example.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      256 2023-05-04 19:30:30.000000 demes-0.2.3/examples/two_epoch.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      692 2023-05-04 19:30:30.000000 demes-0.2.3/examples/zigzag.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      144 2023-05-04 19:30:30.000000 demes-0.2.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 19:30:44.009119 demes-0.2.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      115 2023-05-04 19:30:30.000000 demes-0.2.3/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       40 2023-05-04 19:30:30.000000 demes-0.2.3/requirements/lint.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       35 2023-05-04 19:30:30.000000 demes-0.2.3/requirements/minimal.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      118 2023-05-04 19:30:30.000000 demes-0.2.3/requirements/tests.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-05-04 19:30:30.000000 demes-0.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2053 2023-05-04 19:30:44.009119 demes-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      283 2023-05-04 19:30:30.000000 demes-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 19:30:44.009119 demes-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      521 2023-05-04 19:30:30.000000 demes-0.2.3/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3348 2023-05-04 19:30:30.000000 demes-0.2.3/tests/ms_asymmetric_migration.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     7746 2023-05-04 19:30:30.000000 demes-0.2.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)   153333 2023-05-04 19:30:30.000000 demes-0.2.3/tests/test_demes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1709 2023-05-04 19:30:30.000000 demes-0.2.3/tests/test_import_visibility.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28150 2023-05-04 19:30:30.000000 demes-0.2.3/tests/test_load_dump.py
+-rw-r--r--   0 runner    (1001) docker     (122)    88515 2023-05-04 19:30:30.000000 demes-0.2.3/tests/test_ms.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3146 2023-05-04 19:30:30.000000 demes-0.2.3/tests/test_spec.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13625 2023-05-04 19:30:30.000000 demes-0.2.3/verification.py
```

### Comparing `demes-0.2.2/.github/mergify.yml` & `demes-0.2.3/.github/mergify.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 queue_rules:
   - name: default
     conditions:
       - base=main
       - check-success=build-deploy-docs
       - check-success=lint
-      - check-success=dev-deps (macos-11, 3.10)
-      - check-success=dev-deps (ubuntu-20.04, 3.10)
-      - check-success=dev-deps (windows-2022, 3.10)
+      - check-success=dev-deps (macos-11, 3.11)
+      - check-success=dev-deps (ubuntu-20.04, 3.11)
+      - check-success=dev-deps (windows-2022, 3.11)
       - check-success=tests (macos-11, 3.7)
-      - check-success=tests (macos-11, 3.10)
+      - check-success=tests (macos-11, 3.11)
       - check-success=tests (ubuntu-20.04, 3.7)
-      - check-success=tests (ubuntu-20.04, 3.10)
+      - check-success=tests (ubuntu-20.04, 3.11)
       - check-success=tests (windows-2022, 3.7)
-      - check-success=tests (windows-2022, 3.10)
+      - check-success=tests (windows-2022, 3.11)
 
 pull_request_rules:
   - name: automatic merge for Dependabot pull requests
     conditions:
       - base=main
       - author~=^dependabot(|-preview)\[bot\]$
       - label=dependencies
       - check-success=build-deploy-docs
       - check-success=lint
-      - check-success=dev-deps (macos-11, 3.10)
-      - check-success=dev-deps (ubuntu-20.04, 3.10)
-      - check-success=dev-deps (windows-2022, 3.10)
+      - check-success=dev-deps (macos-11, 3.11)
+      - check-success=dev-deps (ubuntu-20.04, 3.11)
+      - check-success=dev-deps (windows-2022, 3.11)
       - check-success=tests (macos-11, 3.7)
-      - check-success=tests (macos-11, 3.10)
+      - check-success=tests (macos-11, 3.11)
       - check-success=tests (ubuntu-20.04, 3.7)
-      - check-success=tests (ubuntu-20.04, 3.10)
+      - check-success=tests (ubuntu-20.04, 3.11)
       - check-success=tests (windows-2022, 3.7)
-      - check-success=tests (windows-2022, 3.10)
+      - check-success=tests (windows-2022, 3.11)
     actions:
       queue:
         name: default
```

### Comparing `demes-0.2.2/.github/workflows/dev.yaml` & `demes-0.2.3/.github/workflows/dev.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -12,20 +12,22 @@
     defaults:
       run:
         shell: bash
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-20.04, windows-2022, macos-11]
-        python-version: ["3.10"]
+        python-version: ["3.11"]
 
     steps:
       - name: checkout
         uses: actions/checkout@v3
 
       - name: setup python
-        uses: actions/setup-python@v3
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: install developer dependencies
-        run: pip install -r requirements.txt
+        run:
+          pip install --upgrade pip
+          pip install -r requirements.txt
```

### Comparing `demes-0.2.2/.github/workflows/docs.yaml` & `demes-0.2.3/.github/workflows/docs.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -14,33 +14,34 @@
     steps:
       - uses: actions/checkout@v3
         with:
           # Fetch the history for all tags and branches
           # so that the correct version string can be constructed
           # by setuptools_scm.
           fetch-depth: 0
-      - uses: actions/setup-python@v3
+      - uses: actions/setup-python@v4
         with:
-          python-version: "3.10"
+          python-version: "3.11"
 
       - name: Install dependencies
         run: |
+          pip install --upgrade pip
           pip install -r requirements/minimal.txt
           pip install -r requirements/docs.txt
           python -m pip install build packaging
 
       - name: Build package
         run: |
           # Generate the version string which appears in the docs.
           python -m build --sdist
 
       - name: Build Docs
         run: |
           cd docs
-          make dist
+          make
 
       - name: Checkout docs site
         if: (!github.event.pull_request)
         uses: actions/checkout@v3
         with:
           repository: popsim-consortium/demes-docs
           token: ${{ secrets.POPSIMBOT_DEMES_DOCS_TOKEN }}
```

### Comparing `demes-0.2.2/.github/workflows/lint.yaml` & `demes-0.2.3/.github/workflows/lint.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     branches: [ main ]
 
 jobs:
   lint:
     runs-on: ubuntu-20.04
     steps:
       - uses: actions/checkout@v3
-      - uses: actions/setup-python@v3
+      - uses: actions/setup-python@v4
         with:
           python-version: "3.10"
 
       - name: Install dependencies
         run: |
           pip install -r requirements/minimal.txt
           pip install -r requirements/lint.txt
```

### Comparing `demes-0.2.2/.github/workflows/tests.yaml` & `demes-0.2.3/.github/workflows/tests.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -7,41 +7,41 @@
     branches: [ main ]
 
 jobs:
   canceller:
     runs-on: ubuntu-20.04
     steps:
       - name: cancel previous runs
-        uses: styfle/cancel-workflow-action@0.9.1
+        uses: styfle/cancel-workflow-action@0.11.0
         with:
           access_token: ${{ github.token }}
 
   tests:
 
     runs-on: ${{ matrix.os }}
     defaults:
       run:
         shell: bash
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-20.04, windows-2022, macos-11]
-        python-version: [3.7, "3.10"]
+        python-version: [3.7, "3.11"]
     env:
       OS: ${{ matrix.os }}
       PYTHON: ${{ matrix.python-version }}
 
     steps:
       - name: checkout
         uses: actions/checkout@v3
         with:
           submodules: true
 
       - name: setup python
-        uses: actions/setup-python@v3
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: install dependencies
         run: |
           pip install -r requirements/minimal.txt
           pip install -r requirements/tests.txt
@@ -55,11 +55,11 @@
 
       - name: run pytest
         run: |
           python -m pytest -n auto \
             --cov=demes --cov-report=term-missing --cov-report=xml -v tests
 
       - name: upload coverage report to codecov
-        uses: codecov/codecov-action@v2.1.0
+        uses: codecov/codecov-action@v3.1.3
         with:
           fail_ci_if_error: true
           env_vars: OS,PYTHON
```

### Comparing `demes-0.2.2/.github/workflows/wheel.yaml` & `demes-0.2.3/.github/workflows/wheel.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -8,28 +8,28 @@
     types: [published]
 
 jobs:
   wheel_build:
     runs-on: ubuntu-20.04
     steps:
       - uses: actions/checkout@v3
-      - uses: actions/setup-python@v3
+      - uses: actions/setup-python@v4
         with:
           python-version: "3.10"
 
       - name: install dependencies
         run: |
           pip install -r requirements/minimal.txt
           pip install build
 
       - name: build wheel
         run: python -m build
 
       - name: upload wheel
-        uses: actions/upload-artifact@v2
+        uses: actions/upload-artifact@v3
         with:
           name: wheel-and-sdist
           path: dist/
 
   wheel_test:
     runs-on: ${{ matrix.os }}
     needs: ['wheel_build']
@@ -40,21 +40,21 @@
       fail-fast: false
       matrix:
         os: [ubuntu-latest, windows-latest, macos-latest]
         python-version: [3.7, 3.8, 3.9, "3.10"]
 
     steps:
       - name: download wheel
-        uses: actions/download-artifact@v2
+        uses: actions/download-artifact@v3
         with:
           name: wheel-and-sdist
           path: dist/
 
       - name: setup python
-        uses: actions/setup-python@v3
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: install
         run: pip install dist/demes-*.whl
 
       - name: test
@@ -67,15 +67,15 @@
             | demes parse --ms 1 -
 
   pypi_upload:
     runs-on: ubuntu-20.04
     needs: ['wheel_test']
     steps:
       - name: download wheel
-        uses: actions/download-artifact@v2
+        uses: actions/download-artifact@v3
         with:
           name: wheel-and-sdist
           path: dist/
 
       - name: publish to test.pypi.org
         if: github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags')
         uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `demes-0.2.2/.pre-commit-config.yaml` & `demes-0.2.3/.pre-commit-config.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 repos:
   - repo: https://github.com/psf/black
-    rev: 22.3.0
+    rev: 23.1.0
     hooks:
       - id: black
         language_version: python3
-  - repo: https://gitlab.com/pycqa/flake8
-    rev: 4.0.1
+  - repo: https://github.com/pycqa/flake8.git
+    rev: 6.0.0
     hooks:
       - id: flake8
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v0.942
+    rev: v1.0.1
     hooks:
       - id: mypy
         additional_dependencies: [attrs==21.4.0]
   - repo: https://github.com/asottile/blacken-docs
-    rev: v1.10.0
+    rev: 1.13.0
     hooks:
       - id: blacken-docs
-        additional_dependencies: [black==21.12b0]
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.0.1
+    rev: v4.4.0
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: check-yaml
       - id: check-added-large-files
       - id: check-merge-conflict
       - id: mixed-line-ending
```

### Comparing `demes-0.2.2/CHANGELOG.md` & `demes-0.2.3/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Changelog
 
+## 0.2.3 - 2023-05-04
+
+- Fixed the use of numpy strings for deme names.
+  ({user}`terhorst`, {user}`grahamgower`, {issue}`495`, {pr}`505`)
+- Added `Graph.rename_demes()` method to return a graph with renamed demes.
+  ({user}`aabiddanda`, {pr}`499`)
+
 ## 0.2.2 - 2022-04-28
 
 Better conformance to the spec. Minor discrepancies between
 demes-python and the reference implementation have been resolved.
 
 - Dropped support for Python 3.6
   ({user}`grahamgower`, {issue}`445`, {pr}`446`)
```

### Comparing `demes-0.2.2/LICENSE` & `demes-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `demes-0.2.2/PKG-INFO` & `demes-0.2.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,22 @@
 Metadata-Version: 2.1
 Name: demes
-Version: 0.2.2
+Version: 0.2.3
 Summary: tools for describing demographic models
 Home-page: https://github.com/popsim-consortium/demes-python
 Author: PopSim Consortium
 License: ISC
 Project-URL: Documentation, https://popsim-consortium.github.io/demes-docs/
 Project-URL: Source Code, https://github.com/popsim-consortium/demes-python/
 Project-URL: Bug Tracker, https://github.com/popsim-consortium/demes-python/issues
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Tools for describing and manipulating demographic models.
@@ -38,9 +33,7 @@
 - A simple declarative high-level format for specifying demographic models. This format is
   intended to be human-readable and to make it easy to correctly specify models.
 - A corresponding low-level format that is an entirely unambiguous and portable description
   of a model, which can be used by many different simulation frameworks as input. Thus,
   we can see part of the role of this package as *compiling* the high-level description of
   a model into the corresponding low-level description.
 - Robust validation of models and reporting of errors for invalid models.
-
-
```

### Comparing `demes-0.2.2/README.md` & `demes-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `demes-0.2.2/demes/__init__.py` & `demes-0.2.3/demes/__init__.py`

 * *Files identical despite different names*

### Comparing `demes-0.2.2/demes/__main__.py` & `demes-0.2.3/demes/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             "--ms",
             metavar="REFERENCE_SIZE",
             type=float,
             default=None,
             help=(
                 "Output ms command line arguments, using the given reference "
                 "population size (N0) to translate into coalescent units "
-                "(see the 'ms' subcommand for interpretation of this value)."
+                "(see the 'ms' subcommand for interpretation of this value). "
                 "The sampling configuration in the output will need editing "
                 "prior to simulation. The order of deme IDs matches the "
                 "order of demes in the input model. "
             ),
         )
 
         parser.add_argument(
@@ -57,17 +57,16 @@
                 "essential details are retained, this is usually easier for "
                 "humans to read. The simplified output is guaranteed to be a "
                 "valid Demes model that can be resolved identically to the "
                 "input model. But exactly which fields are simplified, "
                 "and how simplification is performed, may change over time. "
                 "Thus users should not rely on details of the output such as "
                 "presence or absence of specific fields, or other details "
-                "that do not alter how the model is resolved into a "
-                "fully-qualified model. "
-                "A fully-qualified model is output by default."
+                "that do not alter how the model is resolved. "
+                "A fully-resolved model is output by default."
             ),
         )
         parser.add_argument(
             "filename",
             type=argparse.FileType(),
             help=(
                 "Filename of the model. The special value '-' may be used to "
@@ -143,15 +142,15 @@
 
     Ms commands correspond to a backwards-time model of population dynamics,
     and use coalescent units for times t, population sizes x, and migration
     rates m. These are converted to more familiar units using the reference
     size N0 according to the following rules:
 
      - time (in generations) = 4 * N0 * t,
-     - deme size (haploid individuals) = N0 * x,
+     - deme size (diploid individuals) = N0 * x,
      - migration rate (per generation) = m / (4 * N0).
 
     Deme IDs are 1-based, and migration matrix entry M[i, j] is the
     forwards-time fraction of deme i which is made up of migrants from
     deme j each generation.
 
     Please refer to the ms manual for the precise semantics of each command.
```

### Comparing `demes-0.2.2/demes/demes.py` & `demes-0.2.3/demes/demes.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+from __future__ import annotations
 import copy
 import collections
 import itertools
 import math
 import numbers
 import operator
-from typing import List, Union, Optional, Dict, MutableMapping, Any, Set, Tuple
+from typing import List, Union, Optional, Dict, MutableMapping, Mapping, Any, Set, Tuple
 import warnings
 
 import attr
 
 from .load_dump import dumps as demes_dumps
 
 Number = Union[int, float]
@@ -172,26 +173,37 @@
         if key not in data:
             data[key] = value
 
 
 @attr.s(auto_attribs=True, kw_only=True, slots=True)
 class Epoch:
     """
-    Population size parameters for a deme in a specified time period.
-    Times follow the forwards-in-time convention (time values increase
-    from the present towards the past). The start time of the epoch is
-    the more ancient time, and the end time is more recent, so that the
-    start time must be greater than the end time
-
-    :ivar float start_time: The start time of the epoch.
-    :ivar float ~.end_time: The end time of the epoch (must be specified).
-    :ivar float start_size: Population size at ``start_time``.
-    :ivar float end_size: Population size at ``end_time``.
+    Population parameters for a deme in a specified time interval.
+
+    An epoch spans the open-closed time interval ``(start_time, end_time]``,
+    where ``start_time`` is the more ancient time,
+    and ``end_time`` is more recent.
+    Time values increase from the present towards the past,
+    and ``start_time`` is strictly greater than ``end_time``.
+
+    Epoch objects are not intended to be constructed directly.
+
+    :ivar float start_time:
+        The start time of the epoch.
+        This value is greater than zero and may be infinity.
+    :ivar float end_time:
+        The end time of the epoch.
+        This value is greater than or equal to zero and finite.
+    :ivar float start_size:
+        Population size at ``start_time``.
+    :ivar float end_size:
+        Population size at ``end_time``.
         If ``start_size != end_size``, the population size changes
-        monotonically between the start and end times.
+        between the start and end times according to the
+        ``size_function``.
     :ivar str size_function: The size change function. This is either
         ``constant``, ``exponential`` or ``linear``, though it is possible
         that additional values will be added in the future.
 
          * ``constant``: the deme's size does not change over the epoch.
          * ``exponential``: the deme's size changes exponentially from
            ``start_size`` to ``end_size`` over the epoch.
@@ -239,14 +251,16 @@
         if self.size_function == "constant" and self.start_size != self.end_size:
             raise ValueError("start_size != end_size, but size_function is constant")
 
     @property
     def time_span(self):
         """
         The time span of the epoch.
+
+        :rtype: float
         """
         return self.start_time - self.end_time
 
     def assert_close(
         self,
         other,
         *,
@@ -331,23 +345,26 @@
         except AssertionError:
             return False
 
 
 @attr.s(auto_attribs=True, kw_only=True, slots=True)
 class AsymmetricMigration:
     """
-    Parameters for continuous asymmetric migration.
+    Continuous asymmetric migration.
+
     The source and destination demes follow the forwards-in-time convention,
     where migrants are born in the source deme and (potentially) have children
     in the dest deme.
 
+    AsymmetricMigration objects are not intended to be constructed directly.
+
     :ivar str source: The source deme for asymmetric migration.
     :ivar str dest: The destination deme for asymmetric migration.
     :ivar float start_time: The time at which the migration rate is activated.
-    :ivar float ~.end_time: The time at which the migration rate is deactivated.
+    :ivar float end_time: The time at which the migration rate is deactivated.
     :ivar float rate: The rate of migration per generation.
     """
 
     source: Name = attr.ib(
         validator=[attr.validators.instance_of(str), valid_deme_name]
     )
     dest: Name = attr.ib(validator=[attr.validators.instance_of(str), valid_deme_name])
@@ -426,23 +443,27 @@
         except AssertionError:
             return False
 
 
 @attr.s(auto_attribs=True, kw_only=True, slots=True)
 class Pulse:
     """
-    Parameters for a pulse of migration from one deme to another.
+    An instantaneous pulse of migration from one deme to another.
+
     Source and destination demes follow the forwards-in-time convention,
-    of migrations born in the source deme having children in the dest
-    deme. If more than one source is given, migration is concurrent, so that
-    the sum of the migrant proportions must sum to less than one.
+    where migrants are born in a source deme and (potentially) have children
+    in the dest deme.
+    If more than one source is given, migration is concurrent,
+    and the sum of the migrant proportions sums to less than or equal to one.
+
+    Pulse objects are not intended to be constructed directly.
 
     :ivar list(str) sources: The source deme(s).
     :ivar str dest: The destination deme.
-    :ivar float ~.time: The time of migration.
+    :ivar float time: The time of migration.
     :ivar list(float) proportions: Immediately following migration, the proportion(s)
         of individuals in the destination deme made up of migrant individuals or
         having parents from the source deme(s).
     """
 
     sources: List[Name] = attr.ib(
         validator=attr.validators.and_(
@@ -553,22 +574,24 @@
         except AssertionError:
             return False
 
 
 @attr.s(auto_attribs=True, kw_only=True, slots=True)
 class Split:
     """
-    Parameters for a split event, in which a deme ends at a given time and
+    A split event, in which a deme ends at a given time and
     contributes ancestry to an arbitrary number of descendant demes. Note
     that there could be just a single descendant deme, in which case ``split``
-    is a bit of a misnomer...
+    is a bit of a misnomer.
+
+    Split objects are not intended to be constructed directly.
 
     :ivar str parent: The parental deme.
     :ivar list[str] children: A list of descendant demes.
-    :ivar float ~.time: The split time.
+    :ivar float time: The split time.
     """
 
     parent: Name = attr.ib(
         validator=[attr.validators.instance_of(str), valid_deme_name]
     )
     children: List[Name] = attr.ib(
         validator=attr.validators.and_(
@@ -651,20 +674,22 @@
         except AssertionError:
             return False
 
 
 @attr.s(auto_attribs=True, kw_only=True, slots=True)
 class Branch:
     """
-    Parameters for a branch event, where a new deme branches off from a parental
+    A branch event, where a new deme branches off from a parental
     deme. The parental deme need not end at that time.
 
+    Branch objects are not intended to be constructed directly.
+
     :ivar str parent: The parental deme.
     :ivar str child: The descendant deme.
-    :ivar float ~.time: The branch time.
+    :ivar float time: The branch time.
     """
 
     parent: Name = attr.ib(
         validator=[attr.validators.instance_of(str), valid_deme_name]
     )
     child: Name = attr.ib(validator=[attr.validators.instance_of(str), valid_deme_name])
     time: Time = attr.ib(validator=[int_or_float, non_negative, finite])
@@ -734,22 +759,24 @@
         except AssertionError:
             return False
 
 
 @attr.s(auto_attribs=True, kw_only=True, slots=True)
 class Merge:
     """
-    Parameters for a merge event, in which two or more demes end at some time and
+    A merge event, in which two or more demes end at some time and
     contribute to a descendant deme.
 
+    Merge objects are not intended to be constructed directly.
+
     :ivar list[str] parents: A list of parental demes.
     :ivar list[float] proportions: A list of ancestry proportions,
         in order of ``parents``.
     :ivar str child: The descendant deme.
-    :ivar float ~.time: The merge time.
+    :ivar float time: The merge time.
     """
 
     parents: List[Name] = attr.ib(
         validator=attr.validators.deep_iterable(
             member_validator=attr.validators.and_(
                 attr.validators.instance_of(str), valid_deme_name
             ),
@@ -855,22 +882,24 @@
         except AssertionError:
             return False
 
 
 @attr.s(auto_attribs=True, kw_only=True, slots=True)
 class Admix:
     """
-    Parameters for an admixture event, where two or more demes contribute ancestry
+    An admixture event, where two or more demes contribute ancestry
     to a new deme.
 
+    Admix objects are not intended to be constructed directly.
+
     :ivar list[str] parents: A list of source demes.
     :ivar list[float] proportions: A list of ancestry proportions,
         in order of ``parents``.
     :ivar str child: The admixed deme.
-    :ivar float ~.time: The admixture time.
+    :ivar float time: The admixture time.
     """
 
     parents: List[Name] = attr.ib(
         validator=attr.validators.deep_iterable(
             member_validator=attr.validators.and_(
                 attr.validators.instance_of(str), valid_deme_name
             ),
@@ -980,24 +1009,36 @@
 
 
 @attr.s(auto_attribs=True, kw_only=True, slots=True)
 class Deme:
     """
     A collection of individuals that have a common set of population parameters.
 
-    :ivar str name: A concise string that identifies the deme.
-    :ivar str description: A description of the deme.
-    :ivar float start_time: The time at which the deme begins to exist.
-    :ivar list[str] ancestors: List of deme names for the deme's ancestors.
-        This may be ``None``, indicating the deme has no ancestors.
-    :ivar list[float] proportions: If ``ancestors`` is not ``None``,
-        this indicates the proportions of ancestry from each ancestor.
-        This list has the same length as ``ancestors``, and must sum to 1.
-    :ivar list[Epoch] epochs: A list of epochs, which define the population
-        size(s) of the deme. The deme must be created with all epochs listed.
+
+    Deme objects are not intended to be constructed directly.
+
+    :ivar str name:
+        A concise string that identifies the deme.
+    :ivar str description:
+        A description of the deme.
+    :ivar float start_time:
+        The time at which the deme begins to exist.
+    :ivar list[str] ancestors:
+        List of deme names for the deme's ancestors.
+    :ivar list[float] proportions:
+        The proportions of ancestry from each ancestor,
+        ordered to correspond with the same order as the ancestors
+        list.
+        If there are one or more ancestors, the proportions sum to 1.
+    :ivar list[Epoch] epochs:
+        A list of epochs that span the time interval over which the
+        deme exists. Epoch time intervals are non-overlapping,
+        completely cover the deme's existence time interval,
+        and are listed in time-descending order (from the past
+        towards the present).
     """
 
     name: Name = attr.ib(validator=[attr.validators.instance_of(str), valid_deme_name])
     description: str = attr.ib(default="", validator=attr.validators.instance_of(str))
     start_time: Time = attr.ib(validator=[int_or_float, positive])
     ancestors: List[Name] = attr.ib(
         validator=attr.validators.deep_iterable(
@@ -1184,21 +1225,25 @@
         except AssertionError:
             return False
 
     @property
     def end_time(self):
         """
         The end time of the deme's existence.
+
+        :rtype: float
         """
         return self.epochs[-1].end_time
 
     @property
     def time_span(self):
         """
         The time span over which the deme exists.
+
+        :rtype: float
         """
         return self.start_time - self.end_time
 
     def size_at(self, time: float) -> float:
         """
         Get the size of the deme at a given time.
 
@@ -1235,37 +1280,53 @@
             raise NotImplementedError(f"unknown size_function '{epoch.size_function}'")
         return N
 
 
 @attr.s(auto_attribs=True, kw_only=True, slots=True)
 class Graph:
     """
-    The Graph class provides a high-level API for working with a demographic
-    model. A Graph object matches Demes' data model, with a small number of
+    The Graph class is a resolved and validated representation of a
+    demographic model.
+
+    A Graph object matches Demes' :ref:`spec:sec_spec_mdm`, with a small number of
     additional redundant attributes that make the Graph a more convenient
     object to use when inspecting a model's properties.
-
-    :ivar str description: A human readable description of the demography.
-    :ivar str time_units: The units of time used for the demography. This is
+    Graph objects are not intended to be constructed directly---demographic
+    models should instead be :func:`loaded from a YAML document <demes.load>`,
+    or constructed programmatically using the :class:`Builder API <demes.Builder>`.
+
+    A demographic model can be thought of as an acyclic directed graph,
+    where each deme is a vertex and each ancestor/descendant relationship
+    is a directed edge. See the :meth:`predecessors` and :meth:`successors`
+    methods for conversion to the `NetworkX <https://networkx.org/>`_
+    graphical representation.
+
+    :ivar str description:
+        A human readable description of the demography.
+    :ivar str time_units:
+        The units of time used for the demography. This is
         commonly ``years`` or ``generations``, but can be any string.
         This field is intended to be useful for documenting a demography,
         but the actual value provided here should not be relied upon.
-    :ivar float generation_time: The generation time of demes, in units given
+    :ivar float generation_time:
+        The generation time of demes, in units given
         by the ``time_units`` parameter. Concretely, dividing all times
         by ``generation_time`` will convert the graph to have time
-        units in generations.  If ``generation_time`` is ``None``, the units
-        are assumed to be in generations already.
+        units in generations.
         See also: :meth:`.in_generations`.
-    :ivar list[str] doi: If the graph describes a published demography,
-        the DOI(s) should be be given here as a list.
-    :ivar dict metadata: A dictionary of arbitrary additional data.
-    :ivar list[Deme] demes: The demes in the demography.
-    :ivar list[AsymmetricMigration] migrations: The continuous migrations for
-        the demographic model.
-    :ivar list[Pulse] pulses: The migration pulses for the demography.
+    :ivar list[str] doi:
+        A list of publications that describe the demographic model.
+    :ivar dict metadata:
+        A dictionary of arbitrary additional data.
+    :ivar list[Deme] demes:
+        The demes in the demographic model.
+    :ivar list[AsymmetricMigration] migrations:
+        The continuous asymmetric migrations for the demographic model.
+    :ivar list[Pulse] pulses:
+        The instantaneous pulse migrations for the demographic model.
     """
 
     description: str = attr.ib(default="", validator=attr.validators.instance_of(str))
     time_units: str = attr.ib(validator=[attr.validators.instance_of(str), nonzero_len])
     generation_time: Optional[Time] = attr.ib(
         default=None,
         validator=attr.validators.optional([int_or_float, positive, finite]),
@@ -1278,15 +1339,15 @@
             ),
             iterable_validator=attr.validators.instance_of(list),
         ),
     )
     metadata: collections.abc.Mapping = attr.ib(
         factory=dict,
         validator=attr.validators.instance_of(
-            collections.abc.Mapping  # type: ignore[misc]
+            collections.abc.Mapping  # type: ignore[type-abstract]
         ),
     )
     demes: List[Deme] = attr.ib(factory=list, init=False)
     migrations: List[AsymmetricMigration] = attr.ib(factory=list, init=False)
     pulses: List[Pulse] = attr.ib(factory=list, init=False)
 
     # This attribute is for internal use only. It's a (hidden) attribute
@@ -1367,15 +1428,15 @@
         :param float abs_tol: The absolute tolerance permitted for numerical
             comparisons. See documentation for :func:`math.isclose`.
         """
 
         def assert_sorted_eq(aa, bb, *, rel_tol, abs_tol, name):
             # Order-agnostic equality check.
             assert len(aa) == len(bb)
-            for (a, b) in zip(sorted(aa), sorted(bb)):
+            for a, b in zip(sorted(aa), sorted(bb)):
                 try:
                     a.assert_close(b, rel_tol=rel_tol, abs_tol=abs_tol)
                 except AssertionError as e:
                     if isinstance(a, Deme) and isinstance(b, Deme):
                         raise AssertionError(
                             f"Failed for {name} {a.name} and {b.name}"
                         ) from e
@@ -1908,17 +1969,21 @@
                     parent=deme_from,
                     children=list(demes_to),
                     time=self[deme_from].end_time,
                 )
             )
         return demo_events
 
-    def in_generations(self) -> "Graph":
+    def in_generations(self) -> Graph:
         """
         Return a copy of the graph with times in units of generations.
+
+        :return:
+            A demographic model with ``time_units`` in `"generations"`.
+        :rtype: Graph
         """
         graph = copy.deepcopy(self)
         assert graph.generation_time is not None
         for deme in graph.demes:
             deme.start_time /= graph.generation_time
             for epoch in deme.epochs:
                 epoch.start_time /= graph.generation_time
@@ -1928,18 +1993,57 @@
             migration.end_time /= graph.generation_time
         for pulse in graph.pulses:
             pulse.time /= graph.generation_time
         graph.time_units = "generations"
         graph.generation_time = 1
         return graph
 
+    def rename_demes(self, names: Mapping[str, str]) -> Graph:
+        """
+        Rename demes according to a dictionary that may contain a partial set of demes.
+
+        :param dict names:
+            A dictionary with deme names and new names.
+        :return:
+            A demographic model with renamed demes.
+        :rtype: Graph
+        """
+        if not isinstance(names, Mapping):
+            raise TypeError("names is not a dictionary")
+        graph = copy.deepcopy(self)
+        for deme in graph.demes:
+            if deme.name in names:
+                deme.name = names[deme.name]
+            deme.ancestors = [names[a] if a in names else a for a in deme.ancestors]
+        for migration in graph.migrations:
+            if migration.source in names:
+                migration.source = names[migration.source]
+            if migration.dest in names:
+                migration.dest = names[migration.dest]
+        for pulse in graph.pulses:
+            pulse.sources = [names[s] if s in names else s for s in pulse.sources]
+            if pulse.dest in names:
+                pulse.dest = names[pulse.dest]
+        for k, deme in list(graph._deme_map.items()):
+            if k in names:
+                del graph._deme_map[k]
+                graph._deme_map[names[k]] = deme
+        return graph
+
     @classmethod
-    def fromdict(cls, data: MutableMapping[str, Any]) -> "Graph":
+    def fromdict(cls, data: MutableMapping[str, Any]) -> Graph:
         """
-        Return a graph from a dict representation. The inverse of :meth:`.asdict`.
+        Return a graph from a data dictionary.
+
+        :param dict data:
+            A data dictionary following either the
+            :ref:`spec:sec_spec_hdm` or the :ref:`spec:sec_spec_mdm`.
+        :return:
+            A resolved and validated demographic model.
+        :rtype: Graph
         """
         if not isinstance(data, MutableMapping):
             raise TypeError("data is not a dictionary")
 
         # Don't modify the input data dict.
         data = copy.deepcopy(data)
 
@@ -2249,46 +2353,60 @@
         graph.pulses.sort(key=lambda pulse: pulse.time, reverse=True)
 
         return graph
 
     def asdict(self, keep_empty_fields=True) -> MutableMapping[str, Any]:
         """
         Return a fully-resolved dict representation of the graph.
+
+        :return:
+            A data dictionary following the :ref:`spec:sec_spec_mdm`.
+        :rtype: dict
         """
 
         def filt(attrib, value):
             return (
                 keep_empty_fields
                 or (not (hasattr(value, "__len__") and len(value) == 0))
             ) and attrib.name != "_deme_map"
 
-        def coerce_numbers(inst, attribute, value):
-            # Explicitly convert numeric types to int or float, so that they
+        def coerce_types(inst, attribute, value):
+            # Explicitly convert numeric and string types, so that they
             # don't cause problems for the YAML and JSON serialisers.
-            # E.g. numpy int32/int64 are part of Python's numeric tower as
+            # Numpy int32/int64 are part of Python's numeric tower as
             # subclasses of numbers.Integral, similarly numpy's float32/float64
             # are subclasses of numbers.Real. There are yet other numeric types,
             # such as the standard library's decimal.Decimal, which are not part
             # of the numeric tower, but provide a __float__() method.
-            if isinstance(value, numbers.Integral):
+            # Likewise, string subclasses such as numpy.str_ aren't recognised
+            # by the YAML serialiser, so we explicitly convert them to str.
+            # We check for 'str' first, because numpy.str_ also has a
+            # __float__() method.
+            if isinstance(value, str):
+                value = str(value)
+            elif isinstance(value, numbers.Integral):
                 value = int(value)
             elif isinstance(value, numbers.Real) or hasattr(value, "__float__"):
                 value = float(value)
             return value
 
-        data = attr.asdict(self, filter=filt, value_serializer=coerce_numbers)
+        data = attr.asdict(self, filter=filt, value_serializer=coerce_types)
         # translate to spec data model
         for deme in data["demes"]:
             for epoch in deme["epochs"]:
                 del epoch["start_time"]
         return data
 
     def asdict_simplified(self) -> MutableMapping[str, Any]:
         """
         Return a simplified dict representation of the graph.
+
+        :return:
+            A data dictionary following the :ref:`spec:sec_spec_hdm`.
+        :rtype: dict
         """
 
         def simplify_epochs(data):
             """
             Remove epoch start times. Also remove deme start time
             if implied by the deme ancestor(s)'s end time(s).
             """
@@ -2413,52 +2531,61 @@
         simplify_epochs(data)
 
         return data
 
 
 class Builder:
     """
-    The Builder provides a set of convenient methods for incrementally
-    constructing a deme graph. The state of the graph is stored internally as a
-    dictionary of objects following Demes' data model, and may be converted
-    into a fully-resolved :class:`Graph` object using the :meth:`.resolve()` method.
-
-    :ivar dict data: The data dictionary of the graph's current state.
-        The objects nested within this dictionary follow Demes' data model,
-        as described in the :ref:`spec:sec_spec`.
+    The Builder class provides a set of convenient methods for
+    incrementally constructing a demographic model.
+
+    The state of the demographic model is stored internally as a dictionary
+    of objects following Demes' :ref:`spec:sec_spec_hdm`.
+    The content of this dictionary is *not* resolved and is *not* verified.
+    The Builder object may be converted into a resolved and validated
+    :class:`Graph` object using the :meth:`.resolve()` method.
+
+    :ivar dict data:
+        The data dictionary of the demographic model's current state.
+        The objects nested within this dictionary should follow
+        Demes' data model, as described in the :ref:`spec:sec_spec_hdm` schema.
 
         .. note::
-            Users may freely modify the data dictionary, as long as the data
-            model is not violated.
+            Users may freely modify the data dictionary, such as temporarily
+            adding or deleting fields, as long as the :ref:`spec:sec_spec_hdm`
+            is not violated when the :meth:`.resolve` method is called.
     """
 
     def __init__(
         self,
         *,
-        description: str = None,
+        description: str | None = None,
         time_units: str = "generations",
-        generation_time: float = None,
-        doi: list = None,
-        defaults: dict = None,
-        metadata: dict = None,
+        generation_time: float | None = None,
+        doi: list | None = None,
+        defaults: dict | None = None,
+        metadata: dict | None = None,
     ):
         """
-        :param str description: A human readable description of the demography.
-            May be ``None``.
-        :param str time_units: The units of time used for the demography. This is
+        :param str description:
+            A human readable description of the demography.
+        :param str time_units:
+            The units of time used for the demography. This is
             commonly ``years`` or ``generations``, but can be any string.
-        :param float generation_time: The generation time of demes, in units given
-            by the ``time_units`` parameter. Concretely, dividing all times
-            by ``generation_time`` will convert the graph to have time
-            units in generations.  If ``generation_time`` is ``None``, the units
-            are assumed to be in generations already.
-        :param doi: If the graph describes a published demography, the DOI(s)
+        :param float generation_time:
+            The generation time of demes, in units given
+            by the ``time_units`` parameter.
+        :param list[str] doi:
+            If the graph describes a published demography, the DOI(s)
             should be be given here as a list.
-        :type doi: list[str]
-        :param dict metadata: A dictionary of arbitrary additional data.
+        :param dict defaults:
+            A dictionary of default values, following the
+            :ref:`spec:sec_spec_hdm` schema for defaults.
+        :param dict metadata:
+            A dictionary of arbitrary additional data.
         """
         self.data: MutableMapping[str, Any] = dict(time_units=time_units)
         if description is not None:
             self.data["description"] = description
         if generation_time is not None:
             self.data["generation_time"] = generation_time
         if doi is not None:
@@ -2468,34 +2595,40 @@
         if metadata is not None:
             self.data["metadata"] = metadata
 
     def add_deme(
         self,
         name: str,
         *,
-        description: str = None,
-        ancestors: list = None,
-        proportions: list = None,
-        start_time: float = None,
-        epochs: list = None,
-        defaults: dict = None,
+        description: str | None = None,
+        ancestors: list | None = None,
+        proportions: list | None = None,
+        start_time: float | None = None,
+        epochs: list | None = None,
+        defaults: dict | None = None,
     ):
         """
-        Add a deme. Ancestor demes must be added before their children.
+        Append a deme to the "demes" list field of the data dictionary.
+
+        If the data dictionary doesn't contain the "demes" field,
+        it will be added.
 
         :param str name: A string identifier for the deme.
-        :param str description: A description of the deme. May be ``None``.
+        :param str description: A description of the deme.
         :param list[str] ancestors: List of deme names for the deme's ancestors.
-            This may be ``None``, indicating the deme has no ancestors.
-        :param list[float] proportions: If ``ancestors`` is not ``None``,
-            this indicates the proportions of ancestry from each ancestor.
+        :param list[float] proportions:
+            The proportions of ancestry from each ancestor.
             This list has the same length as ``ancestors``, and must sum to 1.
         :param float start_time: The deme's start time.
-        :param list[dict] epochs: List of epoch dictionaries. Each dictionary
-            follows the data model for an epoch.
+        :param list[dict] epochs:
+            List of epoch dictionaries. Each dictionary
+            follows the :ref:`spec:sec_spec_hdm` schema for an epoch object.
+        :param dict defaults:
+            A dictionary of default deme values, following the
+            :ref:`spec:sec_spec_hdm` schema for deme defaults.
         """
         deme: MutableMapping[str, Any] = dict(name=name)
         if description is not None:
             deme["description"] = description
         if ancestors is not None:
             deme["ancestors"] = ancestors
         if proportions is not None:
@@ -2512,44 +2645,54 @@
         if "demes" not in self.data:
             self.data["demes"] = []
         self.data["demes"].append(deme)
 
     def add_migration(
         self,
         *,
-        rate: float = None,
+        rate: float | None = None,
         # We use a special NO_DEFAULT value here, to distinguish between the user
         # not specifying anything, and specifying the value None (which may be
         # necessary to override a 'defaults' value set in the data dictionary).
         demes: list = NO_DEFAULT,  # type: ignore
         source: str = NO_DEFAULT,  # type: ignore
         dest: str = NO_DEFAULT,  # type: ignore
-        start_time: float = None,
-        end_time: float = None,
+        start_time: float | None = None,
+        end_time: float | None = None,
     ):
         """
-        Add continuous symmetric migrations between all pairs of demes in a list,
-        or alternately, add asymmetric migration from one deme to another.
-        Source and destination demes follow the forwards-in-time convention,
-        so that the migration rate refers to the movement of individuals from
-        the ``source`` deme to the ``dest`` deme.
+        Append a period of continuous migration to the "migrations" list field
+        of the data dictionary.
 
-        :param list[str] demes: list of deme names. Migration is symmetric
-            between all pairs of demes in this list. If not specified,
-            migration will be asymmetric (and ``source`` and ``dest`` must
-            be given).
-        :param str source: The name of the source deme.
-        :param str dest: The name of the destination deme.
-        :param float rate: The rate of migration per generation.
-        :param float start_time: The time at which the migration rate is enabled.
-            If ``None``, the start time is defined by the earliest time at
-            which the demes coexist.
-        :param float end_time: The time at which the migration rate is disabled.
-            If ``None``, the end time is defined by the latest time at which
-            the demes coexist.
+        If the data dictionary doesn't contain the "migrations" field,
+        it will be added.
+        Continuous migrations may be either symmetric or asymmetric.
+        For symmetric migrations, a list of deme names must be provided in the
+        ``demes`` field, and the ``source`` and ``dest`` fields must not
+        be used.
+        For asymmetric migrations, the ``source`` and ``dest`` fields must
+        be provided and the ``demes`` field must not be used.
+        Source and destination demes refer to individuals migrating
+        forwards in time.
+
+        :param list[str] demes:
+            List of deme names. If specified, migration is symmetric
+            between all pairs of demes in this list.
+        :param str source:
+            The name of the source deme. If specified, migration is asymmetric
+            from this deme.
+        :param str dest:
+            The name of the destination deme. If specified, migration is
+            asymmetric into this deme.
+        :param float rate:
+            The rate of migration per generation.
+        :param float start_time:
+            The time at which the migration rate is enabled.
+        :param float end_time:
+            The time at which the migration rate is disabled.
         """
         migration: MutableMapping[str, Any] = dict()
         if rate is not None:
             migration["rate"] = rate
         if demes is not NO_DEFAULT:
             migration["demes"] = demes
         if source is not NO_DEFAULT:
@@ -2566,29 +2709,38 @@
         if "migrations" not in self.data:
             self.data["migrations"] = []
         self.data["migrations"].append(migration)
 
     def add_pulse(
         self,
         *,
-        sources: List[str] = None,
-        dest: str = None,
-        proportions: List[float] = None,
-        time: float = None,
+        sources: List[str] | None = None,
+        dest: str | None = None,
+        proportions: List[float] | None = None,
+        time: float | None = None,
     ):
         """
-        Add a pulse of migration at a fixed time.
-        Source and destination demes follow the forwards-in-time convention.
+        Append a pulse of migration at a fixed time to the "pulses" list
+        field of the data dictionary.
 
-        :param list(str) source: The name of the source deme(s).
-        :param str dest: The name of the destination deme.
-        :param list(float) proportion: At the instant after migration, this is the
-            expected proportion(s) of individuals in the destination deme made up
+        If the data dictionary doesn't contain the "pulses" field,
+        it will be added.
+        Source and destination demes refer to individuals migrating
+        forwards in time.
+
+        :param list(str) sources:
+            A list of names of the source deme(s).
+        :param str dest:
+            The name of the destination deme.
+        :param list(float) proportion:
+            At the instant after migration, this is the expected proportion(s)
+            of individuals in the destination deme made up
             of individuals from the source deme(s).
-        :param float time: The time at which migrations occur.
+        :param float time:
+            The time at which migrations occur.
         """
         pulse: MutableMapping[str, Any] = dict()
         if sources is not None:
             pulse["sources"] = sources
         if dest is not None:
             pulse["dest"] = dest
         if proportions is not None:
@@ -2598,29 +2750,31 @@
 
         if "pulses" not in self.data:
             self.data["pulses"] = []
         self.data["pulses"].append(pulse)
 
     def resolve(self):
         """
-        Resolve the data dictionary into a Graph.
+        Resolve the Builder's data dictionary into a Graph.
 
         :return: The fully-resolved Graph.
         :rtype: Graph
         """
         return Graph.fromdict(self.data)
 
     @classmethod
     def fromdict(cls, data: MutableMapping[str, Any]) -> "Builder":
         """
         Make a Builder object from an existing data dictionary.
 
-        :param MutableMapping data: The data dictionary to initialise the
-            graph's state. The objects nested within this dictionary must
-            follow Demes' data model, as described in the :ref:`spec:sec_spec`.
+        :param MutableMapping data:
+            The data dictionary to initialise the Builder's state.
+            The objects nested within this dictionary should follow
+            Demes' :ref:`spec:sec_spec_hdm`, but see the note for
+            :attr:`.Builder.data`.
 
         :return: The new Builder object.
         :rtype: Builder
         """
         builder = cls()
         builder.data = data
         return builder
```

### Comparing `demes-0.2.2/demes/load_dump.py` & `demes-0.2.3/demes/load_dump.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Functions to load and dump graphs in YAML and JSON formats.
 """
+from __future__ import annotations
 import contextlib
 import json
 import io
 import math
 from typing import Any, Generator, MutableMapping
 
 import ruamel.yaml
@@ -142,32 +143,38 @@
     data_no_metadata = {k: v for k, v in data.items() if k != "metadata"}
     assert_no_nulls(data_no_metadata)
 
 
 def loads_asdict(string, *, format="yaml") -> MutableMapping[str, Any]:
     """
     Load a YAML or JSON string into a dictionary of nested objects.
-    The keywords and structure of the input are defined by the
-    :ref:`spec:sec_spec`.
+
+    The input is *not* resolved, and is *not* validated.
+    The returned object may be converted into a :class:`Builder`
+    using :meth:`Builder.fromdict` or converted into a :class:`Graph`
+    using :meth:`Graph.fromdict`.
 
     :param str string: The string to be loaded.
     :param str format: The format of the input string. Either "yaml" or "json".
     :return: A dictionary of nested objects, with the same data model as the
         YAML or JSON input string.
     :rtype: dict
     """
     with io.StringIO(string) as stream:
         return load_asdict(stream, format=format)
 
 
 def load_asdict(filename, *, format="yaml") -> MutableMapping[str, Any]:
     """
     Load a YAML or JSON file into a dictionary of nested objects.
-    The keywords and structure of the input are defined by the
-    :ref:`spec:sec_spec`.
+
+    The input is *not* resolved, and is *not* validated.
+    The returned object may be converted into a :class:`Builder`
+    using :meth:`Builder.fromdict` or converted into a :class:`Graph`
+    using :meth:`Graph.fromdict`.
 
     :param filename: The path to the file to be loaded, or a file-like object
         with a ``read()`` method.
     :type filename: Union[str, os.PathLike, FileLike]
     :param str format: The format of the input file. Either "yaml" or "json".
     :return: A dictionary of nested objects, with the same data model as the
         YAML or JSON input.
@@ -187,57 +194,57 @@
     # The string "Infinity" should only be present in JSON files.
     # But YAML is a superset of JSON, so we want the YAML loader to also
     # load JSON files without problem.
     _unstringify_infinities(data)
     return data
 
 
-def loads(string, *, format="yaml") -> "demes.Graph":
+def loads(string, *, format="yaml") -> demes.Graph:
     """
     Load a graph from a YAML or JSON string.
     The keywords and structure of the input are defined by the
     :ref:`spec:sec_spec`.
 
     :param str string: The string to be loaded.
     :param str format: The format of the input string. Either "yaml" or "json".
-    :return: A graph.
-    :rtype: .Graph
+    :return: A resolved and validated demographic model.
+    :rtype: demes.Graph
     """
     data = loads_asdict(string, format=format)
     return demes.Graph.fromdict(data)
 
 
-def load(filename, *, format="yaml") -> "demes.Graph":
+def load(filename, *, format="yaml") -> demes.Graph:
     """
     Load a graph from a YAML or JSON file.
     The keywords and structure of the input are defined by the
     :ref:`spec:sec_spec`.
 
     :param filename: The path to the file to be loaded, or a file-like object
         with a ``read()`` method.
     :type filename: Union[str, os.PathLike, FileLike]
     :param str format: The format of the input file. Either "yaml" or "json".
-    :return: A graph.
-    :rtype: .Graph
+    :return: A resolved and validated demographic model.
+    :rtype: demes.Graph
     """
     data = load_asdict(filename, format=format)
     return demes.Graph.fromdict(data)
 
 
-def load_all(filename) -> Generator["demes.Graph", None, None]:
+def load_all(filename) -> Generator[demes.Graph, None, None]:
     """
     Generate graphs from a YAML document stream. Documents must be separated by
     the YAML document start indicator, ``---``.
     The keywords and structure of each document are defined by the
     :ref:`spec:sec_spec`.
 
     :param filename: The path to the file to be loaded, or a file-like object
         with a ``read()`` method.
     :type filename: Union[str, os.PathLike, FileLike]
-    :return: A generator of graphs.
+    :return: A generator of resolved and validated demographic models.
     :rtype: Generator[demes.Graph, None, None]
     """
     with _open_file_polymorph(filename) as f:
         with ruamel.yaml.YAML(typ="safe") as yaml:
             for data in yaml.load_all(f):
                 # We forbid null values in the input data.
                 # See https://github.com/popsim-consortium/demes-spec/issues/76
@@ -251,18 +258,21 @@
 
 def dumps(graph, *, format="yaml", simplified=True) -> str:
     """
     Dump the specified graph to a YAML or JSON string.
     The keywords and structure of the output are defined by the
     :ref:`spec:sec_spec`.
 
-    :param .Graph graph: The graph to dump.
+    :param demes.Graph graph: The graph to dump.
     :param str format: The format of the output file. Either "yaml" or "json".
-    :param bool simplified: If True, returns a simplified graph. If False, returns
-        a fully-qualified graph.
+    :param bool simplified:
+        If True, returns a string following the :ref:`spec:sec_spec_hdm`,
+        which has many fields omitted and is thus more compact.
+        If False, returns a string that is fully-resolved following the
+        :ref:`spec:sec_spec_mdm`.
     :return: The YAML or JSON string.
     :rtype: str
     """
     with io.StringIO() as stream:
         dump(graph, stream, format=format, simplified=simplified)
         string = stream.getvalue()
     return string
@@ -270,21 +280,24 @@
 
 def dump(graph, filename, *, format="yaml", simplified=True) -> None:
     """
     Dump the specified graph to a file.
     The keywords and structure of the output are defined by the
     :ref:`spec:sec_spec`.
 
-    :param .Graph graph: The graph to dump.
+    :param demes.Graph graph: The graph to dump.
     :param filename: Path to the output file, or a file-like object with a
         ``write()`` method.
     :type filename: Union[str, os.PathLike, FileLike]
     :param str format: The format of the output file. Either "yaml" or "json".
-    :param bool simplified: If True, outputs a simplified graph. If False, outputs
-        a fully-qualified graph.
+    :param bool simplified:
+        If True, the output file follows the :ref:`spec:sec_spec_hdm`,
+        which has many fields omitted and is thus more compact.
+        If False, the output file is fully-resolved and follows the
+        :ref:`spec:sec_spec_mdm`.
     """
     if simplified:
         data = graph.asdict_simplified()
     else:
         data = graph.asdict()
 
     if format == "json":
@@ -302,16 +315,19 @@
     """
     Dump the specified graphs to a multi-document YAML file or output stream.
 
     :param graphs: An iterable of graphs to dump.
     :param filename: Path to the output file, or a file-like object with a
         ``write()`` method.
     :type filename: Union[str, os.PathLike, FileLike]
-    :param bool simplified: If True, outputs simplified graphs. If False, outputs
-        fully-qualified graphs.
+    :param bool simplified:
+        If True, the output file follows the :ref:`spec:sec_spec_hdm`,
+        which has many fields omitted and is thus more compact.
+        If False, the output file is fully-resolved and follows the
+        :ref:`spec:sec_spec_mdm`.
     """
     with _open_file_polymorph(filename, "w") as f:
         for graph in graphs:
             if simplified:
                 data = graph.asdict_simplified()
             else:
                 data = graph.asdict()
```

### Comparing `demes-0.2.2/demes/ms.py` & `demes-0.2.3/demes/ms.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 import copy
 import math
 import argparse
 import logging
 import sys
 import operator
 import itertools
@@ -818,53 +819,60 @@
 
     graph = b.resolve()
     return graph
 
 
 def remap_deme_names(graph: demes.Graph, names: Mapping[str, str]) -> demes.Graph:
     assert sorted(names.keys()) == sorted(deme.name for deme in graph.demes)
-    graph = copy.deepcopy(graph)
-    for deme in graph.demes:
-        deme.name = names[deme.name]
-        deme.ancestors = [names[ancestor] for ancestor in deme.ancestors]
-    for migration in graph.migrations:
-        migration.source = names[migration.source]
-        migration.dest = names[migration.dest]
-    for pulse in graph.pulses:
-        pulse.sources = [names[s] for s in pulse.sources]
-        pulse.dest = names[pulse.dest]
-    for k, deme in list(graph._deme_map.items()):
-        del graph._deme_map[k]
-        graph._deme_map[names[k]] = deme
+    graph = graph.rename_demes(names)
     return graph
 
 
 def from_ms(
     command: str,
     *,
     N0: float,
-    deme_names: List[str] = None,
+    deme_names: List[str] | None = None,
 ) -> demes.Graph:
     """
     Convert an ms demographic model into a demes graph.
 
     `Hudson's ms <https://doi.org/10.1093/bioinformatics/18.2.337>`_
     uses coalescent units for times (:math:`t`),
     population sizes (:math:`x`), and migration rates (:math:`M`).
     These will be converted to more familiar units using the given
     ``N0`` value (:math:`N_0`) according to the following rules:
 
     .. math::
 
         \\text{time (in generations)} &= 4 N_0 t
 
-        \\text{deme size (haploid individuals)} &= N_0 x
+        \\text{deme size (diploid individuals)} &= N_0 x
 
         \\text{migration rate (per generation)} &= \\frac{M}{4 N_0}
 
+    .. seealso::
+        The :ref:`sec_cli_ms` command line interface.
+
+    .. warning::
+
+        Several programs exist that implement an ms or ms-like
+        command line interface. But discrepancies do exist
+        between ms and its clones for some command line arguments,
+        and such discrepancies alter the interpretation of the
+        demographic model.
+        This function implements the behaviour as described in
+        Hudson's ms manual. Command lines constructed for use with
+        other programs may work as desired, but users are cautioned to
+        carefully check the appropriate documentation to identify where
+        discrepancies may exist.
+
+        The ms manual may be obtained from
+        http://home.uchicago.edu/~rhudson1/source/mksamples.html
+
     :param str command: The ms command line.
     :param float N0:
         The reference population size (:math:`N_0`) used to translate
         from coalescent units. For a ``command`` that specifies a
         :math:`\\theta` value with the ``-t theta`` option,
         this can be calculated as :math:`N_0 = \\theta / (4 \\mu L)`,
         where :math:`\\mu` is the per-generation mutation rate and
@@ -895,22 +903,27 @@
 
 def to_ms(graph: demes.Graph, *, N0, samples=None) -> str:
     """
     Get ms command line arguments for the graph.
 
     The order of deme IDs matches the order of demes in the graph.
 
+    .. seealso::
+        The ``--ms`` option of the :ref:`sec_cli_parse` command line interface.
+
     :param float N0:
         The reference population size used to translate into coalescent units.
         See :func:`from_ms` for details.
     :param list(int) samples:
-        Sampling scheme that will be used with the '-I' option. This is ignored
-        for graphs with only one deme. If not specified, the sampling
-        configuration in the returned string will need editing prior to
-        simulation.
+        A list of haploid sample numbers, one for each deme, in the same
+        order as the order of demes in the graph.
+        The parameter is ignored for demographic models with only one deme.
+        The given sampling scheme will be used with the ``-I`` argument.
+        If not specified, the sampling configuration in the returned string
+        will need editing prior to use.
     :return: The ms command line.
     :rtype: str
     """
     graph = graph.in_generations()
     cmd = []
     num_demes = len(graph.demes)
     if samples is not None and len(samples) != num_demes:
```

### Comparing `demes-0.2.2/demes.egg-info/PKG-INFO` & `demes-0.2.3/demes.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,22 @@
 Metadata-Version: 2.1
 Name: demes
-Version: 0.2.2
+Version: 0.2.3
 Summary: tools for describing demographic models
 Home-page: https://github.com/popsim-consortium/demes-python
 Author: PopSim Consortium
 License: ISC
 Project-URL: Documentation, https://popsim-consortium.github.io/demes-docs/
 Project-URL: Source Code, https://github.com/popsim-consortium/demes-python/
 Project-URL: Bug Tracker, https://github.com/popsim-consortium/demes-python/issues
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Tools for describing and manipulating demographic models.
@@ -38,9 +33,7 @@
 - A simple declarative high-level format for specifying demographic models. This format is
   intended to be human-readable and to make it easy to correctly specify models.
 - A corresponding low-level format that is an entirely unambiguous and portable description
   of a model, which can be used by many different simulation frameworks as input. Thus,
   we can see part of the role of this package as *compiling* the high-level description of
   a model into the corresponding low-level description.
 - Robust validation of models and reporting of errors for invalid models.
-
-
```

### Comparing `demes-0.2.2/demes.egg-info/SOURCES.txt` & `demes-0.2.3/demes.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 .gitignore
 .gitmodules
 .pre-commit-config.yaml
 CHANGELOG.md
+CITATION.md
 LICENSE
 README.md
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 verification.py
@@ -27,27 +28,30 @@
 demes.egg-info/SOURCES.txt
 demes.egg-info/dependency_links.txt
 demes.egg-info/entry_points.txt
 demes.egg-info/not-zip-safe
 demes.egg-info/requires.txt
 demes.egg-info/top_level.txt
 docs/CHANGELOG.md
+docs/CITATION.md
 docs/Makefile
 docs/_config.yml
 docs/_toc.yml
 docs/api.md
 docs/build.sh
 docs/cli.md
 docs/convert_changelog.py
 docs/development.md
+docs/index.md
 docs/installation.md
 docs/introduction.md
 docs/is_new_stable.py
 docs/quickstart.md
 docs/release.md
+docs/_static/custom.css
 examples/bottleneck.yaml
 examples/browning_america.yaml
 examples/cloning_example.yaml
 examples/gutenkunst_ooa.yaml
 examples/jacobs_papuans.yaml
 examples/linear_size_function_example.yaml
 examples/offshoots.yaml
```

### Comparing `demes-0.2.2/docs/CHANGELOG.md` & `demes-0.2.3/docs/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Changelog
 
+## 0.2.3 - 2023-05-04
+
+- Fixed the use of numpy strings for deme names.
+  ({user}`terhorst`, {user}`grahamgower`, {issue}`495`, {pr}`505`)
+- Added `Graph.rename_demes()` method to return a graph with renamed demes.
+  ({user}`aabiddanda`, {pr}`499`)
+
 ## 0.2.2 - 2022-04-28
 
 Better conformance to the spec. Minor discrepancies between
 demes-python and the reference implementation have been resolved.
 
 - Dropped support for Python 3.6
   ({user}`grahamgower`, {issue}`445`, {pr}`446`)
```

### Comparing `demes-0.2.2/docs/api.md` & `demes-0.2.3/docs/api.md`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 .. autofunction:: demes.dump_all
 ```
 
 ## Building Demes graphs
 
 ```{eval-rst}
 .. autoclass:: demes.Builder
-   :members:
+    :members:
+
+    .. automethod:: __init__
 ```
 
 ## Working with Demes graphs
 
 ```{eval-rst}
 .. autoclass:: demes.Graph
     :members:
```

### Comparing `demes-0.2.2/docs/convert_changelog.py` & `demes-0.2.3/docs/convert_changelog.py`

 * *Files identical despite different names*

### Comparing `demes-0.2.2/docs/development.md` & `demes-0.2.3/docs/development.md`

 * *Files identical despite different names*

### Comparing `demes-0.2.2/docs/introduction.md` & `demes-0.2.3/docs/introduction.md`

 * *Files 6% similar despite different names*

```diff
@@ -65,9 +65,9 @@
 the [`demesdraw`](https://github.com/grahamgower/demesdraw) Python package.
 
 ```{code-cell}
 import demes
 import demesdraw
 
 graph = demes.load("../examples/two_epoch.yaml")
-demesdraw.tubes(graph, inf_ratio=0.4);
+demesdraw.tubes(graph)
 ```
```

### Comparing `demes-0.2.2/docs/is_new_stable.py` & `demes-0.2.3/docs/is_new_stable.py`

 * *Files identical despite different names*

### Comparing `demes-0.2.2/docs/quickstart.md` & `demes-0.2.3/docs/quickstart.md`

 * *Files 3% similar despite different names*

```diff
@@ -36,23 +36,22 @@
 
 ooa_graph = demes.load("../examples/gutenkunst_ooa.yaml")
 fig, ax = demesdraw.utils.get_fig_axes(aspect=0.8, scale=1.5)
 demesdraw.tubes(ooa_graph, ax=ax, log_time=True)
 glue("demesdraw_gutenkunst_ooa", fig, display=False)
 ```
 
-`````{panels}
-:column: container
-````{tabbed} YAML
+`````{tab-set}
+````{tab-item} YAML
 :class-label: pt-0
 ```{literalinclude} ../examples/gutenkunst_ooa.yaml
 :language: yaml
 ```
 ````
-````{tabbed} Drawing
+````{tab-item} Drawing
 :class-label: pt-0
 ```{glue:} demesdraw_gutenkunst_ooa
 ```
 ````
 `````
 
 This YAML file can be loaded into Python with the {func}`.load` function,
@@ -160,18 +159,15 @@
 The external [`demesdraw`](https://github.com/grahamgower/demesdraw)
 library offers a way to visualise {class}`.Graph` objects, which can be
 a useful way to check that the model is what we expect.
 
 ```{code-cell}
 import demesdraw
 
-w = 2.0 * demesdraw.utils.size_max(ring_graph)
-# Manually set x-axis coordinates for each deme, to improve spacing.
-positions = {deme.name: j * w for j, deme in enumerate(ring_graph.demes)}
-demesdraw.tubes(ring_graph, positions=positions);
+demesdraw.tubes(ring_graph)
 ```
 
 ## Saving a Demes graph
 
 The graph can be written out to a new YAML file using the {func}`.dump` function.
 
 ```{code-cell}
```

### Comparing `demes-0.2.2/docs/release.md` & `demes-0.2.3/docs/release.md`

 * *Files identical despite different names*

### Comparing `demes-0.2.2/examples/browning_america.yaml` & `demes-0.2.3/examples/browning_america.yaml`

 * *Files identical despite different names*

### Comparing `demes-0.2.2/examples/cloning_example.yaml` & `demes-0.2.3/examples/cloning_example.yaml`

 * *Files identical despite different names*

### Comparing `demes-0.2.2/examples/gutenkunst_ooa.yaml` & `demes-0.2.3/examples/gutenkunst_ooa.yaml`

 * *Files identical despite different names*

### Comparing `demes-0.2.2/examples/jacobs_papuans.yaml` & `demes-0.2.3/examples/jacobs_papuans.yaml`

 * *Files identical despite different names*

### Comparing `demes-0.2.2/examples/linear_size_function_example.yaml` & `demes-0.2.3/examples/linear_size_function_example.yaml`

 * *Files identical despite different names*

### Comparing `demes-0.2.2/examples/offshoots.yaml` & `demes-0.2.3/examples/offshoots.yaml`

 * *Files identical despite different names*

### Comparing `demes-0.2.2/examples/selfing_example.yaml` & `demes-0.2.3/examples/selfing_example.yaml`

 * *Files identical despite different names*

### Comparing `demes-0.2.2/examples/zigzag.yaml` & `demes-0.2.3/examples/zigzag.yaml`

 * *Files identical despite different names*

### Comparing `demes-0.2.2/setup.cfg` & `demes-0.2.3/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -8,18 +8,14 @@
 url = https://github.com/popsim-consortium/demes-python
 classifiers = 
 	Development Status :: 4 - Beta
 	License :: OSI Approved :: ISC License (ISCL)
 	Operating System :: OS Independent
 	Intended Audience :: Science/Research
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
-	Programming Language :: Python :: 3.8
-	Programming Language :: Python :: 3.9
-	Programming Language :: Python :: 3.10
 	Topic :: Scientific/Engineering
 	Topic :: Scientific/Engineering :: Bio-Informatics
 project_urls = 
 	Documentation = https://popsim-consortium.github.io/demes-docs/
 	Source Code = https://github.com/popsim-consortium/demes-python/
 	Bug Tracker = https://github.com/popsim-consortium/demes-python/issues
 
@@ -46,15 +42,15 @@
 per-file-ignores = 
 	tests/test_import_visibility.py:F403,F405
 
 [mypy]
 files = demes, tests
 warn_unused_ignores = True
 show_error_codes = True
-python_version = 3.7
+python_version = 3.8
 
 [mypy-numpy.*]
 ignore_missing_imports = True
 
 [mypy-ruamel.*]
 ignore_missing_imports = True
```

### Comparing `demes-0.2.2/tests/__init__.py` & `demes-0.2.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `demes-0.2.2/tests/ms_asymmetric_migration.sh` & `demes-0.2.3/tests/ms_asymmetric_migration.sh`

 * *Files identical despite different names*

### Comparing `demes-0.2.2/tests/test_cli.py` & `demes-0.2.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `demes-0.2.2/tests/test_demes.py` & `demes-0.2.3/tests/test_demes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1873,14 +1873,63 @@
         # so it doesn't make sense to set generation_time != 1 when time units
         # are generations.
         b = Builder(time_units="generations", generation_time=13)
         b.add_deme("A", epochs=[dict(start_size=1, end_time=0)])
         with pytest.raises(ValueError, match="generation_time!=1"):
             b.resolve()
 
+    @pytest.mark.parametrize("graph", tests.example_graphs())
+    def test_bad_rename_demes(self, graph):
+        rev_graph = graph.rename_demes(names={})
+        graph.assert_close(rev_graph)
+        for b in [[], set(), "X", 1, 1.0]:
+            with pytest.raises(TypeError, match="names is not a dictionary"):
+                graph.rename_demes(names=b)
+
+    @pytest.mark.parametrize("graph", tests.example_graphs())
+    def test_rename_all_demes(self, graph):
+        name_dict = {d.name: f"{d.name}X" for d in graph.demes}
+        rev_graph = graph.rename_demes(names=name_dict)
+        for deme in rev_graph.demes:
+            assert (deme.name not in name_dict) and (deme.name in name_dict.values())
+            for ancestor in deme.ancestors:
+                assert (ancestor not in name_dict) and (ancestor in name_dict.values())
+        for migration in rev_graph.migrations:
+            assert (migration.source not in name_dict) and (
+                migration.source in name_dict.values()
+            )
+            assert (migration.dest not in name_dict) and (
+                migration.dest in name_dict.values()
+            )
+        for pulse in rev_graph.pulses:
+            for s in pulse.sources:
+                assert (s not in name_dict) and (s in name_dict.values())
+            assert pulse.dest not in name_dict
+            assert pulse.dest in name_dict.values()
+
+    @pytest.mark.parametrize("graph", tests.example_graphs())
+    def test_rename_single_deme(self, graph):
+        name_dict_small = {graph.demes[0].name: f"{graph.demes[0].name}Y"}
+        rev_graph = graph.rename_demes(names=name_dict_small)
+        rename_cnt = 0
+        for deme in rev_graph.demes:
+            assert deme.name not in name_dict_small
+            if deme.name in name_dict_small.values():
+                rename_cnt += 1
+            for ancestor in deme.ancestors:
+                assert ancestor not in name_dict_small
+        for migration in rev_graph.migrations:
+            assert migration.source not in name_dict_small
+            assert migration.dest not in name_dict_small
+        for pulse in rev_graph.pulses:
+            for s in pulse.sources:
+                assert s not in name_dict_small
+            assert pulse.dest not in name_dict_small
+        assert rename_cnt == 1
+
     def test_isclose(self):
         b1 = Builder(description="test", time_units="generations")
         b2 = copy.deepcopy(b1)
         b1.add_deme("d1", epochs=[dict(start_size=1000, end_time=0)])
         g1 = b1.resolve()
         g1.assert_close(g1)
         g1.assert_close(demes.loads(demes.dumps(g1)))
```

### Comparing `demes-0.2.2/tests/test_import_visibility.py` & `demes-0.2.3/tests/test_import_visibility.py`

 * *Files identical despite different names*

### Comparing `demes-0.2.2/tests/test_load_dump.py` & `demes-0.2.3/tests/test_load_dump.py`

 * *Files 2% similar despite different names*

```diff
@@ -571,14 +571,24 @@
             dest="B",
             start_time=T[1],
             end_time=T[2],
             rate=decimal.Decimal("0.000012345"),
         )
         self.check_dump_load_roundtrip(b.resolve())
 
+    def test_str_subclass(self):
+        # Check that numpy.str_ are round-trippable.
+        b = demes.Builder(defaults=dict(epoch=dict(start_size=1)))
+        names = np.array(["a", "b"])
+        b.add_deme(names[0])
+        b.add_deme(names[1], ancestors=[names[0]], start_time=50)
+        b.add_pulse(sources=[names[0]], dest=names[1], time=10, proportions=[0.1])
+        b.add_migration(source=names[0], dest=names[1], rate=1e-3)
+        self.check_dump_load_roundtrip(b.resolve())
+
     def test_json_infinities_get_stringified(self):
         b = demes.Builder()
         b.add_deme("a", epochs=[dict(start_size=1)])
         b.add_deme("b", epochs=[dict(start_size=1)])
         b.add_migration(source="a", dest="b", rate=1e-4)
         g1 = b.resolve()
         json_str = demes.dumps(g1, format="json", simplified=False)
```

### Comparing `demes-0.2.2/tests/test_ms.py` & `demes-0.2.3/tests/test_ms.py`

 * *Files 0% similar despite different names*

```diff
@@ -399,15 +399,14 @@
                     f"-ema {T1} 2 0 0 0 0",
                 ):
                     for on2 in (
                         # turn migration on again, with twice the rate, at t=T2
                         f"-em {T2} 1 2 {rate*2}",
                         f"-ema {T2} 2 0 {rate*2} 0 0",
                     ):
-
                         cmd = f"-I 2 0 2 {on1} {off} {on2}"
                         graph = demes.from_ms(cmd, N0=N0)
                         assert len(graph.migrations) == 2
                         # Check the migration details, but avoid depending on the
                         # ordering of the migrations list.
                         m1, m2 = sorted(graph.migrations, key=lambda m: m.end_time)
                         assert m1.end_time == 0
```

### Comparing `demes-0.2.2/tests/test_spec.py` & `demes-0.2.3/tests/test_spec.py`

 * *Files identical despite different names*

### Comparing `demes-0.2.2/verification.py` & `demes-0.2.3/verification.py`

 * *Files identical despite different names*

