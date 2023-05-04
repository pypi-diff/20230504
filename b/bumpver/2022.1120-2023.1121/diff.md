# Comparing `tmp/bumpver-2022.1120.tar.gz` & `tmp/bumpver-2023.1121.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bumpver-2022.1120.tar", last modified: Fri Dec  2 01:21:47 2022, max compression
+gzip compressed data, was "bumpver-2023.1121.tar", last modified: Thu May  4 16:35:11 2023, max compression
```

## Comparing `bumpver-2022.1120.tar` & `bumpver-2023.1121.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 mbarkhau  (1000) mbarkhau  (1000)        0 2022-12-02 01:21:47.978611 bumpver-2022.1120/
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)     8637 2022-12-02 00:43:35.000000 bumpver-2022.1120/CHANGELOG.md
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)     1127 2022-12-02 00:43:56.000000 bumpver-2022.1120/LICENSE
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)      148 2022-12-02 00:09:19.000000 bumpver-2022.1120/MANIFEST.in
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)    49885 2022-12-02 01:21:47.978611 bumpver-2022.1120/PKG-INFO
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)    40066 2022-12-02 00:43:56.000000 bumpver-2022.1120/README.md
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)     4053 2022-12-02 00:09:19.000000 bumpver-2022.1120/fastentrypoints.py
-drwxr-xr-x   0 mbarkhau  (1000) mbarkhau  (1000)        0 2022-12-02 01:21:47.968611 bumpver-2022.1120/requirements/
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)      648 2022-12-02 00:09:19.000000 bumpver-2022.1120/requirements/pypi.txt
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)     2370 2022-12-02 01:21:47.978611 bumpver-2022.1120/setup.cfg
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)     2457 2022-12-02 00:43:56.000000 bumpver-2022.1120/setup.py
-drwxr-xr-x   0 mbarkhau  (1000) mbarkhau  (1000)        0 2022-12-02 01:21:47.968611 bumpver-2022.1120/src/
-drwxr-xr-x   0 mbarkhau  (1000) mbarkhau  (1000)        0 2022-12-02 01:21:47.978611 bumpver-2022.1120/src/bumpver/
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)      262 2022-12-02 00:43:56.000000 bumpver-2022.1120/src/bumpver/__init__.py
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)      363 2022-12-02 00:43:56.000000 bumpver-2022.1120/src/bumpver/__main__.py
--rwxr-xr-x   0 mbarkhau  (1000) mbarkhau  (1000)    25562 2022-12-02 00:43:56.000000 bumpver-2022.1120/src/bumpver/cli.py
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)    21008 2022-12-02 00:43:56.000000 bumpver-2022.1120/src/bumpver/config.py
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)     2548 2022-12-02 00:43:56.000000 bumpver-2022.1120/src/bumpver/parse.py
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)      793 2022-12-02 00:43:56.000000 bumpver-2022.1120/src/bumpver/patterns.py
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)     1214 2022-12-02 00:43:56.000000 bumpver-2022.1120/src/bumpver/pysix.py
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)     2267 2022-12-02 00:43:56.000000 bumpver-2022.1120/src/bumpver/regexfmt.py
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)     2290 2022-12-02 00:43:56.000000 bumpver-2022.1120/src/bumpver/rewrite.py
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)      612 2022-12-02 00:43:56.000000 bumpver-2022.1120/src/bumpver/utils.py
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)     7915 2022-12-02 00:43:56.000000 bumpver-2022.1120/src/bumpver/v1patterns.py
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)     5257 2022-12-02 00:43:56.000000 bumpver-2022.1120/src/bumpver/v1rewrite.py
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)    13411 2022-12-02 00:43:56.000000 bumpver-2022.1120/src/bumpver/v1version.py
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)    11037 2022-12-02 00:43:56.000000 bumpver-2022.1120/src/bumpver/v2patterns.py
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)     5736 2022-12-02 00:43:56.000000 bumpver-2022.1120/src/bumpver/v2rewrite.py
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)    28055 2022-12-02 00:43:56.000000 bumpver-2022.1120/src/bumpver/v2version.py
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)     8275 2022-12-02 00:43:56.000000 bumpver-2022.1120/src/bumpver/vcs.py
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)     4042 2022-12-02 00:43:56.000000 bumpver-2022.1120/src/bumpver/version.py
-drwxr-xr-x   0 mbarkhau  (1000) mbarkhau  (1000)        0 2022-12-02 01:21:47.978611 bumpver-2022.1120/src/bumpver.egg-info/
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)    49885 2022-12-02 01:21:47.000000 bumpver-2022.1120/src/bumpver.egg-info/PKG-INFO
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)     1262 2022-12-02 01:21:47.000000 bumpver-2022.1120/src/bumpver.egg-info/SOURCES.txt
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)        1 2022-12-02 01:21:47.000000 bumpver-2022.1120/src/bumpver.egg-info/dependency_links.txt
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)       44 2022-12-02 01:21:47.000000 bumpver-2022.1120/src/bumpver.egg-info/entry_points.txt
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)      204 2022-12-02 01:21:47.000000 bumpver-2022.1120/src/bumpver.egg-info/requires.txt
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)        8 2022-12-02 01:21:47.000000 bumpver-2022.1120/src/bumpver.egg-info/top_level.txt
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)        1 2022-12-02 01:21:47.000000 bumpver-2022.1120/src/bumpver.egg-info/zip-safe
-drwxr-xr-x   0 mbarkhau  (1000) mbarkhau  (1000)        0 2022-12-02 01:21:47.978611 bumpver-2022.1120/test/
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)        0 2022-12-02 00:09:19.000000 bumpver-2022.1120/test/__init__.py
-drwxr-xr-x   0 mbarkhau  (1000) mbarkhau  (1000)        0 2022-12-02 01:21:47.968611 bumpver-2022.1120/test/fixtures/
-drwxr-xr-x   0 mbarkhau  (1000) mbarkhau  (1000)        0 2022-12-02 01:21:47.978611 bumpver-2022.1120/test/fixtures/project_a/
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)       66 2022-12-02 00:09:19.000000 bumpver-2022.1120/test/fixtures/project_a/README.md
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)      266 2022-12-02 00:09:19.000000 bumpver-2022.1120/test/fixtures/project_a/bumpver.toml
-drwxr-xr-x   0 mbarkhau  (1000) mbarkhau  (1000)        0 2022-12-02 01:21:47.978611 bumpver-2022.1120/test/fixtures/project_b/
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)      219 2022-12-02 00:09:19.000000 bumpver-2022.1120/test/fixtures/project_b/README.rst
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)      461 2022-12-02 00:09:19.000000 bumpver-2022.1120/test/fixtures/project_b/setup.cfg
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)      136 2022-12-02 00:09:19.000000 bumpver-2022.1120/test/fixtures/project_b/setup.py
-drwxr-xr-x   0 mbarkhau  (1000) mbarkhau  (1000)        0 2022-12-02 01:21:47.968611 bumpver-2022.1120/test/fixtures/project_b/src/
-drwxr-xr-x   0 mbarkhau  (1000) mbarkhau  (1000)        0 2022-12-02 01:21:47.978611 bumpver-2022.1120/test/fixtures/project_b/src/module_v1/
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)       34 2022-12-02 00:09:19.000000 bumpver-2022.1120/test/fixtures/project_b/src/module_v1/__init__.py
-drwxr-xr-x   0 mbarkhau  (1000) mbarkhau  (1000)        0 2022-12-02 01:21:47.978611 bumpver-2022.1120/test/fixtures/project_b/src/module_v2/
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)       34 2022-12-02 00:09:19.000000 bumpver-2022.1120/test/fixtures/project_b/src/module_v2/__init__.py
-drwxr-xr-x   0 mbarkhau  (1000) mbarkhau  (1000)        0 2022-12-02 01:21:47.978611 bumpver-2022.1120/test/fixtures/project_c/
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)      135 2022-12-02 00:09:19.000000 bumpver-2022.1120/test/fixtures/project_c/pyproject.toml
-drwxr-xr-x   0 mbarkhau  (1000) mbarkhau  (1000)        0 2022-12-02 01:21:47.978611 bumpver-2022.1120/test/fixtures/project_d/
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)      114 2022-12-02 00:09:19.000000 bumpver-2022.1120/test/fixtures/project_d/pyproject.toml
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)    41823 2022-12-02 00:43:35.000000 bumpver-2022.1120/test/test_cli.py
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)    11574 2022-12-02 00:09:19.000000 bumpver-2022.1120/test/test_config.py
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)     2381 2022-12-02 00:09:19.000000 bumpver-2022.1120/test/test_parse.py
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)     9708 2022-12-02 00:09:19.000000 bumpver-2022.1120/test/test_patterns.py
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)    12813 2022-12-02 00:09:19.000000 bumpver-2022.1120/test/test_rewrite.py
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)    10453 2022-12-02 00:09:19.000000 bumpver-2022.1120/test/test_version.py
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)     2481 2022-12-02 00:09:19.000000 bumpver-2022.1120/test/util.py
+drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-04 16:35:11.679573 bumpver-2023.1121/
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     8986 2023-05-04 16:01:47.000000 bumpver-2023.1121/CHANGELOG.md
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     1127 2023-05-04 16:02:43.000000 bumpver-2023.1121/LICENSE
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      148 2023-05-04 13:50:20.000000 bumpver-2023.1121/MANIFEST.in
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    50255 2023-05-04 16:35:11.679573 bumpver-2023.1121/PKG-INFO
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    40087 2023-05-04 16:02:43.000000 bumpver-2023.1121/README.md
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     4053 2023-05-04 13:50:20.000000 bumpver-2023.1121/fastentrypoints.py
+drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-04 16:35:09.968430 bumpver-2023.1121/requirements/
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      697 2023-05-04 14:52:41.000000 bumpver-2023.1121/requirements/pypi.txt
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     2370 2023-05-04 16:35:11.679573 bumpver-2023.1121/setup.cfg
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     2457 2023-05-04 16:02:43.000000 bumpver-2023.1121/setup.py
+drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-04 16:35:09.735361 bumpver-2023.1121/src/
+drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-04 16:35:10.657263 bumpver-2023.1121/src/bumpver/
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      262 2023-05-04 16:02:43.000000 bumpver-2023.1121/src/bumpver/__init__.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      363 2023-05-04 16:02:43.000000 bumpver-2023.1121/src/bumpver/__main__.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    25569 2023-05-04 16:02:43.000000 bumpver-2023.1121/src/bumpver/cli.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    21008 2023-05-04 16:02:43.000000 bumpver-2023.1121/src/bumpver/config.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     2548 2023-05-04 16:02:43.000000 bumpver-2023.1121/src/bumpver/parse.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      793 2023-05-04 16:02:43.000000 bumpver-2023.1121/src/bumpver/patterns.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     1214 2023-05-04 16:02:43.000000 bumpver-2023.1121/src/bumpver/pysix.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     2267 2023-05-04 16:02:43.000000 bumpver-2023.1121/src/bumpver/regexfmt.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     2290 2023-05-04 16:02:43.000000 bumpver-2023.1121/src/bumpver/rewrite.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      612 2023-05-04 16:02:43.000000 bumpver-2023.1121/src/bumpver/utils.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     7915 2023-05-04 16:02:43.000000 bumpver-2023.1121/src/bumpver/v1patterns.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     5257 2023-05-04 16:02:43.000000 bumpver-2023.1121/src/bumpver/v1rewrite.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    13411 2023-05-04 16:02:43.000000 bumpver-2023.1121/src/bumpver/v1version.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    11045 2023-05-04 16:02:43.000000 bumpver-2023.1121/src/bumpver/v2patterns.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     5736 2023-05-04 16:02:43.000000 bumpver-2023.1121/src/bumpver/v2rewrite.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    28055 2023-05-04 16:02:43.000000 bumpver-2023.1121/src/bumpver/v2version.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     8275 2023-05-04 16:02:43.000000 bumpver-2023.1121/src/bumpver/vcs.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     4177 2023-05-04 16:02:43.000000 bumpver-2023.1121/src/bumpver/version.py
+drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-04 16:35:11.054247 bumpver-2023.1121/src/bumpver.egg-info/
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    50255 2023-05-04 16:35:09.000000 bumpver-2023.1121/src/bumpver.egg-info/PKG-INFO
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     1262 2023-05-04 16:35:09.000000 bumpver-2023.1121/src/bumpver.egg-info/SOURCES.txt
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        1 2023-05-04 16:35:09.000000 bumpver-2023.1121/src/bumpver.egg-info/dependency_links.txt
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)       44 2023-05-04 16:35:09.000000 bumpver-2023.1121/src/bumpver.egg-info/entry_points.txt
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      198 2023-05-04 16:35:09.000000 bumpver-2023.1121/src/bumpver.egg-info/requires.txt
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        8 2023-05-04 16:35:09.000000 bumpver-2023.1121/src/bumpver.egg-info/top_level.txt
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        1 2023-05-04 16:35:09.000000 bumpver-2023.1121/src/bumpver.egg-info/zip-safe
+drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-04 16:35:11.271266 bumpver-2023.1121/test/
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-04 13:50:20.000000 bumpver-2023.1121/test/__init__.py
+drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-04 16:35:09.817424 bumpver-2023.1121/test/fixtures/
+drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-04 16:35:11.335332 bumpver-2023.1121/test/fixtures/project_a/
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)       66 2023-05-04 13:50:20.000000 bumpver-2023.1121/test/fixtures/project_a/README.md
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      266 2023-05-04 13:50:20.000000 bumpver-2023.1121/test/fixtures/project_a/bumpver.toml
+drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-04 16:35:11.460004 bumpver-2023.1121/test/fixtures/project_b/
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      219 2023-05-04 13:50:20.000000 bumpver-2023.1121/test/fixtures/project_b/README.rst
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      461 2023-05-04 13:50:20.000000 bumpver-2023.1121/test/fixtures/project_b/setup.cfg
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      136 2023-05-04 13:50:20.000000 bumpver-2023.1121/test/fixtures/project_b/setup.py
+drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-04 16:35:09.797842 bumpver-2023.1121/test/fixtures/project_b/src/
+drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-04 16:35:11.506882 bumpver-2023.1121/test/fixtures/project_b/src/module_v1/
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)       34 2023-05-04 13:50:20.000000 bumpver-2023.1121/test/fixtures/project_b/src/module_v1/__init__.py
+drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-04 16:35:11.569787 bumpver-2023.1121/test/fixtures/project_b/src/module_v2/
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)       34 2023-05-04 13:50:20.000000 bumpver-2023.1121/test/fixtures/project_b/src/module_v2/__init__.py
+drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-04 16:35:11.601036 bumpver-2023.1121/test/fixtures/project_c/
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      135 2023-05-04 13:50:20.000000 bumpver-2023.1121/test/fixtures/project_c/pyproject.toml
+drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-04 16:35:11.648322 bumpver-2023.1121/test/fixtures/project_d/
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      114 2023-05-04 16:02:18.000000 bumpver-2023.1121/test/fixtures/project_d/pyproject.toml
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    42098 2023-05-04 16:01:47.000000 bumpver-2023.1121/test/test_cli.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    11574 2023-05-04 16:02:18.000000 bumpver-2023.1121/test/test_config.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     2381 2023-05-04 13:50:20.000000 bumpver-2023.1121/test/test_parse.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     9708 2023-05-04 13:50:20.000000 bumpver-2023.1121/test/test_patterns.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    12813 2023-05-04 13:50:20.000000 bumpver-2023.1121/test/test_rewrite.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    10453 2023-05-04 13:50:20.000000 bumpver-2023.1121/test/test_version.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     2481 2023-05-04 13:50:20.000000 bumpver-2023.1121/test/util.py
```

### Comparing `bumpver-2022.1120/CHANGELOG.md` & `bumpver-2023.1121/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,20 @@
 # Changelog for https://github.com/mbarkhau/bumpver
 
