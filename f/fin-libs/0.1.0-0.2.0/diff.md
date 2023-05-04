# Comparing `tmp/fin_libs-0.1.0.tar.gz` & `tmp/fin_libs-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fin_libs-0.1.0.tar", last modified: Sun Mar 26 02:31:39 2023, max compression
+gzip compressed data, was "fin_libs-0.2.0.tar", last modified: Thu May  4 06:10:13 2023, max compression
```

## Comparing `fin_libs-0.1.0.tar` & `fin_libs-0.2.0.tar`

### file list

```diff
@@ -1,40 +1,96 @@
-drwxr-xr-x   0 annezepecki   (501) staff       (20)        0 2023-03-26 02:31:39.542053 fin_libs-0.1.0/
--rw-r--r--   0 annezepecki   (501) staff       (20)      505 2023-03-26 01:44:48.000000 fin_libs-0.1.0/CONTRIBUTING.md
--rw-r--r--   0 annezepecki   (501) staff       (20)    11357 2023-02-19 01:44:34.000000 fin_libs-0.1.0/LICENSE
--rw-r--r--   0 annezepecki   (501) staff       (20)      379 2023-03-26 01:44:48.000000 fin_libs-0.1.0/MANIFEST.in
--rw-r--r--   0 annezepecki   (501) staff       (20)     1011 2023-03-26 01:44:48.000000 fin_libs-0.1.0/Makefile
--rw-r--r--   0 annezepecki   (501) staff       (20)    14307 2023-03-26 02:31:39.541903 fin_libs-0.1.0/PKG-INFO
--rw-r--r--   0 annezepecki   (501) staff       (20)     1021 2023-03-26 01:44:48.000000 fin_libs-0.1.0/README.md
--rw-r--r--   0 annezepecki   (501) staff       (20)     1186 2023-03-26 02:30:01.000000 fin_libs-0.1.0/pyproject.toml
--rw-r--r--   0 annezepecki   (501) staff       (20)       38 2023-03-26 02:31:39.542086 fin_libs-0.1.0/setup.cfg
--rw-r--r--   0 annezepecki   (501) staff       (20)       38 2023-03-10 01:23:55.000000 fin_libs-0.1.0/setup.py
-drwxr-xr-x   0 annezepecki   (501) staff       (20)        0 2023-03-26 02:31:39.539376 fin_libs-0.1.0/src/
-drwxr-xr-x   0 annezepecki   (501) staff       (20)        0 2023-03-26 02:31:39.539536 fin_libs-0.1.0/src/fin_libs/
--rw-r--r--   0 annezepecki   (501) staff       (20)      773 2023-03-26 01:44:48.000000 fin_libs-0.1.0/src/fin_libs/__init__.py
-drwxr-xr-x   0 annezepecki   (501) staff       (20)        0 2023-03-26 02:31:39.540176 fin_libs-0.1.0/src/fin_libs/compound_annual_growth_rate/
--rw-r--r--   0 annezepecki   (501) staff       (20)      597 2023-03-10 01:23:55.000000 fin_libs-0.1.0/src/fin_libs/compound_annual_growth_rate/__init__.py
-drwxr-xr-x   0 annezepecki   (501) staff       (20)        0 2023-03-26 02:31:39.540381 fin_libs-0.1.0/src/fin_libs/dividends/
--rw-r--r--   0 annezepecki   (501) staff       (20)      529 2023-03-10 01:23:55.000000 fin_libs-0.1.0/src/fin_libs/dividends/__init__.py
-drwxr-xr-x   0 annezepecki   (501) staff       (20)        0 2023-03-26 02:31:39.540555 fin_libs-0.1.0/src/fin_libs/eps/
--rw-r--r--   0 annezepecki   (501) staff       (20)      315 2023-03-10 01:23:55.000000 fin_libs-0.1.0/src/fin_libs/eps/__init__.py
-drwxr-xr-x   0 annezepecki   (501) staff       (20)        0 2023-03-26 02:31:39.540713 fin_libs-0.1.0/src/fin_libs/income/
--rw-r--r--   0 annezepecki   (501) staff       (20)      451 2023-03-10 01:23:55.000000 fin_libs-0.1.0/src/fin_libs/income/__init__.py
-drwxr-xr-x   0 annezepecki   (501) staff       (20)        0 2023-03-26 02:31:39.540862 fin_libs-0.1.0/src/fin_libs/interest/
--rw-r--r--   0 annezepecki   (501) staff       (20)      127 2023-03-26 01:44:48.000000 fin_libs-0.1.0/src/fin_libs/interest/__init__.py
-drwxr-xr-x   0 annezepecki   (501) staff       (20)        0 2023-03-26 02:31:39.540989 fin_libs-0.1.0/src/fin_libs/interest/compound/
--rw-r--r--   0 annezepecki   (501) staff       (20)      420 2023-03-10 01:23:55.000000 fin_libs-0.1.0/src/fin_libs/interest/compound/__init__.py
-drwxr-xr-x   0 annezepecki   (501) staff       (20)        0 2023-03-26 02:31:39.541098 fin_libs-0.1.0/src/fin_libs/interest/simple/
--rw-r--r--   0 annezepecki   (501) staff       (20)      369 2023-03-10 01:23:55.000000 fin_libs-0.1.0/src/fin_libs/interest/simple/__init__.py
-drwxr-xr-x   0 annezepecki   (501) staff       (20)        0 2023-03-26 02:31:39.541274 fin_libs-0.1.0/src/fin_libs/linear_least_squares/
--rw-r--r--   0 annezepecki   (501) staff       (20)      706 2023-03-26 01:44:48.000000 fin_libs-0.1.0/src/fin_libs/linear_least_squares/__init__.py
-drwxr-xr-x   0 annezepecki   (501) staff       (20)        0 2023-03-26 02:31:39.541446 fin_libs-0.1.0/src/fin_libs/price/
--rw-r--r--   0 annezepecki   (501) staff       (20)      610 2023-03-10 01:23:55.000000 fin_libs-0.1.0/src/fin_libs/price/__init__.py
-drwxr-xr-x   0 annezepecki   (501) staff       (20)        0 2023-03-26 02:31:39.541668 fin_libs-0.1.0/src/fin_libs/weighted_average/
--rw-r--r--   0 annezepecki   (501) staff       (20)      713 2023-03-26 01:44:48.000000 fin_libs-0.1.0/src/fin_libs/weighted_average/__init__.py
-drwxr-xr-x   0 annezepecki   (501) staff       (20)        0 2023-03-26 02:31:39.540075 fin_libs-0.1.0/src/fin_libs.egg-info/
--rw-r--r--   0 annezepecki   (501) staff       (20)    14307 2023-03-26 02:31:39.000000 fin_libs-0.1.0/src/fin_libs.egg-info/PKG-INFO
--rw-r--r--   0 annezepecki   (501) staff       (20)      680 2023-03-26 02:31:39.000000 fin_libs-0.1.0/src/fin_libs.egg-info/SOURCES.txt
--rw-r--r--   0 annezepecki   (501) staff       (20)        1 2023-03-26 02:31:39.000000 fin_libs-0.1.0/src/fin_libs.egg-info/dependency_links.txt
--rw-r--r--   0 annezepecki   (501) staff       (20)      173 2023-03-26 02:31:39.000000 fin_libs-0.1.0/src/fin_libs.egg-info/requires.txt
--rw-r--r--   0 annezepecki   (501) staff       (20)       14 2023-03-26 02:31:39.000000 fin_libs-0.1.0/src/fin_libs.egg-info/top_level.txt
--rw-r--r--   0 annezepecki   (501) staff       (20)     3253 2023-03-26 01:44:48.000000 fin_libs-0.1.0/src/test.py
+drwxr-xr-x   0 annezepecki   (501) staff       (20)        0 2023-05-04 06:10:13.217594 fin_libs-0.2.0/
+-rw-r--r--   0 annezepecki   (501) staff       (20)      505 2023-04-05 02:25:57.000000 fin_libs-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0 annezepecki   (501) staff       (20)    11357 2023-04-05 02:25:57.000000 fin_libs-0.2.0/LICENSE
+-rw-r--r--   0 annezepecki   (501) staff       (20)      938 2023-04-05 02:25:57.000000 fin_libs-0.2.0/MANIFEST.in
+-rw-r--r--   0 annezepecki   (501) staff       (20)     1011 2023-04-05 02:25:57.000000 fin_libs-0.2.0/Makefile
+-rw-r--r--   0 annezepecki   (501) staff       (20)    14638 2023-05-04 06:10:13.217415 fin_libs-0.2.0/PKG-INFO
+-rw-r--r--   0 annezepecki   (501) staff       (20)     1352 2023-05-04 06:00:26.000000 fin_libs-0.2.0/README.md
+drwxr-xr-x   0 annezepecki   (501) staff       (20)        0 2023-05-04 06:10:13.209796 fin_libs-0.2.0/docs/
+-rw-r--r--   0 annezepecki   (501) staff       (20)      230 2023-04-05 02:25:57.000000 fin_libs-0.2.0/docs/.buildinfo
+drwxr-xr-x   0 annezepecki   (501) staff       (20)        0 2023-05-04 06:10:13.210644 fin_libs-0.2.0/docs/.doctrees/
+drwxr-xr-x   0 annezepecki   (501) staff       (20)        0 2023-05-04 06:10:13.204940 fin_libs-0.2.0/docs/.doctrees/.github/
+drwxr-xr-x   0 annezepecki   (501) staff       (20)        0 2023-05-04 06:10:13.210914 fin_libs-0.2.0/docs/.doctrees/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 annezepecki   (501) staff       (20)     9337 2023-04-05 02:25:57.000000 fin_libs-0.2.0/docs/.doctrees/.github/ISSUE_TEMPLATE/bug_report.doctree
+-rw-r--r--   0 annezepecki   (501) staff       (20)     5693 2023-04-05 02:25:57.000000 fin_libs-0.2.0/docs/.doctrees/.github/ISSUE_TEMPLATE/feature_request.doctree
+-rw-r--r--   0 annezepecki   (501) staff       (20)     5885 2023-04-05 02:25:57.000000 fin_libs-0.2.0/docs/.doctrees/CONTRIBUTING.doctree
+-rw-r--r--   0 annezepecki   (501) staff       (20)     7304 2023-04-05 02:25:57.000000 fin_libs-0.2.0/docs/.doctrees/README.doctree
+drwxr-xr-x   0 annezepecki   (501) staff       (20)        0 2023-05-04 06:10:13.211054 fin_libs-0.2.0/docs/.doctrees/docs/
+drwxr-xr-x   0 annezepecki   (501) staff       (20)        0 2023-05-04 06:10:13.205096 fin_libs-0.2.0/docs/.doctrees/docs/_build/
+drwxr-xr-x   0 annezepecki   (501) staff       (20)        0 2023-05-04 06:10:13.211191 fin_libs-0.2.0/docs/.doctrees/docs/_build/markdown/
+-rw-r--r--   0 annezepecki   (501) staff       (20)     4280 2023-04-05 02:25:57.000000 fin_libs-0.2.0/docs/.doctrees/docs/_build/markdown/index.doctree
+-rw-r--r--   0 annezepecki   (501) staff       (20)     4097 2023-04-05 02:25:57.000000 fin_libs-0.2.0/docs/.doctrees/docs/index.doctree
+-rw-r--r--   0 annezepecki   (501) staff       (20)    67920 2023-04-05 02:25:57.000000 fin_libs-0.2.0/docs/.doctrees/environment.pickle
+-rw-r--r--   0 annezepecki   (501) staff       (20)     4082 2023-04-05 02:25:57.000000 fin_libs-0.2.0/docs/.doctrees/index.doctree
+drwxr-xr-x   0 annezepecki   (501) staff       (20)        0 2023-05-04 06:10:13.205195 fin_libs-0.2.0/docs/.github/
+drwxr-xr-x   0 annezepecki   (501) staff       (20)        0 2023-05-04 06:10:13.211461 fin_libs-0.2.0/docs/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 annezepecki   (501) staff       (20)     4665 2023-04-05 02:25:57.000000 fin_libs-0.2.0/docs/.github/ISSUE_TEMPLATE/bug_report.html
+-rw-r--r--   0 annezepecki   (501) staff       (20)     4149 2023-04-05 02:25:57.000000 fin_libs-0.2.0/docs/.github/ISSUE_TEMPLATE/feature_request.html
+-rw-r--r--   0 annezepecki   (501) staff       (20)     5255 2023-04-05 02:25:57.000000 fin_libs-0.2.0/docs/CONTRIBUTING.html
+-rw-r--r--   0 annezepecki   (501) staff       (20)      634 2023-04-05 02:25:57.000000 fin_libs-0.2.0/docs/Makefile
+-rw-r--r--   0 annezepecki   (501) staff       (20)     5624 2023-04-05 02:25:57.000000 fin_libs-0.2.0/docs/README.html
+drwxr-xr-x   0 annezepecki   (501) staff       (20)        0 2023-05-04 06:10:13.211952 fin_libs-0.2.0/docs/_sources/
+drwxr-xr-x   0 annezepecki   (501) staff       (20)        0 2023-05-04 06:10:13.205337 fin_libs-0.2.0/docs/_sources/.github/
+drwxr-xr-x   0 annezepecki   (501) staff       (20)        0 2023-05-04 06:10:13.212256 fin_libs-0.2.0/docs/_sources/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 annezepecki   (501) staff       (20)      834 2023-04-05 02:25:57.000000 fin_libs-0.2.0/docs/_sources/.github/ISSUE_TEMPLATE/bug_report.md.txt
+-rw-r--r--   0 annezepecki   (501) staff       (20)      595 2023-04-05 02:25:57.000000 fin_libs-0.2.0/docs/_sources/.github/ISSUE_TEMPLATE/feature_request.md.txt
+-rw-r--r--   0 annezepecki   (501) staff       (20)      505 2023-04-05 02:25:57.000000 fin_libs-0.2.0/docs/_sources/CONTRIBUTING.md.txt
+-rw-r--r--   0 annezepecki   (501) staff       (20)     1104 2023-04-05 02:25:57.000000 fin_libs-0.2.0/docs/_sources/README.md.txt
+drwxr-xr-x   0 annezepecki   (501) staff       (20)        0 2023-05-04 06:10:13.205429 fin_libs-0.2.0/docs/_sources/docs/
+drwxr-xr-x   0 annezepecki   (501) staff       (20)        0 2023-05-04 06:10:13.205470 fin_libs-0.2.0/docs/_sources/docs/_build/
+drwxr-xr-x   0 annezepecki   (501) staff       (20)        0 2023-05-04 06:10:13.212394 fin_libs-0.2.0/docs/_sources/docs/_build/markdown/
+-rw-r--r--   0 annezepecki   (501) staff       (20)      145 2023-04-05 02:25:57.000000 fin_libs-0.2.0/docs/_sources/docs/_build/markdown/index.md.txt
+-rw-r--r--   0 annezepecki   (501) staff       (20)      234 2023-04-05 02:25:57.000000 fin_libs-0.2.0/docs/_sources/index.rst.txt
+-rw-r--r--   0 annezepecki   (501) staff       (20)     1453 2023-04-05 02:25:57.000000 fin_libs-0.2.0/docs/conf.py
+drwxr-xr-x   0 annezepecki   (501) staff       (20)        0 2023-05-04 06:10:13.213456 fin_libs-0.2.0/docs/docs/
+-rw-r--r--   0 annezepecki   (501) staff       (20)      230 2023-04-05 02:25:57.000000 fin_libs-0.2.0/docs/docs/.buildinfo
+drwxr-xr-x   0 annezepecki   (501) staff       (20)        0 2023-05-04 06:10:13.214135 fin_libs-0.2.0/docs/docs/.doctrees/
+-rw-r--r--   0 annezepecki   (501) staff       (20)   129714 2023-04-05 02:25:57.000000 fin_libs-0.2.0/docs/docs/.doctrees/environment.pickle
+-rw-r--r--   0 annezepecki   (501) staff       (20)    76804 2023-04-05 02:25:57.000000 fin_libs-0.2.0/docs/docs/.doctrees/index.doctree
+drwxr-xr-x   0 annezepecki   (501) staff       (20)        0 2023-05-04 06:10:13.214420 fin_libs-0.2.0/docs/docs/_sources/
+-rw-r--r--   0 annezepecki   (501) staff       (20)     1400 2023-04-05 02:25:57.000000 fin_libs-0.2.0/docs/docs/_sources/index.rst.txt
+-rw-r--r--   0 annezepecki   (501) staff       (20)     8724 2023-04-05 02:25:57.000000 fin_libs-0.2.0/docs/docs/genindex.html
+-rw-r--r--   0 annezepecki   (501) staff       (20)    28994 2023-04-05 02:25:57.000000 fin_libs-0.2.0/docs/docs/index.html
+-rw-r--r--   0 annezepecki   (501) staff       (20)      506 2023-04-05 02:25:57.000000 fin_libs-0.2.0/docs/docs/objects.inv
+-rw-r--r--   0 annezepecki   (501) staff       (20)     5680 2023-04-05 02:25:57.000000 fin_libs-0.2.0/docs/docs/py-modindex.html
+-rw-r--r--   0 annezepecki   (501) staff       (20)     3597 2023-04-05 02:25:57.000000 fin_libs-0.2.0/docs/docs/search.html
+-rw-r--r--   0 annezepecki   (501) staff       (20)     7313 2023-04-05 02:25:57.000000 fin_libs-0.2.0/docs/docs/searchindex.js
+-rw-r--r--   0 annezepecki   (501) staff       (20)     3130 2023-04-05 02:25:57.000000 fin_libs-0.2.0/docs/genindex.html
+-rw-r--r--   0 annezepecki   (501) staff       (20)     4044 2023-04-05 02:25:57.000000 fin_libs-0.2.0/docs/index.html
+-rw-r--r--   0 annezepecki   (501) staff       (20)     1400 2023-04-05 02:25:57.000000 fin_libs-0.2.0/docs/index.rst
+-rw-r--r--   0 annezepecki   (501) staff       (20)      800 2023-04-05 02:25:57.000000 fin_libs-0.2.0/docs/make.bat
+-rw-r--r--   0 annezepecki   (501) staff       (20)      419 2023-04-05 02:25:57.000000 fin_libs-0.2.0/docs/objects.inv
+-rw-r--r--   0 annezepecki   (501) staff       (20)     3529 2023-04-05 02:25:57.000000 fin_libs-0.2.0/docs/search.html
+-rw-r--r--   0 annezepecki   (501) staff       (20)     4456 2023-04-05 02:25:57.000000 fin_libs-0.2.0/docs/searchindex.js
+-rw-r--r--   0 annezepecki   (501) staff       (20)     1186 2023-05-04 06:07:13.000000 fin_libs-0.2.0/pyproject.toml
+-rw-r--r--   0 annezepecki   (501) staff       (20)       38 2023-05-04 06:10:13.217641 fin_libs-0.2.0/setup.cfg
+-rw-r--r--   0 annezepecki   (501) staff       (20)       38 2023-04-05 02:25:57.000000 fin_libs-0.2.0/setup.py
+drwxr-xr-x   0 annezepecki   (501) staff       (20)        0 2023-05-04 06:10:13.214569 fin_libs-0.2.0/src/
+drwxr-xr-x   0 annezepecki   (501) staff       (20)        0 2023-05-04 06:10:13.214828 fin_libs-0.2.0/src/fin_libs/
+-rw-r--r--   0 annezepecki   (501) staff       (20)      773 2023-04-05 02:25:57.000000 fin_libs-0.2.0/src/fin_libs/__init__.py
+drwxr-xr-x   0 annezepecki   (501) staff       (20)        0 2023-05-04 06:10:13.215521 fin_libs-0.2.0/src/fin_libs/compound_annual_growth_rate/
+-rw-r--r--   0 annezepecki   (501) staff       (20)      961 2023-04-05 02:25:57.000000 fin_libs-0.2.0/src/fin_libs/compound_annual_growth_rate/__init__.py
+drwxr-xr-x   0 annezepecki   (501) staff       (20)        0 2023-05-04 06:10:13.215656 fin_libs-0.2.0/src/fin_libs/dividends/
+-rw-r--r--   0 annezepecki   (501) staff       (20)      658 2023-04-05 02:25:57.000000 fin_libs-0.2.0/src/fin_libs/dividends/__init__.py
+drwxr-xr-x   0 annezepecki   (501) staff       (20)        0 2023-05-04 06:10:13.215791 fin_libs-0.2.0/src/fin_libs/eps/
+-rw-r--r--   0 annezepecki   (501) staff       (20)      404 2023-04-05 02:25:57.000000 fin_libs-0.2.0/src/fin_libs/eps/__init__.py
+drwxr-xr-x   0 annezepecki   (501) staff       (20)        0 2023-05-04 06:10:13.216016 fin_libs-0.2.0/src/fin_libs/income/
+-rw-r--r--   0 annezepecki   (501) staff       (20)      582 2023-04-05 02:25:57.000000 fin_libs-0.2.0/src/fin_libs/income/__init__.py
+drwxr-xr-x   0 annezepecki   (501) staff       (20)        0 2023-05-04 06:10:13.216159 fin_libs-0.2.0/src/fin_libs/interest/
+-rw-r--r--   0 annezepecki   (501) staff       (20)      127 2023-04-05 02:25:57.000000 fin_libs-0.2.0/src/fin_libs/interest/__init__.py
+drwxr-xr-x   0 annezepecki   (501) staff       (20)        0 2023-05-04 06:10:13.216323 fin_libs-0.2.0/src/fin_libs/interest/compound/
+-rw-r--r--   0 annezepecki   (501) staff       (20)      531 2023-04-05 02:25:57.000000 fin_libs-0.2.0/src/fin_libs/interest/compound/__init__.py
+drwxr-xr-x   0 annezepecki   (501) staff       (20)        0 2023-05-04 06:10:13.216609 fin_libs-0.2.0/src/fin_libs/interest/simple/
+-rw-r--r--   0 annezepecki   (501) staff       (20)      477 2023-04-05 02:25:57.000000 fin_libs-0.2.0/src/fin_libs/interest/simple/__init__.py
+drwxr-xr-x   0 annezepecki   (501) staff       (20)        0 2023-05-04 06:10:13.216770 fin_libs-0.2.0/src/fin_libs/linear_least_squares/
+-rw-r--r--   0 annezepecki   (501) staff       (20)     1282 2023-04-05 02:25:57.000000 fin_libs-0.2.0/src/fin_libs/linear_least_squares/__init__.py
+drwxr-xr-x   0 annezepecki   (501) staff       (20)        0 2023-05-04 06:10:13.216934 fin_libs-0.2.0/src/fin_libs/price/
+-rw-r--r--   0 annezepecki   (501) staff       (20)      784 2023-04-05 02:25:57.000000 fin_libs-0.2.0/src/fin_libs/price/__init__.py
+drwxr-xr-x   0 annezepecki   (501) staff       (20)        0 2023-05-04 06:10:13.217118 fin_libs-0.2.0/src/fin_libs/weighted_average/
+-rw-r--r--   0 annezepecki   (501) staff       (20)     1010 2023-04-05 02:25:57.000000 fin_libs-0.2.0/src/fin_libs/weighted_average/__init__.py
+drwxr-xr-x   0 annezepecki   (501) staff       (20)        0 2023-05-04 06:10:13.215406 fin_libs-0.2.0/src/fin_libs.egg-info/
+-rw-r--r--   0 annezepecki   (501) staff       (20)    14638 2023-05-04 06:10:12.000000 fin_libs-0.2.0/src/fin_libs.egg-info/PKG-INFO
+-rw-r--r--   0 annezepecki   (501) staff       (20)     1827 2023-05-04 06:10:13.000000 fin_libs-0.2.0/src/fin_libs.egg-info/SOURCES.txt
+-rw-r--r--   0 annezepecki   (501) staff       (20)        1 2023-05-04 06:10:12.000000 fin_libs-0.2.0/src/fin_libs.egg-info/dependency_links.txt
+-rw-r--r--   0 annezepecki   (501) staff       (20)      173 2023-05-04 06:10:13.000000 fin_libs-0.2.0/src/fin_libs.egg-info/requires.txt
+-rw-r--r--   0 annezepecki   (501) staff       (20)       14 2023-05-04 06:10:13.000000 fin_libs-0.2.0/src/fin_libs.egg-info/top_level.txt
+-rw-r--r--   0 annezepecki   (501) staff       (20)     3253 2023-04-05 02:25:57.000000 fin_libs-0.2.0/src/test.py
```

### Comparing `fin_libs-0.1.0/LICENSE` & `fin_libs-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fin_libs-0.1.0/Makefile` & `fin_libs-0.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `fin_libs-0.1.0/PKG-INFO` & `fin_libs-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fin_libs
-Version: 0.1.0
+Version: 0.2.0
 Summary: Python library that exposes tools for financial analytics
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -213,27 +213,30 @@
 
 # fin-libs
 Financial analytics toolkit
 
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0) ![Issues](https://img.shields.io/github/issues/azepecki/fin-libs)
 [![Build Status](https://github.com/ColumbiaOSS/example-project-python/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/azepecki/fin-libs/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/azepecki/fin-libs/branch/main/graph/badge.svg)](https://codecov.io/gh/azepecki/fin-libs)
+[![PyPI](https://img.shields.io/pypi/v/numpy)](https://pypi.org/project/fin-libs/)
+[![Docs](https://inch-ci.org/github/dwyl/hapi-auth-jwt2.svg?branch=master)](https://azepecki.github.io/fin-libs/)
 
 
 ## Overview
 
-Python library that exposes tools for financial analytics. This includs functions to:
+Python library that exposes tools for financial analytics. This includes functions to:
 - calculate simple and compound interest
 - compound annual growth rate 
 - weighted average
 - linear least squares
 - earning per share
 - net income
 
 ## Installation
 
-This library can be installed by running `pip install fin_libs`
+This library can be installed by running `pip install fin_libs`. This will pull the latest version of the library.
 
 ## Usage
 
-This library is meant to be used for financial analytics purposes. You can import specific functionality from modules in the library. 
+This library is meant to be used for financial analytics purposes. You can import specific functionality from modules in the library. Example usage of each module can be found at the documentation site linked above.
+
```

