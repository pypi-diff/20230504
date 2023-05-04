# Comparing `tmp/pyobjectify-0.1.1.tar.gz` & `tmp/pyobjectify-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjectify-0.1.1.tar", last modified: Sun Mar 26 06:57:17 2023, max compression
+gzip compressed data, was "pyobjectify-0.2.1.tar", last modified: Thu May  4 03:21:33 2023, max compression
```

## Comparing `pyobjectify-0.1.1.tar` & `pyobjectify-0.2.1.tar`

### file list

```diff
@@ -1,32 +1,105 @@
-drwxr-xr-x   0 rjw        (501) staff       (20)        0 2023-03-26 06:57:17.135126 pyobjectify-0.1.1/
--rw-r--r--   0 rjw        (501) staff       (20)      404 2023-03-26 06:44:00.000000 pyobjectify-0.1.1/.bumpversion.cfg
--rw-r--r--   0 rjw        (501) staff       (20)     2540 2023-03-26 06:44:00.000000 pyobjectify-0.1.1/CONTRIBUTING.md
--rw-r--r--   0 rjw        (501) staff       (20)     1067 2023-03-26 06:05:28.000000 pyobjectify-0.1.1/LICENSE
--rw-r--r--   0 rjw        (501) staff       (20)      580 2023-03-26 06:44:00.000000 pyobjectify-0.1.1/MANIFEST.in
--rw-r--r--   0 rjw        (501) staff       (20)     2525 2023-03-26 06:44:00.000000 pyobjectify-0.1.1/Makefile
--rw-r--r--   0 rjw        (501) staff       (20)     4262 2023-03-26 06:57:17.134896 pyobjectify-0.1.1/PKG-INFO
--rw-r--r--   0 rjw        (501) staff       (20)     2113 2023-03-26 06:44:00.000000 pyobjectify-0.1.1/README.md
--rw-r--r--   0 rjw        (501) staff       (20)      112 2023-03-26 06:44:00.000000 pyobjectify-0.1.1/codecov.yml
-drwxr-xr-x   0 rjw        (501) staff       (20)        0 2023-03-26 06:57:17.129373 pyobjectify-0.1.1/pyobjectify/
--rw-r--r--   0 rjw        (501) staff       (20)      265 2023-03-26 06:44:00.000000 pyobjectify-0.1.1/pyobjectify/__init__.py
--rw-r--r--   0 rjw        (501) staff       (20)       22 2023-03-26 06:44:00.000000 pyobjectify-0.1.1/pyobjectify/_version.py
--rw-r--r--   0 rjw        (501) staff       (20)    10449 2023-03-26 06:44:00.000000 pyobjectify-0.1.1/pyobjectify/pyobjectify.py
-drwxr-xr-x   0 rjw        (501) staff       (20)        0 2023-03-26 06:57:17.131564 pyobjectify-0.1.1/pyobjectify/tests/
-drwxr-xr-x   0 rjw        (501) staff       (20)        0 2023-03-26 06:57:17.134221 pyobjectify-0.1.1/pyobjectify/tests/data/
--rw-r--r--   0 rjw        (501) staff       (20)       21 2023-03-26 06:44:00.000000 pyobjectify-0.1.1/pyobjectify/tests/data/data.example
--rw-r--r--   0 rjw        (501) staff       (20)     3291 2023-03-26 06:05:28.000000 pyobjectify-0.1.1/pyobjectify/tests/data/example.csv
--rw-r--r--   0 rjw        (501) staff       (20)      330 2023-03-26 06:44:00.000000 pyobjectify-0.1.1/pyobjectify/tests/data/example.json
--rw-r--r--   0 rjw        (501) staff       (20)     3218 2023-03-26 06:05:28.000000 pyobjectify-0.1.1/pyobjectify/tests/data/example.tsv
--rw-r--r--   0 rjw        (501) staff       (20)     9495 2023-03-26 06:05:28.000000 pyobjectify-0.1.1/pyobjectify/tests/data/example.xml
--rw-r--r--   0 rjw        (501) staff       (20)      936 2023-03-26 06:05:28.000000 pyobjectify-0.1.1/pyobjectify/tests/data/test.json
--rw-r--r--   0 rjw        (501) staff       (20)     1983 2023-03-26 06:44:00.000000 pyobjectify-0.1.1/pyobjectify/tests/test_integration.py
--rw-r--r--   0 rjw        (501) staff       (20)    43016 2023-03-26 06:44:00.000000 pyobjectify-0.1.1/pyobjectify/tests/test_unit.py
-drwxr-xr-x   0 rjw        (501) staff       (20)        0 2023-03-26 06:57:17.130994 pyobjectify-0.1.1/pyobjectify.egg-info/
--rw-r--r--   0 rjw        (501) staff       (20)     4262 2023-03-26 06:57:17.000000 pyobjectify-0.1.1/pyobjectify.egg-info/PKG-INFO
--rw-r--r--   0 rjw        (501) staff       (20)      635 2023-03-26 06:57:17.000000 pyobjectify-0.1.1/pyobjectify.egg-info/SOURCES.txt
--rw-r--r--   0 rjw        (501) staff       (20)        1 2023-03-26 06:57:17.000000 pyobjectify-0.1.1/pyobjectify.egg-info/dependency_links.txt
--rw-r--r--   0 rjw        (501) staff       (20)      392 2023-03-26 06:57:17.000000 pyobjectify-0.1.1/pyobjectify.egg-info/requires.txt
--rw-r--r--   0 rjw        (501) staff       (20)       12 2023-03-26 06:57:17.000000 pyobjectify-0.1.1/pyobjectify.egg-info/top_level.txt
--rw-r--r--   0 rjw        (501) staff       (20)     2567 2023-03-26 06:44:00.000000 pyobjectify-0.1.1/pyproject.toml
--rw-r--r--   0 rjw        (501) staff       (20)       38 2023-03-26 06:57:17.135206 pyobjectify-0.1.1/setup.cfg
--rw-r--r--   0 rjw        (501) staff       (20)       57 2023-03-26 06:44:00.000000 pyobjectify-0.1.1/setup.py
+drwxr-xr-x   0 rjw        (501) staff       (20)        0 2023-05-04 03:21:33.039692 pyobjectify-0.2.1/
+-rw-r--r--   0 rjw        (501) staff       (20)      404 2023-05-04 03:13:36.000000 pyobjectify-0.2.1/.bumpversion.cfg
+-rw-r--r--   0 rjw        (501) staff       (20)     2799 2023-05-04 02:01:24.000000 pyobjectify-0.2.1/CONTRIBUTING.md
+-rw-r--r--   0 rjw        (501) staff       (20)     1067 2023-05-04 02:01:24.000000 pyobjectify-0.2.1/LICENSE
+-rw-r--r--   0 rjw        (501) staff       (20)     1222 2023-05-04 03:13:36.000000 pyobjectify-0.2.1/MANIFEST.in
+-rw-r--r--   0 rjw        (501) staff       (20)     2525 2023-05-04 02:01:24.000000 pyobjectify-0.2.1/Makefile
+-rw-r--r--   0 rjw        (501) staff       (20)     4567 2023-05-04 03:21:33.039480 pyobjectify-0.2.1/PKG-INFO
+-rw-r--r--   0 rjw        (501) staff       (20)     2418 2023-05-04 03:13:36.000000 pyobjectify-0.2.1/README.md
+-rw-r--r--   0 rjw        (501) staff       (20)      112 2023-05-04 02:01:24.000000 pyobjectify-0.2.1/codecov.yml
+drwxr-xr-x   0 rjw        (501) staff       (20)        0 2023-05-04 03:21:33.004643 pyobjectify-0.2.1/docs/
+-rw-r--r--   0 rjw        (501) staff       (20)      230 2023-05-04 02:01:24.000000 pyobjectify-0.2.1/docs/.buildinfo
+-rw-r--r--   0 rjw        (501) staff       (20)        0 2023-05-04 02:01:24.000000 pyobjectify-0.2.1/docs/.nojekyll
+-rw-r--r--   0 rjw        (501) staff       (20)      635 2023-05-04 02:01:24.000000 pyobjectify-0.2.1/docs/Makefile
+drwxr-xr-x   0 rjw        (501) staff       (20)        0 2023-05-04 03:21:32.997098 pyobjectify-0.2.1/docs/_build/
+drwxr-xr-x   0 rjw        (501) staff       (20)        0 2023-05-04 03:21:33.005940 pyobjectify-0.2.1/docs/_build/doctrees/
+-rw-r--r--   0 rjw        (501) staff       (20)   200609 2023-05-04 03:13:36.000000 pyobjectify-0.2.1/docs/_build/doctrees/environment.pickle
+-rw-r--r--   0 rjw        (501) staff       (20)    34936 2023-05-04 03:13:36.000000 pyobjectify-0.2.1/docs/_build/doctrees/index.doctree
+drwxr-xr-x   0 rjw        (501) staff       (20)        0 2023-05-04 03:21:33.007028 pyobjectify-0.2.1/docs/_build/doctrees/source/
+-rw-r--r--   0 rjw        (501) staff       (20)     3088 2023-05-04 03:13:36.000000 pyobjectify-0.2.1/docs/_build/doctrees/source/modules.doctree
+-rw-r--r--   0 rjw        (501) staff       (20)    87317 2023-05-04 03:13:36.000000 pyobjectify-0.2.1/docs/_build/doctrees/source/pyobjectify.doctree
+drwxr-xr-x   0 rjw        (501) staff       (20)        0 2023-05-04 03:21:33.009683 pyobjectify-0.2.1/docs/_build/html/
+-rw-r--r--   0 rjw        (501) staff       (20)      230 2023-05-04 03:13:36.000000 pyobjectify-0.2.1/docs/_build/html/.buildinfo
+drwxr-xr-x   0 rjw        (501) staff       (20)        0 2023-05-04 03:21:33.009908 pyobjectify-0.2.1/docs/_build/html/_sources/
+-rw-r--r--   0 rjw        (501) staff       (20)     7637 2023-05-04 03:13:36.000000 pyobjectify-0.2.1/docs/_build/html/_sources/index.md.txt
+drwxr-xr-x   0 rjw        (501) staff       (20)        0 2023-05-04 03:21:33.010630 pyobjectify-0.2.1/docs/_build/html/_sources/source/
+-rw-r--r--   0 rjw        (501) staff       (20)       70 2023-05-04 02:01:24.000000 pyobjectify-0.2.1/docs/_build/html/_sources/source/modules.rst.txt
+-rw-r--r--   0 rjw        (501) staff       (20)      337 2023-05-04 02:01:24.000000 pyobjectify-0.2.1/docs/_build/html/_sources/source/pyobjectify.rst.txt
+drwxr-xr-x   0 rjw        (501) staff       (20)        0 2023-05-04 03:21:33.013533 pyobjectify-0.2.1/docs/_build/html/_static/
+-rw-r--r--   0 rjw        (501) staff       (20)    14813 2023-05-04 02:51:26.000000 pyobjectify-0.2.1/docs/_build/html/_static/basic.css
+drwxr-xr-x   0 rjw        (501) staff       (20)        0 2023-05-04 03:21:33.013937 pyobjectify-0.2.1/docs/_build/html/_static/css/
+-rw-r--r--   0 rjw        (501) staff       (20)     3229 2023-05-04 02:01:24.000000 pyobjectify-0.2.1/docs/_build/html/_static/css/badge_only.css
+drwxr-xr-x   0 rjw        (501) staff       (20)        0 2023-05-04 03:21:33.031137 pyobjectify-0.2.1/docs/_build/html/_static/css/fonts/
+-rw-r--r--   0 rjw        (501) staff       (20)    87624 2023-05-04 02:01:24.000000 pyobjectify-0.2.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0 rjw        (501) staff       (20)    67312 2023-05-04 02:01:24.000000 pyobjectify-0.2.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0 rjw        (501) staff       (20)    86288 2023-05-04 02:01:24.000000 pyobjectify-0.2.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0 rjw        (501) staff       (20)    66444 2023-05-04 02:01:24.000000 pyobjectify-0.2.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0 rjw        (501) staff       (20)   165742 2023-05-04 02:01:24.000000 pyobjectify-0.2.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 rjw        (501) staff       (20)   444379 2023-05-04 02:01:24.000000 pyobjectify-0.2.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 rjw        (501) staff       (20)   165548 2023-05-04 02:01:24.000000 pyobjectify-0.2.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 rjw        (501) staff       (20)    98024 2023-05-04 02:01:24.000000 pyobjectify-0.2.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 rjw        (501) staff       (20)    77160 2023-05-04 02:01:24.000000 pyobjectify-0.2.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 rjw        (501) staff       (20)   323344 2023-05-04 02:01:24.000000 pyobjectify-0.2.1/docs/_build/html/_static/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0 rjw        (501) staff       (20)   193308 2023-05-04 02:01:24.000000 pyobjectify-0.2.1/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0 rjw        (501) staff       (20)   309728 2023-05-04 02:01:24.000000 pyobjectify-0.2.1/docs/_build/html/_static/css/fonts/lato-bold.woff
+-rw-r--r--   0 rjw        (501) staff       (20)   184912 2023-05-04 02:01:24.000000 pyobjectify-0.2.1/docs/_build/html/_static/css/fonts/lato-bold.woff2
+-rw-r--r--   0 rjw        (501) staff       (20)   328412 2023-05-04 02:01:24.000000 pyobjectify-0.2.1/docs/_build/html/_static/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0 rjw        (501) staff       (20)   195704 2023-05-04 02:01:24.000000 pyobjectify-0.2.1/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0 rjw        (501) staff       (20)   309192 2023-05-04 02:01:24.000000 pyobjectify-0.2.1/docs/_build/html/_static/css/fonts/lato-normal.woff
+-rw-r--r--   0 rjw        (501) staff       (20)   182708 2023-05-04 02:01:24.000000 pyobjectify-0.2.1/docs/_build/html/_static/css/fonts/lato-normal.woff2
+-rw-r--r--   0 rjw        (501) staff       (20)   135235 2023-05-04 02:01:24.000000 pyobjectify-0.2.1/docs/_build/html/_static/css/theme.css
+-rw-r--r--   0 rjw        (501) staff       (20)     4472 2023-05-04 02:01:24.000000 pyobjectify-0.2.1/docs/_build/html/_static/doctools.js
+-rw-r--r--   0 rjw        (501) staff       (20)      420 2023-05-04 02:51:26.000000 pyobjectify-0.2.1/docs/_build/html/_static/documentation_options.js
+-rw-r--r--   0 rjw        (501) staff       (20)      286 2023-05-04 02:01:24.000000 pyobjectify-0.2.1/docs/_build/html/_static/file.png
+drwxr-xr-x   0 rjw        (501) staff       (20)        0 2023-05-04 03:21:33.033057 pyobjectify-0.2.1/docs/_build/html/_static/js/
+-rw-r--r--   0 rjw        (501) staff       (20)      934 2023-05-04 02:01:24.000000 pyobjectify-0.2.1/docs/_build/html/_static/js/badge_only.js
+-rw-r--r--   0 rjw        (501) staff       (20)     4370 2023-05-04 02:01:24.000000 pyobjectify-0.2.1/docs/_build/html/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0 rjw        (501) staff       (20)     2734 2023-05-04 02:01:24.000000 pyobjectify-0.2.1/docs/_build/html/_static/js/html5shiv.min.js
+-rw-r--r--   0 rjw        (501) staff       (20)     5023 2023-05-04 02:01:24.000000 pyobjectify-0.2.1/docs/_build/html/_static/js/theme.js
+-rw-r--r--   0 rjw        (501) staff       (20)     4758 2023-05-04 02:51:26.000000 pyobjectify-0.2.1/docs/_build/html/_static/language_data.js
+-rw-r--r--   0 rjw        (501) staff       (20)       90 2023-05-04 02:01:24.000000 pyobjectify-0.2.1/docs/_build/html/_static/minus.png
+-rw-r--r--   0 rjw        (501) staff       (20)       90 2023-05-04 02:01:24.000000 pyobjectify-0.2.1/docs/_build/html/_static/plus.png
+-rw-r--r--   0 rjw        (501) staff       (20)     4819 2023-05-04 02:51:26.000000 pyobjectify-0.2.1/docs/_build/html/_static/pygments.css
+-rw-r--r--   0 rjw        (501) staff       (20)    18215 2023-05-04 02:01:24.000000 pyobjectify-0.2.1/docs/_build/html/_static/searchtools.js
+-rw-r--r--   0 rjw        (501) staff       (20)     4712 2023-05-04 02:01:24.000000 pyobjectify-0.2.1/docs/_build/html/_static/sphinx_highlight.js
+-rw-r--r--   0 rjw        (501) staff       (20)    10419 2023-05-04 03:13:36.000000 pyobjectify-0.2.1/docs/_build/html/genindex.html
+-rw-r--r--   0 rjw        (501) staff       (20)    25677 2023-05-04 03:13:36.000000 pyobjectify-0.2.1/docs/_build/html/index.html
+-rw-r--r--   0 rjw        (501) staff       (20)      534 2023-05-04 03:13:36.000000 pyobjectify-0.2.1/docs/_build/html/objects.inv
+-rw-r--r--   0 rjw        (501) staff       (20)     3956 2023-05-04 02:51:26.000000 pyobjectify-0.2.1/docs/_build/html/py-modindex.html
+-rw-r--r--   0 rjw        (501) staff       (20)     3536 2023-05-04 02:51:26.000000 pyobjectify-0.2.1/docs/_build/html/search.html
+-rw-r--r--   0 rjw        (501) staff       (20)     9769 2023-05-04 03:13:36.000000 pyobjectify-0.2.1/docs/_build/html/searchindex.js
+drwxr-xr-x   0 rjw        (501) staff       (20)        0 2023-05-04 03:21:33.033602 pyobjectify-0.2.1/docs/_build/html/source/
+-rw-r--r--   0 rjw        (501) staff       (20)     9482 2023-05-04 03:13:36.000000 pyobjectify-0.2.1/docs/_build/html/source/modules.html
+-rw-r--r--   0 rjw        (501) staff       (20)    37533 2023-05-04 03:13:36.000000 pyobjectify-0.2.1/docs/_build/html/source/pyobjectify.html
+-rw-r--r--   0 rjw        (501) staff       (20)     1360 2023-05-04 02:01:24.000000 pyobjectify-0.2.1/docs/conf.py
+-rw-r--r--   0 rjw        (501) staff       (20)     7637 2023-05-04 03:13:36.000000 pyobjectify-0.2.1/docs/index.md
+-rw-r--r--   0 rjw        (501) staff       (20)      765 2023-05-04 02:01:24.000000 pyobjectify-0.2.1/docs/make.bat
+-rw-r--r--   0 rjw        (501) staff       (20)     9054 2023-05-04 02:01:24.000000 pyobjectify-0.2.1/docs/modules.html
+-rw-r--r--   0 rjw        (501) staff       (20)      524 2023-05-04 02:01:24.000000 pyobjectify-0.2.1/docs/objects.inv
+drwxr-xr-x   0 rjw        (501) staff       (20)        0 2023-05-04 03:21:33.034887 pyobjectify-0.2.1/docs/source/
+-rw-r--r--   0 rjw        (501) staff       (20)       70 2023-05-04 02:01:24.000000 pyobjectify-0.2.1/docs/source/modules.rst
+-rw-r--r--   0 rjw        (501) staff       (20)      337 2023-05-04 02:01:24.000000 pyobjectify-0.2.1/docs/source/pyobjectify.rst
+drwxr-xr-x   0 rjw        (501) staff       (20)        0 2023-05-04 03:21:33.035534 pyobjectify-0.2.1/pyobjectify/
+-rw-r--r--   0 rjw        (501) staff       (20)      265 2023-05-04 02:01:24.000000 pyobjectify-0.2.1/pyobjectify/__init__.py
+-rw-r--r--   0 rjw        (501) staff       (20)       22 2023-05-04 03:13:36.000000 pyobjectify-0.2.1/pyobjectify/_version.py
+-rw-r--r--   0 rjw        (501) staff       (20)    14517 2023-05-04 03:13:36.000000 pyobjectify-0.2.1/pyobjectify/pyobjectify.py
+drwxr-xr-x   0 rjw        (501) staff       (20)        0 2023-05-04 03:21:33.037028 pyobjectify-0.2.1/pyobjectify/tests/
+drwxr-xr-x   0 rjw        (501) staff       (20)        0 2023-05-04 03:21:33.039174 pyobjectify-0.2.1/pyobjectify/tests/data/
+-rw-r--r--   0 rjw        (501) staff       (20)       21 2023-05-04 02:01:24.000000 pyobjectify-0.2.1/pyobjectify/tests/data/data.example
+-rw-r--r--   0 rjw        (501) staff       (20)     3291 2023-05-04 02:01:24.000000 pyobjectify-0.2.1/pyobjectify/tests/data/example.csv
+-rw-r--r--   0 rjw        (501) staff       (20)      330 2023-05-04 02:01:24.000000 pyobjectify-0.2.1/pyobjectify/tests/data/example.json
+-rw-r--r--   0 rjw        (501) staff       (20)     3218 2023-05-04 02:01:24.000000 pyobjectify-0.2.1/pyobjectify/tests/data/example.tsv
+-rw-r--r--   0 rjw        (501) staff       (20)     9887 2023-05-04 03:13:36.000000 pyobjectify-0.2.1/pyobjectify/tests/data/example.xlsx
+-rw-r--r--   0 rjw        (501) staff       (20)     9495 2023-05-04 02:01:24.000000 pyobjectify-0.2.1/pyobjectify/tests/data/example.xml
+-rw-r--r--   0 rjw        (501) staff       (20)      936 2023-05-04 02:01:24.000000 pyobjectify-0.2.1/pyobjectify/tests/data/test.json
+-rw-r--r--   0 rjw        (501) staff       (20)     1983 2023-05-04 02:01:24.000000 pyobjectify-0.2.1/pyobjectify/tests/test_integration.py
+-rw-r--r--   0 rjw        (501) staff       (20)    44418 2023-05-04 03:13:36.000000 pyobjectify-0.2.1/pyobjectify/tests/test_unit.py
+drwxr-xr-x   0 rjw        (501) staff       (20)        0 2023-05-04 03:21:33.036598 pyobjectify-0.2.1/pyobjectify.egg-info/
+-rw-r--r--   0 rjw        (501) staff       (20)     4567 2023-05-04 03:21:32.000000 pyobjectify-0.2.1/pyobjectify.egg-info/PKG-INFO
+-rw-r--r--   0 rjw        (501) staff       (20)     3067 2023-05-04 03:21:32.000000 pyobjectify-0.2.1/pyobjectify.egg-info/SOURCES.txt
+-rw-r--r--   0 rjw        (501) staff       (20)        1 2023-05-04 03:21:32.000000 pyobjectify-0.2.1/pyobjectify.egg-info/dependency_links.txt
+-rw-r--r--   0 rjw        (501) staff       (20)      494 2023-05-04 03:21:32.000000 pyobjectify-0.2.1/pyobjectify.egg-info/requires.txt
+-rw-r--r--   0 rjw        (501) staff       (20)       12 2023-05-04 03:21:32.000000 pyobjectify-0.2.1/pyobjectify.egg-info/top_level.txt
+-rw-r--r--   0 rjw        (501) staff       (20)     2704 2023-05-04 03:13:36.000000 pyobjectify-0.2.1/pyproject.toml
+-rw-r--r--   0 rjw        (501) staff       (20)       38 2023-05-04 03:21:33.039748 pyobjectify-0.2.1/setup.cfg
+-rw-r--r--   0 rjw        (501) staff       (20)       57 2023-05-04 03:13:36.000000 pyobjectify-0.2.1/setup.py
```

### Comparing `pyobjectify-0.1.1/CONTRIBUTING.md` & `pyobjectify-0.2.1/CONTRIBUTING.md`

 * *Files 8% similar despite different names*

```diff
@@ -6,24 +6,27 @@
 - `git clone` the repo locally or create your own fork.
 - Run `make develop` to install the development dependencies.
 
 ### Pull request checklist
 
 - [x] Update all relevant existing tests in [`/pyobjectify/tests`](https://github.com/wu-rymd/pyobjectify/tree/main/pyobjectify/tests) as necessary.
 - [x] Create relevant tests as necessary. All test files and test class functions must begin with `test_`.
+- [x] Comment all exposed functions and methods using ReStructuredText. See examples in the source code.
+- [x] Run `make html` in the `/docs` folder to update the autogenerated documentation.
+- [x] If anything in [`README.md`](https://github.com/wu-rymd/pyobjectify/blob/main/README.md) needs to be updated, please change as necessary.
 - [x] If any subdirectories were created, add paths to `Makefile` in the [black](https://github.com/wu-rymd/pyobjectify/blob/main/Makefile#L23-L24) and [flake8](https://github.com/wu-rymd/pyobjectify/blob/main/Makefile#L16-L18) configurations.
   - Avoid `**` (for now). [It's weird](https://superuser.com/questions/619849/bash-extended-globbing-inside-a-makefile). Globstar relies on newer versions of bash shell that may not be installed across many Macs.
 - [x] Add any new dependent library files to `/MANIFEST.in`
 - [x] Add any new pip packages to `/pyproject.toml`
+- [x] Run `make check` from the root directory and fix any errors.
 - [x] Run `make test` from the root directory and fix any failures.
 - [x] Run `make coverage` to see the branch coverage results. Ensure that the coverage does not decrease. If it does and is warranted, please document this in your pull request.
   - You can also run `make coverage-html` to generate an HTML report in `/htmlcov`.
 - [x] Run `make format` to run the autoformatter.
 - [x] Run `make lint` to check for any linting errors and fix any errors that occur.
-- [x] If anything in [`README.md`](https://github.com/wu-rymd/pyobjectify/blob/main/README.md) needs to be updated, please change as necessary.
 - [x] If all of the following run successfully, squash all commits into one, push changes to your own branch, and create the pull request with at least one other contributor as a reviewer.
 - [x] Merge the pull request once approved by the reviewer(s).
 
 ### Built-in commands
 
 This project uses a `Makefile` as a command registry, with the following commands:
```

### Comparing `pyobjectify-0.1.1/LICENSE` & `pyobjectify-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyobjectify-0.1.1/Makefile` & `pyobjectify-0.2.1/Makefile`

 * *Files identical despite different names*

### Comparing `pyobjectify-0.1.1/PKG-INFO` & `pyobjectify-0.2.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjectify
-Version: 0.1.1
+Version: 0.2.1
 Summary: Bridging the gap across the different file formats and streamlining the process to accessing ingested data via Python objects
 Author-email: Raymond Wu <wu.raymond@columbia.edu>
 License: MIT License
         
         Copyright (c) 2023 Raymond Wu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -36,19 +36,19 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: develop
 License-File: LICENSE
 
-# pyobjectify
+# pyobjectify [![PyPI](https://img.shields.io/pypi/v/pyobjectify?style=flat-square&color=222222)](https://pypi.org/project/pyobjectify) [![docs](https://img.shields.io/badge/-docs-black?style=flat-square)](https://wu-rymd.github.io/pyobjectify/docs/_build/html/index.html) 
 
 Bridge the gap across the different file formats and streamline the process to accessing ingested data via Python objects
 
-![license](https://img.shields.io/badge/license-MIT-green?style=flat-square&color=022169) ![issues](https://img.shields.io/github/issues/wu-rymd/pyobjectify?style=flat-square&color=841C1C) [![codecov](https://codecov.io/gh/wu-rymd/pyobjectify/branch/main/graph/badge.svg?token=410L0PN9UC)](https://codecov.io/gh/wu-rymd/pyobjectify) ![build](https://img.shields.io/github/actions/workflow/status/wu-rymd/pyobjectify/build.yml)
+![license](https://img.shields.io/badge/license-MIT-green?style=flat-square&color=022169) ![issues](https://img.shields.io/github/issues/wu-rymd/pyobjectify?style=flat-square&color=841C1C) [![codecov](https://codecov.io/gh/wu-rymd/pyobjectify/branch/main/graph/badge.svg?token=410L0PN9UC)](https://codecov.io/gh/wu-rymd/pyobjectify) ![build](https://img.shields.io/github/actions/workflow/status/wu-rymd/pyobjectify/build.yml?style=flat-square)
 
 ## Overview
 
 Open data is abound. For example, NYC Open Data has over 3,000 datasets spanning over 97 agencies in New York City. This data comes in many different formats, including CSV, JSON, XML, XLS/XLSX, KML, KMZ, Shapefile, GeoJSON, JSON, and more.
 
 In order to import and analyze the data in Python involves sending a request to download the raw data, then converting it into a Python object so that methods can be used to parse its contents. However, this process varies across the many different data types.
 
@@ -63,15 +63,15 @@
 ## Quick start
 
 ```python
 import pyobjectify
 import pandas as pd
 
 json_dict = pyobjectify.from_url("https://bit.ly/42KCUSv")  # URL holds JSON data, returns data in dict
-json_df = pyobjectify.from_url("https://bit.ly/42KCUSv", pd.DataFrames)  # User-specified output data type
+json_df = pyobjectify.from_url("https://bit.ly/42KCUSv", pd.DataFrame)  # User-specified output data type
 ```
 
 ## Supported types
 
 #### Connectivity tyes
 
 - Local files (_e.g._ `./relative/example.json`, `/absolute/path/example.json`)
@@ -81,14 +81,16 @@
 
 #### Resource (input) data types
 
 - JSON
 - CSV
 - TSV
 - XML
+- XLSX
 
 #### Supported conversions
 
 - JSON &rarr; `dict`, `list`, `pandas.DataFrame`
 - CSV &rarr; `list`
 - TSV &rarr; `list`
 - XML &rarr; `dict`
+- XLSX &rarr; `dict`
```

### Comparing `pyobjectify-0.1.1/README.md` & `pyobjectify-0.2.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# pyobjectify
+# pyobjectify [![PyPI](https://img.shields.io/pypi/v/pyobjectify?style=flat-square&color=222222)](https://pypi.org/project/pyobjectify) [![docs](https://img.shields.io/badge/-docs-black?style=flat-square)](https://wu-rymd.github.io/pyobjectify/docs/_build/html/index.html) 
 
 Bridge the gap across the different file formats and streamline the process to accessing ingested data via Python objects
 
-![license](https://img.shields.io/badge/license-MIT-green?style=flat-square&color=022169) ![issues](https://img.shields.io/github/issues/wu-rymd/pyobjectify?style=flat-square&color=841C1C) [![codecov](https://codecov.io/gh/wu-rymd/pyobjectify/branch/main/graph/badge.svg?token=410L0PN9UC)](https://codecov.io/gh/wu-rymd/pyobjectify) ![build](https://img.shields.io/github/actions/workflow/status/wu-rymd/pyobjectify/build.yml)
+![license](https://img.shields.io/badge/license-MIT-green?style=flat-square&color=022169) ![issues](https://img.shields.io/github/issues/wu-rymd/pyobjectify?style=flat-square&color=841C1C) [![codecov](https://codecov.io/gh/wu-rymd/pyobjectify/branch/main/graph/badge.svg?token=410L0PN9UC)](https://codecov.io/gh/wu-rymd/pyobjectify) ![build](https://img.shields.io/github/actions/workflow/status/wu-rymd/pyobjectify/build.yml?style=flat-square)
 
 ## Overview
 
 Open data is abound. For example, NYC Open Data has over 3,000 datasets spanning over 97 agencies in New York City. This data comes in many different formats, including CSV, JSON, XML, XLS/XLSX, KML, KMZ, Shapefile, GeoJSON, JSON, and more.
 
 In order to import and analyze the data in Python involves sending a request to download the raw data, then converting it into a Python object so that methods can be used to parse its contents. However, this process varies across the many different data types.
 
@@ -21,15 +21,15 @@
 ## Quick start
 
 ```python
 import pyobjectify
 import pandas as pd
 
 json_dict = pyobjectify.from_url("https://bit.ly/42KCUSv")  # URL holds JSON data, returns data in dict
-json_df = pyobjectify.from_url("https://bit.ly/42KCUSv", pd.DataFrames)  # User-specified output data type
+json_df = pyobjectify.from_url("https://bit.ly/42KCUSv", pd.DataFrame)  # User-specified output data type
 ```
 
 ## Supported types
 
 #### Connectivity tyes
 
 - Local files (_e.g._ `./relative/example.json`, `/absolute/path/example.json`)
@@ -39,14 +39,16 @@
 
 #### Resource (input) data types
 
 - JSON
 - CSV
 - TSV
 - XML
+- XLSX
 
 #### Supported conversions
 
 - JSON &rarr; `dict`, `list`, `pandas.DataFrame`
 - CSV &rarr; `list`
 - TSV &rarr; `list`
 - XML &rarr; `dict`
+- XLSX &rarr; `dict`
```

### Comparing `pyobjectify-0.1.1/pyobjectify/tests/data/example.csv` & `pyobjectify-0.2.1/pyobjectify/tests/data/example.csv`

 * *Files identical despite different names*

### Comparing `pyobjectify-0.1.1/pyobjectify/tests/data/example.tsv` & `pyobjectify-0.2.1/pyobjectify/tests/data/example.tsv`

 * *Files identical despite different names*

### Comparing `pyobjectify-0.1.1/pyobjectify/tests/data/example.xml` & `pyobjectify-0.2.1/pyobjectify/tests/data/example.xml`

 * *Files identical despite different names*

### Comparing `pyobjectify-0.1.1/pyobjectify/tests/data/test.json` & `pyobjectify-0.2.1/pyobjectify/tests/data/test.json`

 * *Files identical despite different names*

### Comparing `pyobjectify-0.1.1/pyobjectify/tests/test_integration.py` & `pyobjectify-0.2.1/pyobjectify/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `pyobjectify-0.1.1/pyobjectify/tests/test_unit.py` & `pyobjectify-0.2.1/pyobjectify/tests/test_unit.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 URL_LOCAL = f"{DIR}/data/example.json"
 URL_ONLINE_STATIC = "https://bit.ly/42KCUSv"
 
 URL_JSON = f"{DIR}/data/example.json"
 URL_CSV = f"{DIR}/data/example.csv"
 URL_TSV = f"{DIR}/data/example.tsv"
 URL_XML = f"{DIR}/data/example.xml"
+URL_XLSX = f"{DIR}/data/example.xlsx"
 URL_OTHER = f"{DIR}/data/data.example"
 
 CONNECTIVITY_UNSUPPORTED = str
 OUTPUT_TYPE_UNSUPPORTED = str
 
 
 class TestPyobjectify(unittest.TestCase):
@@ -60,14 +61,19 @@
         assert pyob.InputType.TSV in actual
 
     def test_get_resource_types_xml(self):
         resource = pyob.Resource(URL_XML, pyob.Connectivity.LOCAL)
         actual = pyob.get_resource_types(resource)
         assert pyob.InputType.XML in actual
 
+    def test_get_resource_types_xlsx(self):
+        resource = pyob.Resource(URL_XLSX, pyob.Connectivity.LOCAL)
+        actual = pyob.get_resource_types(resource)
+        assert pyob.InputType.XLSX in actual
+
     def test_get_resource_types_error(self):
         resource = pyob.Resource(URL_OTHER, pyob.Connectivity.LOCAL)
         with self.assertRaises(TypeError):
             pyob.get_resource_types(resource)
 
     def test_get_conversions_json(self):
         actual = pyob.get_conversions([pyob.InputType.JSON])
@@ -85,14 +91,19 @@
         self.assertEqual(actual, expected)
 
     def test_get_conversions_xml(self):
         actual = pyob.get_conversions([pyob.InputType.XML])
         expected = [(pyob.InputType.XML, dict)]
         self.assertEqual(actual, expected)
 
+    def test_get_conversions_xlsx(self):
+        actual = pyob.get_conversions([pyob.InputType.XLSX])
+        expected = [(pyob.InputType.XLSX, dict)]
+        self.assertEqual(actual, expected)
+
     def test_get_conversions_json_dataframe(self):
         actual = pyob.get_conversions([pyob.InputType.JSON], DataFrame)
         expected = [(pyob.InputType.JSON, DataFrame)]
         self.assertEqual(actual, expected)
 
     def test_get_conversions_error(self):
         with self.assertRaises(TypeError):
@@ -894,14 +905,37 @@
                         },
                     ]
                 }
             }
         }
         self.assertEqual(actual, expected)
 
+    def test_convert_xlsx_dict(self):
+        resource = pyob.Resource(URL_XLSX, pyob.Connectivity.LOCAL)
+        actual = pyob.convert(resource, [(pyob.InputType.XLSX, dict)])
+        expected = {
+            "Sheet1": {
+                "Abbreviation": {0: "MN", 1: "BK", 2: "QN", 3: "BX", 4: "SI"},
+                "Borough": {0: "Manhattan", 1: "Brooklyn", 2: "Queens", 3: "The Bronx", 4: "Staten Island"},
+                "Index": {0: 1, 1: 2, 2: 3, 3: 4, 4: 5},
+            },
+            "Sheet2": {
+                "Abbreviation": {0: "XM", 1: "XB", 2: "XQ", 3: "XX", 4: "XS"},
+                "Borough": {
+                    0: "Not Manhattan",
+                    1: "Not Brooklyn",
+                    2: "Not Queens",
+                    3: "Not The Bronx",
+                    4: "Not Staten Island",
+                },
+                "Index": {0: 6, 1: 7, 2: 8, 3: 9, 4: 10},
+            },
+        }
+        self.assertEqual(actual, expected)
+
     def test_convert_error(self):
         resource = pyob.Resource(URL_JSON, pyob.Connectivity.LOCAL)
         with self.assertRaises(TypeError):
             pyob.convert(resource, [(pyob.InputType.JSON, OUTPUT_TYPE_UNSUPPORTED)])
 
     def test_from_url(self):
         actual = pyob.from_url(URL_JSON)
```

### Comparing `pyobjectify-0.1.1/pyobjectify.egg-info/PKG-INFO` & `pyobjectify-0.2.1/pyobjectify.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjectify
-Version: 0.1.1
+Version: 0.2.1
 Summary: Bridging the gap across the different file formats and streamlining the process to accessing ingested data via Python objects
 Author-email: Raymond Wu <wu.raymond@columbia.edu>
 License: MIT License
         
         Copyright (c) 2023 Raymond Wu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -36,19 +36,19 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: develop
 License-File: LICENSE
 
-# pyobjectify
+# pyobjectify [![PyPI](https://img.shields.io/pypi/v/pyobjectify?style=flat-square&color=222222)](https://pypi.org/project/pyobjectify) [![docs](https://img.shields.io/badge/-docs-black?style=flat-square)](https://wu-rymd.github.io/pyobjectify/docs/_build/html/index.html) 
 
 Bridge the gap across the different file formats and streamline the process to accessing ingested data via Python objects
 
-![license](https://img.shields.io/badge/license-MIT-green?style=flat-square&color=022169) ![issues](https://img.shields.io/github/issues/wu-rymd/pyobjectify?style=flat-square&color=841C1C) [![codecov](https://codecov.io/gh/wu-rymd/pyobjectify/branch/main/graph/badge.svg?token=410L0PN9UC)](https://codecov.io/gh/wu-rymd/pyobjectify) ![build](https://img.shields.io/github/actions/workflow/status/wu-rymd/pyobjectify/build.yml)
+![license](https://img.shields.io/badge/license-MIT-green?style=flat-square&color=022169) ![issues](https://img.shields.io/github/issues/wu-rymd/pyobjectify?style=flat-square&color=841C1C) [![codecov](https://codecov.io/gh/wu-rymd/pyobjectify/branch/main/graph/badge.svg?token=410L0PN9UC)](https://codecov.io/gh/wu-rymd/pyobjectify) ![build](https://img.shields.io/github/actions/workflow/status/wu-rymd/pyobjectify/build.yml?style=flat-square)
 
 ## Overview
 
 Open data is abound. For example, NYC Open Data has over 3,000 datasets spanning over 97 agencies in New York City. This data comes in many different formats, including CSV, JSON, XML, XLS/XLSX, KML, KMZ, Shapefile, GeoJSON, JSON, and more.
 
 In order to import and analyze the data in Python involves sending a request to download the raw data, then converting it into a Python object so that methods can be used to parse its contents. However, this process varies across the many different data types.
 
@@ -63,15 +63,15 @@
 ## Quick start
 
 ```python
 import pyobjectify
 import pandas as pd
 
 json_dict = pyobjectify.from_url("https://bit.ly/42KCUSv")  # URL holds JSON data, returns data in dict
-json_df = pyobjectify.from_url("https://bit.ly/42KCUSv", pd.DataFrames)  # User-specified output data type
+json_df = pyobjectify.from_url("https://bit.ly/42KCUSv", pd.DataFrame)  # User-specified output data type
 ```
 
 ## Supported types
 
 #### Connectivity tyes
 
 - Local files (_e.g._ `./relative/example.json`, `/absolute/path/example.json`)
@@ -81,14 +81,16 @@
 
 #### Resource (input) data types
 
 - JSON
 - CSV
 - TSV
 - XML
+- XLSX
 
 #### Supported conversions
 
 - JSON &rarr; `dict`, `list`, `pandas.DataFrame`
 - CSV &rarr; `list`
 - TSV &rarr; `list`
 - XML &rarr; `dict`
+- XLSX &rarr; `dict`
```

### Comparing `pyobjectify-0.1.1/pyproject.toml` & `pyobjectify-0.2.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "pyobjectify"
 authors = [{name = "Raymond Wu", email = "wu.raymond@columbia.edu"}]
 description="Bridging the gap across the different file formats and streamlining the process to accessing ingested data via Python objects"
 readme = "README.md"
-version = "0.1.1"
+version = "0.2.1"
 requires-python = ">=3.7"
 
 dependencies = [
     "certifi==2022.12.7",
     "charset-normalizer==3.0.1",
     "idna==3.4",
     "requests==2.28.2",
@@ -23,15 +23,16 @@
     "types-xmltodict==0.13.0.2",
     "urllib3==1.26.14",
     "xmltodict==0.13.0",
     "numpy==1.24.2",
     "pandas==1.5.3",
     "python-dateutil==2.8.2",
     "pytz==2023.2",
-    "six==1.16.0"
+    "six==1.16.0",
+    "openpyxl==3.1.2"
 ]
 
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Programming Language :: Python :: 3",
@@ -57,15 +58,19 @@
     "flake8>=3.7.8",
     "flake8-black>=0.2.1",
     "flake8-pyproject",
     "mypy",
     "pytest>=4.3.0",
     "pytest-cov>=2.6.1",
     "twine",
-    "wheel"
+    "wheel",
+    "sphinx==6.1.3",
+    "sphinx-rtd-theme==1.2.0",
+    "recommonmark==0.7.1",
+    "sphinxcontrib-napoleon==0.7"
 ]
 
 [tool.black]
 color = true
 line-length = 120
 exclude=[
     'pyobjectify/tests/*'
```