+## BumpVer 2023.1121
+
+- Fix [#200][gh_i200]: Fix compatability with packaging 23.0.
+- Fix [#203][gh_i203]: Add dev to the list of valid release tags
+
+[gh_i200]: https://github.com/mbarkhau/bumpver/issues/200
+[gh_i203]: https://github.com/mbarkhau/bumpver/issues/203
+
+Thank you [Sharon Yogev](https://github.com/sharonyogev) for your contribution.
+
+
 ## BumpVer 2022.1120
 
 - Fix [#196][gh_i196]: Add `--pin-increments`.
 
 [gh_i196]: https://github.com/mbarkhau/bumpver/issues/196
 
 Thank you [Markus Holtermann](https://github.com/MarkusH) for
```

### Comparing `bumpver-2022.1120/LICENSE` & `bumpver-2023.1121/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-MIT License Copyright (c) 2018-2022 Manuel Barkhau (mbarkhau@gmail.com)
+MIT License Copyright (c) 2018-2023 Manuel Barkhau (mbarkhau@gmail.com)
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is furnished
 to do so, subject to the following conditions:
```

### Comparing `bumpver-2022.1120/PKG-INFO` & `bumpver-2023.1121/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bumpver
-Version: 2022.1120
+Version: 2023.1121
 Summary: Bump version numbers in project files.
 Home-page: https://github.com/mbarkhau/bumpver
 Author: Manuel Barkhau
 Author-email: mbarkhau@gmail.com
 License: MIT
 Keywords: version bumpver calver semver versioning bumpversion pep440
 Classifier: Development Status :: 4 - Beta
@@ -47,15 +47,15 @@
 [url_calver_org]: https://calver.org/
 
 
 Project/Repo:
 
 [![MIT License][img_license]][url_license]
 [![Supported Python Versions][img_pyversions]][url_pyversions]
-[![CalVer 2022.1120][img_version]][url_version]
+[![CalVer 2023.1121][img_version]][url_version]
 [![PyPI Releases][img_pypi]][url_pypi]
 [![PyPI Downloads][img_downloads]][url_downloads]
 
 Code Quality/CI:
 
 [![GitHub Build Status][img_github_build]][url_github_build]
 [![GitLab Build Status][img_gitlab_build]][url_gitlab_build]
@@ -81,15 +81,15 @@
 
 [img_style]: https://img.shields.io/badge/code%20style-%20sjfmt-f71.svg
 [url_style]: https://gitlab.com/mbarkhau/straitjacket/
 
 [img_downloads]: https://pepy.tech/badge/bumpver/month
 [url_downloads]: https://pepy.tech/project/bumpver
 
-[img_version]: https://img.shields.io/static/v1.svg?label=CalVer&message=2022.1120&color=blue
+[img_version]: https://img.shields.io/static/v1.svg?label=CalVer&message=2023.1121&color=blue
 [url_version]: https://pypi.org/project/bumpver/
 
 [img_pypi]: https://img.shields.io/badge/PyPI-wheels-green.svg
 [url_pypi]: https://pypi.org/project/bumpver/#files
 
 [img_pyversions]: https://img.shields.io/pypi/pyversions/bumpver.svg
 [url_pyversions]: https://pypi.python.org/pypi/bumpver
@@ -634,15 +634,15 @@
   --date <ISODATE>                Set explicit date in format YYYY-0M-0D (e.g.
                                   2021-05-13).
   --pin-date                      Leave date components unchanged.
   --pin-increments                Leave the auto-increments INC0 and INC1
   --tag-num                       Increment release tag number (rc1, rc2,
                                   rc3..).
   -t, --tag <NAME>                Override release tag of current_version. Valid
-                                  options are: alpha, beta, rc, post, final.
+                                  options are: alpha, beta, dev, rc, post, final.
   -p, --patch                     Increment PATCH component.
   -m, --minor                     Increment MINOR component.
   --major                         Increment MAJOR component.
   -c, --commit-message <TMPL>     Set commit message template.
   --commit / --no-commit          Create a commit with all updated files.
   --tag-commit / --no-tag-commit  Tag the newly created commit.
   --push / --no-push              Push to the default remote.
@@ -669,30 +669,30 @@
 
 ### Part Overview
 
 > Where possible, these patterns match the conventions from [CalVer.org][url_calver_org_scheme].
 
 [url_calver_org_scheme]: https://calver.org/#scheme
 
-|    part    |     range / example(s)    |                     info                    |
-|------------|---------------------------|---------------------------------------------|
-| `MAJOR`    | 0..9, 10..99, 100..       | `bumpver update --major`                    |
-| `MINOR`    | 0..9, 10..99, 100..       | `bumpver update --minor`                    |
-| `PATCH`    | 0..9, 10..99, 100..       | `bumpver update --patch`                    |
-| `TAG`      | alpha, beta, rc, post     | `--tag=<tag>`                               |
-| `PYTAG`    | a, b, rc, post            | `--tag=<tag>`                               |
-| `NUM`      | 0, 1, 2...                | `-r/--tag-num`                              |
-| `YYYY`     | 2019, 2020...             | Full year, based on `strftime('%Y')`        |
-| `YY`       | 18, 19..99, 0, 1          | Short year, based on `int(strftime('%y'))`  |
-| `MM`       | 9, 10, 11, 12             | Month, based on `int(strftime('%m'))`       |
-| `DD`       | 1, 2, 3..31               | Day, based on `int(strftime('%d'))`         |
-| `BUILD`    | 1001, 1002 .. 1999, 22000 | build number (maintains lexical order)      |
-| `INC0`     | 0, 1, 2...                | 0-based auto incrementing number            |
-| `INC1`     | 1, 2...                   | 1-based auto incrementing number            |
-| `PYTAGNUM` | a0, a1, rc0, ...          | `PYTAG` + `NUM` (no white-space in between) |
+|    part    | range / example(s)         |                     info                    |
+|------------|----------------------------|---------------------------------------------|
+| `MAJOR`    | 0..9, 10..99, 100..        | `bumpver update --major`                    |
+| `MINOR`    | 0..9, 10..99, 100..        | `bumpver update --minor`                    |
+| `PATCH`    | 0..9, 10..99, 100..        | `bumpver update --patch`                    |
+| `TAG`      | dev, alpha, beta, rc, post | `--tag=<tag>`                               |
+| `PYTAG`    | a, b, rc, post             | `--tag=<tag>`                               |
+| `NUM`      | 0, 1, 2...                 | `-r/--tag-num`                              |
+| `YYYY`     | 2019, 2020...              | Full year, based on `strftime('%Y')`        |
+| `YY`       | 18, 19..99, 0, 1           | Short year, based on `int(strftime('%y'))`  |
+| `MM`       | 9, 10, 11, 12              | Month, based on `int(strftime('%m'))`       |
+| `DD`       | 1, 2, 3..31                | Day, based on `int(strftime('%d'))`         |
+| `BUILD`    | 1001, 1002 .. 1999, 22000  | build number (maintains lexical order)      |
+| `INC0`     | 0, 1, 2...                 | 0-based auto incrementing number            |
+| `INC1`     | 1, 2...                    | 1-based auto incrementing number            |
+| `PYTAGNUM` | a0, a1, rc0, ...           | `PYTAG` + `NUM` (no white-space in between) |
 
 
 The following are also available, but you should review the [Normalization Caveats](#normalization-caveats) before you decide to use them.
 
 
 | part   | range / example(s)  | comment                                      |
 | ------ | ------------------- | -------------------------------------------- |
@@ -821,15 +821,15 @@
 
 The create an initial configuration for project with `bumpver init`.
 
 ```shell
 $ pip install bumpver
 ...
 Installing collected packages: click toml lexid bumpver
-Successfully installed bumpver-2022.1120
+Successfully installed bumpver-2023.1121
 
 $ cd myproject
 ~/myproject/
 
 $ bumpver init --dry
 Exiting because of '-d/--dry'. Would have written to bumpver.toml:
 
@@ -1117,14 +1117,25 @@
 |                Name                 |    role           |  since  | until |
 |-------------------------------------|-------------------|---------|-------|
 | Manuel Barkhau (mbarkhau@gmail.com) | author/maintainer | 2018-09 | -     |
 
 
 # Changelog for https://github.com/mbarkhau/bumpver
 
+## BumpVer 2023.1121
+
+- Fix [#200][gh_i200]: Fix compatability with packaging 23.0.
+- Fix [#203][gh_i203]: Add dev to the list of valid release tags
+
+[gh_i200]: https://github.com/mbarkhau/bumpver/issues/200
+[gh_i203]: https://github.com/mbarkhau/bumpver/issues/203
+
+Thank you [Sharon Yogev](https://github.com/sharonyogev) for your contribution.
+
+
 ## BumpVer 2022.1120
 
 - Fix [#196][gh_i196]: Add `--pin-increments`.
 
 [gh_i196]: https://github.com/mbarkhau/bumpver/issues/196
 
 Thank you [Markus Holtermann](https://github.com/MarkusH) for
```

### Comparing `bumpver-2022.1120/README.md` & `bumpver-2023.1121/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 [url_calver_org]: https://calver.org/
 
 
 Project/Repo:
 
 [![MIT License][img_license]][url_license]
 [![Supported Python Versions][img_pyversions]][url_pyversions]
-[![CalVer 2022.1120][img_version]][url_version]
+[![CalVer 2023.1121][img_version]][url_version]
 [![PyPI Releases][img_pypi]][url_pypi]
 [![PyPI Downloads][img_downloads]][url_downloads]
 
 Code Quality/CI:
 
 [![GitHub Build Status][img_github_build]][url_github_build]
 [![GitLab Build Status][img_gitlab_build]][url_gitlab_build]
@@ -52,15 +52,15 @@
 
 [img_style]: https://img.shields.io/badge/code%20style-%20sjfmt-f71.svg
 [url_style]: https://gitlab.com/mbarkhau/straitjacket/
 
 [img_downloads]: https://pepy.tech/badge/bumpver/month
 [url_downloads]: https://pepy.tech/project/bumpver
 
-[img_version]: https://img.shields.io/static/v1.svg?label=CalVer&message=2022.1120&color=blue
+[img_version]: https://img.shields.io/static/v1.svg?label=CalVer&message=2023.1121&color=blue
 [url_version]: https://pypi.org/project/bumpver/
 
 [img_pypi]: https://img.shields.io/badge/PyPI-wheels-green.svg
 [url_pypi]: https://pypi.org/project/bumpver/#files
 
 [img_pyversions]: https://img.shields.io/pypi/pyversions/bumpver.svg
 [url_pyversions]: https://pypi.python.org/pypi/bumpver
@@ -605,15 +605,15 @@
   --date <ISODATE>                Set explicit date in format YYYY-0M-0D (e.g.
                                   2021-05-13).
   --pin-date                      Leave date components unchanged.
   --pin-increments                Leave the auto-increments INC0 and INC1
   --tag-num                       Increment release tag number (rc1, rc2,
                                   rc3..).
   -t, --tag <NAME>                Override release tag of current_version. Valid
-                                  options are: alpha, beta, rc, post, final.
+                                  options are: alpha, beta, dev, rc, post, final.
   -p, --patch                     Increment PATCH component.
   -m, --minor                     Increment MINOR component.
   --major                         Increment MAJOR component.
   -c, --commit-message <TMPL>     Set commit message template.
   --commit / --no-commit          Create a commit with all updated files.
   --tag-commit / --no-tag-commit  Tag the newly created commit.
   --push / --no-push              Push to the default remote.
@@ -640,30 +640,30 @@
 
 ### Part Overview
 
 > Where possible, these patterns match the conventions from [CalVer.org][url_calver_org_scheme].
 
 [url_calver_org_scheme]: https://calver.org/#scheme
 
-|    part    |     range / example(s)    |                     info                    |
-|------------|---------------------------|---------------------------------------------|
-| `MAJOR`    | 0..9, 10..99, 100..       | `bumpver update --major`                    |
-| `MINOR`    | 0..9, 10..99, 100..       | `bumpver update --minor`                    |
-| `PATCH`    | 0..9, 10..99, 100..       | `bumpver update --patch`                    |
-| `TAG`      | alpha, beta, rc, post     | `--tag=<tag>`                               |
-| `PYTAG`    | a, b, rc, post            | `--tag=<tag>`                               |
-| `NUM`      | 0, 1, 2...                | `-r/--tag-num`                              |
-| `YYYY`     | 2019, 2020...             | Full year, based on `strftime('%Y')`        |
-| `YY`       | 18, 19..99, 0, 1          | Short year, based on `int(strftime('%y'))`  |
-| `MM`       | 9, 10, 11, 12             | Month, based on `int(strftime('%m'))`       |
-| `DD`       | 1, 2, 3..31               | Day, based on `int(strftime('%d'))`         |
-| `BUILD`    | 1001, 1002 .. 1999, 22000 | build number (maintains lexical order)      |
-| `INC0`     | 0, 1, 2...                | 0-based auto incrementing number            |
-| `INC1`     | 1, 2...                   | 1-based auto incrementing number            |
-| `PYTAGNUM` | a0, a1, rc0, ...          | `PYTAG` + `NUM` (no white-space in between) |
+|    part    | range / example(s)         |                     info                    |
+|------------|----------------------------|---------------------------------------------|
+| `MAJOR`    | 0..9, 10..99, 100..        | `bumpver update --major`                    |
+| `MINOR`    | 0..9, 10..99, 100..        | `bumpver update --minor`                    |
+| `PATCH`    | 0..9, 10..99, 100..        | `bumpver update --patch`                    |
+| `TAG`      | dev, alpha, beta, rc, post | `--tag=<tag>`                               |
+| `PYTAG`    | a, b, rc, post             | `--tag=<tag>`                               |
+| `NUM`      | 0, 1, 2...                 | `-r/--tag-num`                              |
+| `YYYY`     | 2019, 2020...              | Full year, based on `strftime('%Y')`        |
+| `YY`       | 18, 19..99, 0, 1           | Short year, based on `int(strftime('%y'))`  |
+| `MM`       | 9, 10, 11, 12              | Month, based on `int(strftime('%m'))`       |
+| `DD`       | 1, 2, 3..31                | Day, based on `int(strftime('%d'))`         |
+| `BUILD`    | 1001, 1002 .. 1999, 22000  | build number (maintains lexical order)      |
+| `INC0`     | 0, 1, 2...                 | 0-based auto incrementing number            |
+| `INC1`     | 1, 2...                    | 1-based auto incrementing number            |
+| `PYTAGNUM` | a0, a1, rc0, ...           | `PYTAG` + `NUM` (no white-space in between) |
 
 
 The following are also available, but you should review the [Normalization Caveats](#normalization-caveats) before you decide to use them.
 
 
 | part   | range / example(s)  | comment                                      |
 | ------ | ------------------- | -------------------------------------------- |
@@ -792,15 +792,15 @@
 
 The create an initial configuration for project with `bumpver init`.
 
 ```shell
 $ pip install bumpver
 ...
 Installing collected packages: click toml lexid bumpver
-Successfully installed bumpver-2022.1120
+Successfully installed bumpver-2023.1121
 
 $ cd myproject
 ~/myproject/
 
 $ bumpver init --dry
 Exiting because of '-d/--dry'. Would have written to bumpver.toml:
```

### Comparing `bumpver-2022.1120/fastentrypoints.py` & `bumpver-2023.1121/fastentrypoints.py`

 * *Files identical despite different names*

### Comparing `bumpver-2022.1120/requirements/pypi.txt` & `bumpver-2023.1121/requirements/pypi.txt`

 * *Files 15% similar despite different names*

```diff
@@ -11,11 +11,13 @@
 typing; python_version < "3.5"
 click<8.0; python_version < "3.6"
 click; python_version >= "3.6"
 toml
 lexid
 colorama>=0.4
 
+# looseversion is needed to parse non PEP440 versions
+looseversion; python_version >= "3.5"
+
 # setuptools is needed for pkg_resources.parse_version
 # Support for Python 2 was dropped with v45
 setuptools<45.0.0; python_version < "3.5"
-setuptools>=45.0.0; python_version >= "3.5"
```

### Comparing `bumpver-2022.1120/setup.cfg` & `bumpver-2023.1121/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 	dist/
 	.mypy_cache
 
 [tool:pytest]
 addopts = --doctest-modules
 
 [bumpver]
-current_version = "2022.1120"
+current_version = "2023.1121"
 version_pattern = "YYYY.BUILD[-TAG]"
 commit_message = "bump {old_version} -> {new_version}"
 commit = True
 tag = True
 push = True
 
 [bumpver:file_patterns]
```

### Comparing `bumpver-2022.1120/setup.py` & `bumpver-2023.1121/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
 setuptools.setup(
     name="bumpver",
     license="MIT",
     author="Manuel Barkhau",
     author_email="mbarkhau@gmail.com",
     url="https://github.com/mbarkhau/bumpver",
-    version="2022.1120",
+    version="2023.1121",
     keywords="version bumpver calver semver versioning bumpversion pep440",
     description="Bump version numbers in project files.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages("src"),
     package_dir=package_dir,
     install_requires=install_requires,
```

### Comparing `bumpver-2022.1120/src/bumpver/cli.py` & `bumpver-2023.1121/src/bumpver/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # This file is part of the bumpver project
 # https://github.com/mbarkhau/bumpver
 #
-# Copyright (c) 2018-2022 Manuel Barkhau (mbarkhau@gmail.com) - MIT License
+# Copyright (c) 2018-2023 Manuel Barkhau (mbarkhau@gmail.com) - MIT License
 # SPDX-License-Identifier: MIT
 """cli module for BumpVer."""
 import io
 import re
 import sys
 import typing as typ
 import logging
@@ -64,15 +64,15 @@
         log_format = "%(levelname)-7s - %(message)s"
         log_level  = logging.INFO
 
     logging.basicConfig(level=log_level, format=log_format, datefmt="%Y-%m-%dT%H:%M:%S")
     logger.debug("Logging configured.")
 
 
-VALID_RELEASE_TAG_VALUES = ("alpha", "beta", "rc", "post", "final")
+VALID_RELEASE_TAG_VALUES = ("alpha", "beta", "dev", "rc", "post", "final")
 
 
 _current_date = dt.date.today().isoformat()
 
 
 def _validate_date(date: typ.Optional[str], pin_date: bool) -> typ.Optional[dt.date]:
     if date and pin_date:
@@ -249,15 +249,15 @@
     decorated = function
     for decorator in decorators:
         decorated = decorator(decorated)
     return decorated
 
 
 @click.group(context_settings={'help_option_names': ["-h", "--help"]})
-@click.version_option(version="2022.1120")
+@click.version_option(version="2023.1121")
 @verbose_option
 def cli(verbose: int = 0) -> None:
     """Automatically update version strings in plaintext files."""
     if verbose:
         _configure_logging(verbose=max(_VERBOSE, verbose))
```

### Comparing `bumpver-2022.1120/src/bumpver/config.py` & `bumpver-2023.1121/src/bumpver/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # This file is part of the bumpver project
 # https://gitlab.com/mbarkhau/bumpver
 #
-# Copyright (c) 2018-2022 Manuel Barkhau (mbarkhau@gmail.com) - MIT License
+# Copyright (c) 2018-2023 Manuel Barkhau (mbarkhau@gmail.com) - MIT License
 # SPDX-License-Identifier: MIT
 """Parse bumpver.toml, setup.cfg or pyproject.toml files."""
 
 import re
 import typing as typ
 import logging
 import datetime as dt
```

### Comparing `bumpver-2022.1120/src/bumpver/parse.py` & `bumpver-2023.1121/src/bumpver/parse.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # This file is part of the bumpver project
 # https://github.com/mbarkhau/bumpver
 #
-# Copyright (c) 2018-2022 Manuel Barkhau (mbarkhau@gmail.com) - MIT License
+# Copyright (c) 2018-2023 Manuel Barkhau (mbarkhau@gmail.com) - MIT License
 # SPDX-License-Identifier: MIT
 """Parse PyCalVer strings from files."""
 
 import typing as typ
 
 from .patterns import Pattern
```

### Comparing `bumpver-2022.1120/src/bumpver/patterns.py` & `bumpver-2023.1121/src/bumpver/patterns.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # This file is part of the bumpver project
 # https://github.com/mbarkhau/bumpver
 #
-# Copyright (c) 2018-2022 Manuel Barkhau (mbarkhau@gmail.com) - MIT License
+# Copyright (c) 2018-2023 Manuel Barkhau (mbarkhau@gmail.com) - MIT License
 # SPDX-License-Identifier: MIT
 import typing as typ
 
 
 class Pattern(typ.NamedTuple):
 
     version_pattern: str  # "{pycalver}", "{year}.{month}", "vYYYY0M.BUILD"
```

### Comparing `bumpver-2022.1120/src/bumpver/pysix.py` & `bumpver-2023.1121/src/bumpver/pysix.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # This file is part of the bumpver project
 # https://github.com/mbarkhau/bumpver
 #
-# Copyright (c) 2018-2022 Manuel Barkhau (mbarkhau@gmail.com) - MIT License
+# Copyright (c) 2018-2023 Manuel Barkhau (mbarkhau@gmail.com) - MIT License
 # SPDX-License-Identifier: MIT
 import sys
 import typing as typ
 
 PY2 = sys.version_info.major < 3
```

### Comparing `bumpver-2022.1120/src/bumpver/regexfmt.py` & `bumpver-2023.1121/src/bumpver/regexfmt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # This file is part of the bumpver project
 # https://github.com/mbarkhau/bumpver
 #
-# Copyright (c) 2018-2022 Manuel Barkhau (mbarkhau@gmail.com) - MIT License
+# Copyright (c) 2018-2023 Manuel Barkhau (mbarkhau@gmail.com) - MIT License
 # SPDX-License-Identifier: MIT
 import re
 import logging
 import textwrap
 
 from . import pysix
```

### Comparing `bumpver-2022.1120/src/bumpver/rewrite.py` & `bumpver-2023.1121/src/bumpver/rewrite.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # This file is part of the bumpver project
 # https://github.com/mbarkhau/bumpver
 #
-# Copyright (c) 2018-2022 Manuel Barkhau (mbarkhau@gmail.com) - MIT License
+# Copyright (c) 2018-2023 Manuel Barkhau (mbarkhau@gmail.com) - MIT License
 # SPDX-License-Identifier: MIT
 import typing as typ
 import difflib
 
 import pathlib2 as pl
 
 from . import config
```

### Comparing `bumpver-2022.1120/src/bumpver/utils.py` & `bumpver-2023.1121/src/bumpver/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # This file is part of the bumpver project
 # https://github.com/mbarkhau/bumpver
 #
-# Copyright (c) 2018-2022 Manuel Barkhau (mbarkhau@gmail.com) - MIT License
+# Copyright (c) 2018-2023 Manuel Barkhau (mbarkhau@gmail.com) - MIT License
 # SPDX-License-Identifier: MIT
 import typing as typ
 import functools
 
 # NOTE (mb 2020-09-24): The main use of the memo function is
 #   not as a performance optimization, but to reduce logging
 #   spam.
```

### Comparing `bumpver-2022.1120/src/bumpver/v1patterns.py` & `bumpver-2023.1121/src/bumpver/v1patterns.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # This file is part of the bumpver project
 # https://github.com/mbarkhau/bumpver
 #
-# Copyright (c) 2018-2022 Manuel Barkhau (mbarkhau@gmail.com) - MIT License
+# Copyright (c) 2018-2023 Manuel Barkhau (mbarkhau@gmail.com) - MIT License
 # SPDX-License-Identifier: MIT
 """Compose Regular Expressions from Patterns.
 
 >>> version_info = PYCALVER_RE.match("v201712.0123-alpha").groupdict()
 >>> assert version_info == {
 ...     "pycalver"    : "v201712.0123-alpha",
 ...     "vYYYYMM"     : "v201712",
```

### Comparing `bumpver-2022.1120/src/bumpver/v1rewrite.py` & `bumpver-2023.1121/src/bumpver/v1rewrite.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # This file is part of the bumpver project
 # https://github.com/mbarkhau/bumpver
 #
-# Copyright (c) 2018-2022 Manuel Barkhau (mbarkhau@gmail.com) - MIT License
+# Copyright (c) 2018-2023 Manuel Barkhau (mbarkhau@gmail.com) - MIT License
 # SPDX-License-Identifier: MIT
 """Rewrite files, updating occurences of version strings."""
 
 import io
 import typing as typ
 import logging
```

### Comparing `bumpver-2022.1120/src/bumpver/v1version.py` & `bumpver-2023.1121/src/bumpver/v1version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # This file is part of the bumpver project
 # https://github.com/mbarkhau/bumpver
 #
-# Copyright (c) 2018-2022 Manuel Barkhau (mbarkhau@gmail.com) - MIT License
+# Copyright (c) 2018-2023 Manuel Barkhau (mbarkhau@gmail.com) - MIT License
 # SPDX-License-Identifier: MIT
 """Functions related to version string manipulation."""
 
 import typing as typ
 import logging
 import datetime as dt
```

### Comparing `bumpver-2022.1120/src/bumpver/v2patterns.py` & `bumpver-2023.1121/src/bumpver/v2patterns.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # This file is part of the bumpver project
 # https://github.com/mbarkhau/bumpver
 #
-# Copyright (c) 2018-2022 Manuel Barkhau (mbarkhau@gmail.com) - MIT License
+# Copyright (c) 2018-2023 Manuel Barkhau (mbarkhau@gmail.com) - MIT License
 # SPDX-License-Identifier: MIT
 """Compose Regular Expressions from Patterns.
 
 >>> pattern = compile_pattern("vYYYY0M.BUILD[-TAG]")
 >>> version_info = pattern.regexp.match("v201712.0123-alpha")
 >>> assert version_info.groupdict() == {
 ...     "year_y" : "2017",
@@ -78,16 +78,16 @@
         ('0V', r"5[0-3]|[1-4][0-9]|0[1-9]"),
         # non calver parts
         ('MAJOR'  , r"[0-9]+"),
         ('MINOR'  , r"[0-9]+"),
         ('PATCH'  , r"[0-9]+"),
         ('BUILD'  , r"[0-9]+"),
         ('BLD'    , r"[1-9][0-9]*"),
-        ('TAG'    , r"preview|final|alpha|beta|post|rc"),
-        ('PYTAG'  , r"post|rc|a|b"),
+        ('TAG'    , r"preview|final|dev|alpha|beta|post|rc"),
+        ('PYTAG'  , r"dev|post|rc|a|b"),
         ('GITHASH', r"\.[0-9]+\+.*"),
         ('NUM'    , r"[0-9]+"),
         ('INC0'   , r"[0-9]+"),
         ('INC1'   , r"[1-9][0-9]*"),
     ]
 )
```

### Comparing `bumpver-2022.1120/src/bumpver/v2rewrite.py` & `bumpver-2023.1121/src/bumpver/v2rewrite.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # This file is part of the bumpver project
 # https://github.com/mbarkhau/bumpver
 #
-# Copyright (c) 2018-2022 Manuel Barkhau (mbarkhau@gmail.com) - MIT License
+# Copyright (c) 2018-2023 Manuel Barkhau (mbarkhau@gmail.com) - MIT License
 # SPDX-License-Identifier: MIT
 """Rewrite files, updating occurences of version strings."""
 
 import io
 import typing as typ
 import logging
```

### Comparing `bumpver-2022.1120/src/bumpver/v2version.py` & `bumpver-2023.1121/src/bumpver/v2version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # This file is part of the bumpver project
 # https://github.com/mbarkhau/bumpver
 #
-# Copyright (c) 2018-2022 Manuel Barkhau (mbarkhau@gmail.com) - MIT License
+# Copyright (c) 2018-2023 Manuel Barkhau (mbarkhau@gmail.com) - MIT License
 # SPDX-License-Identifier: MIT
 """Functions related to version string manipulation."""
 
 import typing as typ
 import logging
 import datetime as dt
```

### Comparing `bumpver-2022.1120/src/bumpver/vcs.py` & `bumpver-2023.1121/src/bumpver/vcs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # This file is part of the bumpver project
 # https://github.com/mbarkhau/bumpver
 #
-# Copyright (c) 2018-2022 Manuel Barkhau (mbarkhau@gmail.com) - MIT License
+# Copyright (c) 2018-2023 Manuel Barkhau (mbarkhau@gmail.com) - MIT License
 # SPDX-License-Identifier: MIT
 #
 # bumpver/vcs.py (this file) is based on code from the
 # bumpversion project: https://github.com/peritus/bumpversion
 # Copyright (c) 2013-2014 Filip Noetzel - MIT License
 
 """Minimal Git and Mercirial API.
```

### Comparing `bumpver-2022.1120/src/bumpver/version.py` & `bumpver-2023.1121/src/bumpver/version.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 # This file is part of the bumpver project
 # https://github.com/mbarkhau/bumpver
 #
-# Copyright (c) 2018-2022 Manuel Barkhau (mbarkhau@gmail.com) - MIT License
+# Copyright (c) 2018-2023 Manuel Barkhau (mbarkhau@gmail.com) - MIT License
 # SPDX-License-Identifier: MIT
 import typing as typ
 import datetime as dt
 
 MaybeInt = typ.Optional[int]
 
 
 def parse_version(version: str) -> typ.Any:
     # pylint: disable=import-outside-toplevel; lazy import to speed up --help
-    import pkg_resources
 
-    return pkg_resources.parse_version(version)
+    try:
+        import pkg_resources
+
+        return pkg_resources.parse_version(version)
+    except (ImportError, ValueError):
+        import looseversion
+
+        return looseversion.LooseVersion(version)
 
 
 class V1CalendarInfo(typ.NamedTuple):
     """Container for calendar components of version strings."""
 
     year    : MaybeInt
     quarter : MaybeInt
```

### Comparing `bumpver-2022.1120/src/bumpver.egg-info/PKG-INFO` & `bumpver-2023.1121/src/bumpver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bumpver
-Version: 2022.1120
+Version: 2023.1121
 Summary: Bump version numbers in project files.
 Home-page: https://github.com/mbarkhau/bumpver
 Author: Manuel Barkhau
 Author-email: mbarkhau@gmail.com
 License: MIT
 Keywords: version bumpver calver semver versioning bumpversion pep440
 Classifier: Development Status :: 4 - Beta
@@ -47,15 +47,15 @@
 [url_calver_org]: https://calver.org/
 
 
 Project/Repo:
 
 [![MIT License][img_license]][url_license]
 [![Supported Python Versions][img_pyversions]][url_pyversions]
-[![CalVer 2022.1120][img_version]][url_version]
+[![CalVer 2023.1121][img_version]][url_version]
 [![PyPI Releases][img_pypi]][url_pypi]
 [![PyPI Downloads][img_downloads]][url_downloads]
 
 Code Quality/CI:
 
 [![GitHub Build Status][img_github_build]][url_github_build]
 [![GitLab Build Status][img_gitlab_build]][url_gitlab_build]
@@ -81,15 +81,15 @@
 
 [img_style]: https://img.shields.io/badge/code%20style-%20sjfmt-f71.svg
 [url_style]: https://gitlab.com/mbarkhau/straitjacket/
 
 [img_downloads]: https://pepy.tech/badge/bumpver/month
 [url_downloads]: https://pepy.tech/project/bumpver
 
-[img_version]: https://img.shields.io/static/v1.svg?label=CalVer&message=2022.1120&color=blue
+[img_version]: https://img.shields.io/static/v1.svg?label=CalVer&message=2023.1121&color=blue
 [url_version]: https://pypi.org/project/bumpver/
 
 [img_pypi]: https://img.shields.io/badge/PyPI-wheels-green.svg
 [url_pypi]: https://pypi.org/project/bumpver/#files
 
 [img_pyversions]: https://img.shields.io/pypi/pyversions/bumpver.svg
 [url_pyversions]: https://pypi.python.org/pypi/bumpver
@@ -634,15 +634,15 @@
   --date <ISODATE>                Set explicit date in format YYYY-0M-0D (e.g.
                                   2021-05-13).
   --pin-date                      Leave date components unchanged.
   --pin-increments                Leave the auto-increments INC0 and INC1
   --tag-num                       Increment release tag number (rc1, rc2,
                                   rc3..).
   -t, --tag <NAME>                Override release tag of current_version. Valid
-                                  options are: alpha, beta, rc, post, final.
+                                  options are: alpha, beta, dev, rc, post, final.
   -p, --patch                     Increment PATCH component.
   -m, --minor                     Increment MINOR component.
   --major                         Increment MAJOR component.
   -c, --commit-message <TMPL>     Set commit message template.
   --commit / --no-commit          Create a commit with all updated files.
   --tag-commit / --no-tag-commit  Tag the newly created commit.
   --push / --no-push              Push to the default remote.
@@ -669,30 +669,30 @@
 
 ### Part Overview
 
 > Where possible, these patterns match the conventions from [CalVer.org][url_calver_org_scheme].
 
 [url_calver_org_scheme]: https://calver.org/#scheme
 
-|    part    |     range / example(s)    |                     info                    |
-|------------|---------------------------|---------------------------------------------|
-| `MAJOR`    | 0..9, 10..99, 100..       | `bumpver update --major`                    |
-| `MINOR`    | 0..9, 10..99, 100..       | `bumpver update --minor`                    |
-| `PATCH`    | 0..9, 10..99, 100..       | `bumpver update --patch`                    |
-| `TAG`      | alpha, beta, rc, post     | `--tag=<tag>`                               |
-| `PYTAG`    | a, b, rc, post            | `--tag=<tag>`                               |
-| `NUM`      | 0, 1, 2...                | `-r/--tag-num`                              |
-| `YYYY`     | 2019, 2020...             | Full year, based on `strftime('%Y')`        |
-| `YY`       | 18, 19..99, 0, 1          | Short year, based on `int(strftime('%y'))`  |
-| `MM`       | 9, 10, 11, 12             | Month, based on `int(strftime('%m'))`       |
-| `DD`       | 1, 2, 3..31               | Day, based on `int(strftime('%d'))`         |
-| `BUILD`    | 1001, 1002 .. 1999, 22000 | build number (maintains lexical order)      |
-| `INC0`     | 0, 1, 2...                | 0-based auto incrementing number            |
-| `INC1`     | 1, 2...                   | 1-based auto incrementing number            |
-| `PYTAGNUM` | a0, a1, rc0, ...          | `PYTAG` + `NUM` (no white-space in between) |
+|    part    | range / example(s)         |                     info                    |
+|------------|----------------------------|---------------------------------------------|
+| `MAJOR`    | 0..9, 10..99, 100..        | `bumpver update --major`                    |
+| `MINOR`    | 0..9, 10..99, 100..        | `bumpver update --minor`                    |
+| `PATCH`    | 0..9, 10..99, 100..        | `bumpver update --patch`                    |
+| `TAG`      | dev, alpha, beta, rc, post | `--tag=<tag>`                               |
+| `PYTAG`    | a, b, rc, post             | `--tag=<tag>`                               |
+| `NUM`      | 0, 1, 2...                 | `-r/--tag-num`                              |
+| `YYYY`     | 2019, 2020...              | Full year, based on `strftime('%Y')`        |
+| `YY`       | 18, 19..99, 0, 1           | Short year, based on `int(strftime('%y'))`  |
+| `MM`       | 9, 10, 11, 12              | Month, based on `int(strftime('%m'))`       |
+| `DD`       | 1, 2, 3..31                | Day, based on `int(strftime('%d'))`         |
+| `BUILD`    | 1001, 1002 .. 1999, 22000  | build number (maintains lexical order)      |
+| `INC0`     | 0, 1, 2...                 | 0-based auto incrementing number            |
+| `INC1`     | 1, 2...                    | 1-based auto incrementing number            |
+| `PYTAGNUM` | a0, a1, rc0, ...           | `PYTAG` + `NUM` (no white-space in between) |
 
 
 The following are also available, but you should review the [Normalization Caveats](#normalization-caveats) before you decide to use them.
 
 
 | part   | range / example(s)  | comment                                      |
 | ------ | ------------------- | -------------------------------------------- |
@@ -821,15 +821,15 @@
 
 The create an initial configuration for project with `bumpver init`.
 
 ```shell
 $ pip install bumpver
 ...
 Installing collected packages: click toml lexid bumpver
-Successfully installed bumpver-2022.1120
+Successfully installed bumpver-2023.1121
 
 $ cd myproject
 ~/myproject/
 
 $ bumpver init --dry
 Exiting because of '-d/--dry'. Would have written to bumpver.toml:
 
@@ -1117,14 +1117,25 @@
 |                Name                 |    role           |  since  | until |
 |-------------------------------------|-------------------|---------|-------|
 | Manuel Barkhau (mbarkhau@gmail.com) | author/maintainer | 2018-09 | -     |
 
 
 # Changelog for https://github.com/mbarkhau/bumpver
 
+## BumpVer 2023.1121
+
+- Fix [#200][gh_i200]: Fix compatability with packaging 23.0.
+- Fix [#203][gh_i203]: Add dev to the list of valid release tags
+
+[gh_i200]: https://github.com/mbarkhau/bumpver/issues/200
+[gh_i203]: https://github.com/mbarkhau/bumpver/issues/203
+
+Thank you [Sharon Yogev](https://github.com/sharonyogev) for your contribution.
+
+
 ## BumpVer 2022.1120
 
 - Fix [#196][gh_i196]: Add `--pin-increments`.
 
 [gh_i196]: https://github.com/mbarkhau/bumpver/issues/196
 
 Thank you [Markus Holtermann](https://github.com/MarkusH) for
```

### Comparing `bumpver-2022.1120/src/bumpver.egg-info/SOURCES.txt` & `bumpver-2023.1121/src/bumpver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bumpver-2022.1120/test/test_cli.py` & `bumpver-2023.1121/test/test_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -254,14 +254,23 @@
     result = runner.invoke(
         cli.cli, ['test', "-vv", old_version, SEMVER, "--patch", "--tag", "beta"]
     )
     assert result.exit_code == 0
     assert f"Version: {new_version}\n" in result.output
 
 
+def test_dev_tag(runner):
+    old_version = "0.1.0"
+    new_version = "0.1.1dev0"
+
+    result = runner.invoke(cli.cli, ['test', "-vv", old_version, SEMVER, "--patch", "--tag", "dev"])
+    assert result.exit_code == 0
+    assert f"Version: {new_version}\n" in result.output
+
+
 def test_incr_tag_num(runner):
     old_version = "0.1.0b0"
     new_version = "0.1.0b1"
 
     result = runner.invoke(cli.cli, ['test', "-vv", old_version, SEMVER, "--tag-num"])
     assert result.exit_code == 0
     assert f"Version: {new_version}\n" in result.output
```

### Comparing `bumpver-2022.1120/test/test_config.py` & `bumpver-2023.1121/test/test_config.py`

 * *Files identical despite different names*

### Comparing `bumpver-2022.1120/test/test_parse.py` & `bumpver-2023.1121/test/test_parse.py`

 * *Files identical despite different names*

### Comparing `bumpver-2022.1120/test/test_patterns.py` & `bumpver-2023.1121/test/test_patterns.py`

 * *Files identical despite different names*

### Comparing `bumpver-2022.1120/test/test_rewrite.py` & `bumpver-2023.1121/test/test_rewrite.py`

 * *Files identical despite different names*

### Comparing `bumpver-2022.1120/test/test_version.py` & `bumpver-2023.1121/test/test_version.py`

 * *Files identical despite different names*

### Comparing `bumpver-2022.1120/test/util.py` & `bumpver-2023.1121/test/util.py`

 * *Files identical despite different names*