### Comparing `fin_libs-0.1.0/README.md` & `fin_libs-0.2.0/docs/_sources/README.md.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # fin-libs
 Financial analytics toolkit
 
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0) ![Issues](https://img.shields.io/github/issues/azepecki/fin-libs)
 [![Build Status](https://github.com/ColumbiaOSS/example-project-python/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/azepecki/fin-libs/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/azepecki/fin-libs/branch/main/graph/badge.svg)](https://codecov.io/gh/azepecki/fin-libs)
+[![PyPI](https://img.shields.io/pypi/v/numpy)](https://pypi.org/project/fin-libs/)
 
 
 ## Overview
 
 Python library that exposes tools for financial analytics. This includs functions to:
 - calculate simple and compound interest
 - compound annual growth rate
```

### Comparing `fin_libs-0.1.0/pyproject.toml` & `fin_libs-0.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "fin_libs"
 description = "Python library that exposes tools for financial analytics"
 readme = "README.md"
-version = "0.1.0"
+version = "0.2.0"
 requires-python = ">=3.9"
 
 dependencies = [
         "matplotlib",
         "pandas",
         "scikit-learn",
         "yfinance",
```

### Comparing `fin_libs-0.1.0/src/fin_libs/__init__.py` & `fin_libs-0.2.0/src/fin_libs/__init__.py`

 * *Files identical despite different names*

### Comparing `fin_libs-0.1.0/src/fin_libs/compound_annual_growth_rate/__init__.py` & `fin_libs-0.2.0/src/fin_libs/compound_annual_growth_rate/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,37 @@
 """
 Library module to compute compund annual growth rate
-"""
 
-"""
-Calculate compound annaul growth rate
+Typical usage example:
 
-Args:
-        first(float): starting value
-        last(float): ending value
-        years(int): number of years
+    rate = calculate_compound_annual_growth_rate(71, 100, 4)
 """
 
 
 def calculate_compound_annual_growth_rate(first, last, years):
+    """
+    Calculate compound annual growth rate
+
+    Args:
+        first (float): starting value
+        last (float): ending value
+        years (int): number of years
+
+    Returns:
+        float: calculated compound annual growth rate"""
     if years < 1:
         raise Exception("Years cannot be less than 1")
     return ((last / first) ** (1 / years) - 1) * 100
 
 
 def print_calculate_compound_annual_growth_rate(first, last, years):
+    """
+    Print compound annaul growth rate
+
+    Args:
+        first (float): starting value
+        last (float): ending value
+        years (int): number of years
+
+    Returns:
+        None"""
     print(f"Compound annual growth rate: {round(calculate_compound_annual_growth_rate(first, last, years), 2)}")
```

### Comparing `fin_libs-0.1.0/src/fin_libs/weighted_average/__init__.py` & `fin_libs-0.2.0/src/fin_libs/weighted_average/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 """
 Library package to compute the weighted average
-"""
-import numpy
-import pandas
 
-"""
-Compute weighted average
+Typical usage example:
 
-Args:
-        csv_file_path(str): file path string
-        distr_col(str): column name for distribution
-        weights_col(str): column name for weights
-Returns:
-        int: weighted average
+    weighted_avg = compute_weighted_average("data.csv", "values", "weights")
 """
+import numpy
+import pandas
 
 
 def compute_weighted_average(csv_file_path, distr_col, weights_col):
+    """
+    Compute weighted average
+
+    Args:
+            csv_file_path (str): file path string
+            distr_col (str): column name for distribution
+            weights_col (str): column name for weights
+    Returns:
+            int: weighted average"""
     df = pandas.read_csv(csv_file_path)
     distribution = df[distr_col]
     weights = df[weights_col]
     return _compute_weighted_average(distribution, weights)
 
 
-"""
-Helper function to calculate weighted average
-"""
-
-
 def _compute_weighted_average(distribution, weights):
+    """
+    Helper function to calculate weighted average
+
+    Args:
+            distribution (list): list of values
+            weights (list): weights for each value
+    Returns:
+            int: weighted average"""
     return numpy.average(distribution, weights=weights)
```

### Comparing `fin_libs-0.1.0/src/fin_libs.egg-info/PKG-INFO` & `fin_libs-0.2.0/src/fin_libs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fin-libs
-Version: 0.1.0
+Version: 0.2.0
 Summary: Python library that exposes tools for financial analytics
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -213,27 +213,30 @@
 
 # fin-libs
 Financial analytics toolkit
 
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0) ![Issues](https://img.shields.io/github/issues/azepecki/fin-libs)
 [![Build Status](https://github.com/ColumbiaOSS/example-project-python/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/azepecki/fin-libs/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/azepecki/fin-libs/branch/main/graph/badge.svg)](https://codecov.io/gh/azepecki/fin-libs)
+[![PyPI](https://img.shields.io/pypi/v/numpy)](https://pypi.org/project/fin-libs/)
+[![Docs](https://inch-ci.org/github/dwyl/hapi-auth-jwt2.svg?branch=master)](https://azepecki.github.io/fin-libs/)
 
 
 ## Overview
 
-Python library that exposes tools for financial analytics. This includs functions to:
+Python library that exposes tools for financial analytics. This includes functions to:
 - calculate simple and compound interest
 - compound annual growth rate 
 - weighted average
 - linear least squares
 - earning per share
 - net income
 
 ## Installation
 
-This library can be installed by running `pip install fin_libs`
+This library can be installed by running `pip install fin_libs`. This will pull the latest version of the library.
 
 ## Usage
 
-This library is meant to be used for financial analytics purposes. You can import specific functionality from modules in the library. 
+This library is meant to be used for financial analytics purposes. You can import specific functionality from modules in the library. Example usage of each module can be found at the documentation site linked above.
+
```

### Comparing `fin_libs-0.1.0/src/test.py` & `fin_libs-0.2.0/src/test.py`

 * *Files identical despite different names*

