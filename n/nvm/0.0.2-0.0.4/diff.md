# Comparing `tmp/nvm-0.0.2.tar.gz` & `tmp/nvm-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvm-0.0.2.tar", last modified: Wed May  3 19:28:10 2023, max compression
+gzip compressed data, was "nvm-0.0.4.tar", last modified: Thu May  4 02:36:01 2023, max compression
```

## Comparing `nvm-0.0.2.tar` & `nvm-0.0.4.tar`

### file list

```diff
@@ -1,70 +1,85 @@
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-03 19:28:10.041162 nvm-0.0.2/
--rw-------   0 jiko      (1000) jiko      (1000)      292 2023-05-03 18:32:02.000000 nvm-0.0.2/.editorconfig
--rw-------   0 jiko      (1000) jiko      (1000)       29 2023-05-03 18:32:02.000000 nvm-0.0.2/.gitattributes
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-03 19:28:10.041162 nvm-0.0.2/.github/
--rw-------   0 jiko      (1000) jiko      (1000)      314 2023-05-03 18:32:02.000000 nvm-0.0.2/.github/ISSUE_TEMPLATE.md
--rw-------   0 jiko      (1000) jiko      (1000)     1217 2023-05-03 18:32:02.000000 nvm-0.0.2/.gitignore
--rw-------   0 jiko      (1000) jiko      (1000)      151 2023-05-03 18:32:02.000000 nvm-0.0.2/AUTHORS.rst
--rw-------   0 jiko      (1000) jiko      (1000)     3466 2023-05-03 18:32:02.000000 nvm-0.0.2/CONTRIBUTING.rst
--rw-------   0 jiko      (1000) jiko      (1000)       89 2023-05-03 18:32:02.000000 nvm-0.0.2/HISTORY.rst
--rw-------   0 jiko      (1000) jiko      (1000)     1534 2023-05-03 18:32:02.000000 nvm-0.0.2/LICENSE
--rw-------   0 jiko      (1000) jiko      (1000)      316 2023-05-03 18:32:02.000000 nvm-0.0.2/MANIFEST.in
--rw-------   0 jiko      (1000) jiko      (1000)     2990 2023-05-03 19:15:50.000000 nvm-0.0.2/Makefile
--rw-------   0 jiko      (1000) jiko      (1000)     1715 2023-05-03 19:28:10.041162 nvm-0.0.2/PKG-INFO
--rw-------   0 jiko      (1000) jiko      (1000)      748 2023-05-03 18:44:59.000000 nvm-0.0.2/README.rst
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-03 19:28:10.041162 nvm-0.0.2/bin/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-03 18:32:02.000000 nvm-0.0.2/bin/.gitkeep
--rw-------   0 jiko      (1000) jiko      (1000)      425 2023-05-03 18:32:02.000000 nvm-0.0.2/bin/nvm.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-03 19:28:10.041162 nvm-0.0.2/data/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-03 18:32:02.000000 nvm-0.0.2/data/.gitkeep
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-03 19:28:10.041162 nvm-0.0.2/data/emacs-logo/
--rw-------   0 jiko      (1000) jiko      (1000)     9818 2023-05-03 18:32:02.000000 nvm-0.0.2/data/emacs-logo/emacs-128x128.png
--rw-rw-r--   0 jiko      (1000) jiko      (1000)    13358 2023-05-03 18:32:02.000000 nvm-0.0.2/data/emacs-logo/emacs.svg
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-03 19:28:10.041162 nvm-0.0.2/docs/
--rw-------   0 jiko      (1000) jiko      (1000)      606 2023-05-03 18:32:02.000000 nvm-0.0.2/docs/Makefile
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-03 19:28:10.037162 nvm-0.0.2/docs/build/
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-03 19:28:10.037162 nvm-0.0.2/docs/build/html/
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-03 19:28:10.041162 nvm-0.0.2/docs/build/html/_static/
--rw-------   0 jiko      (1000) jiko      (1000)      313 2023-05-03 15:23:48.000000 nvm-0.0.2/docs/build/html/_static/check-solid.svg
--rw-------   0 jiko      (1000) jiko      (1000)      411 2023-05-03 15:23:48.000000 nvm-0.0.2/docs/build/html/_static/copy-button.svg
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-03 19:28:10.037162 nvm-0.0.2/docs/build/html/_static/css/
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-03 19:28:10.041162 nvm-0.0.2/docs/build/html/_static/css/fonts/
--rw-------   0 jiko      (1000) jiko      (1000)   444379 2023-05-03 15:23:49.000000 nvm-0.0.2/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-------   0 jiko      (1000) jiko      (1000)      286 2023-05-03 15:23:35.000000 nvm-0.0.2/docs/build/html/_static/file.png
--rw-------   0 jiko      (1000) jiko      (1000)       90 2023-05-03 15:23:35.000000 nvm-0.0.2/docs/build/html/_static/minus.png
--rw-------   0 jiko      (1000) jiko      (1000)       90 2023-05-03 15:23:35.000000 nvm-0.0.2/docs/build/html/_static/plus.png
--rw-------   0 jiko      (1000) jiko      (1000)      526 2023-05-03 19:24:06.000000 nvm-0.0.2/docs/requirements.txt
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-03 19:28:10.041162 nvm-0.0.2/docs/source/
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-03 19:28:10.041162 nvm-0.0.2/docs/source/_static/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-03 18:32:02.000000 nvm-0.0.2/docs/source/_static/.gitkeep
--rw-------   0 jiko      (1000) jiko      (1000)       31 2023-05-03 18:32:02.000000 nvm-0.0.2/docs/source/authors.rst
--rwx------   0 jiko      (1000) jiko      (1000)     5202 2023-05-03 19:00:16.000000 nvm-0.0.2/docs/source/conf.py
--rw-------   0 jiko      (1000) jiko      (1000)       36 2023-05-03 18:32:02.000000 nvm-0.0.2/docs/source/contributing.rst
--rw-------   0 jiko      (1000) jiko      (1000)       31 2023-05-03 18:32:02.000000 nvm-0.0.2/docs/source/history.rst
--rw-------   0 jiko      (1000) jiko      (1000)      319 2023-05-03 18:32:02.000000 nvm-0.0.2/docs/source/index.rst
--rw-------   0 jiko      (1000) jiko      (1000)     1086 2023-05-03 18:32:02.000000 nvm-0.0.2/docs/source/installation.rst
--rw-------   0 jiko      (1000) jiko      (1000)       46 2023-05-03 19:00:19.000000 nvm-0.0.2/docs/source/modules.rst
--rw-------   0 jiko      (1000) jiko      (1000)      265 2023-05-03 19:00:19.000000 nvm-0.0.2/docs/source/nvm.rst
--rw-------   0 jiko      (1000) jiko      (1000)       30 2023-05-03 18:32:02.000000 nvm-0.0.2/docs/source/readme.rst
--rw-------   0 jiko      (1000) jiko      (1000)       61 2023-05-03 18:32:02.000000 nvm-0.0.2/docs/source/usage.rst
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-03 19:28:10.041162 nvm-0.0.2/nvm/
--rw-------   0 jiko      (1000) jiko      (1000)      338 2023-05-03 18:32:02.000000 nvm-0.0.2/nvm/__init__.py
--rw-------   0 jiko      (1000) jiko      (1000)      497 2023-05-03 19:28:10.041162 nvm-0.0.2/nvm/_version.py
--rw-------   0 jiko      (1000) jiko      (1000)       66 2023-05-03 18:32:02.000000 nvm-0.0.2/nvm/nvm.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-03 19:28:10.041162 nvm-0.0.2/nvm.egg-info/
--rw-------   0 jiko      (1000) jiko      (1000)     1715 2023-05-03 19:28:09.000000 nvm-0.0.2/nvm.egg-info/PKG-INFO
--rw-------   0 jiko      (1000) jiko      (1000)     1130 2023-05-03 19:28:10.000000 nvm-0.0.2/nvm.egg-info/SOURCES.txt
--rw-------   0 jiko      (1000) jiko      (1000)        1 2023-05-03 19:28:09.000000 nvm-0.0.2/nvm.egg-info/dependency_links.txt
--rw-------   0 jiko      (1000) jiko      (1000)       37 2023-05-03 19:28:09.000000 nvm-0.0.2/nvm.egg-info/entry_points.txt
--rw-------   0 jiko      (1000) jiko      (1000)        1 2023-05-03 19:28:09.000000 nvm-0.0.2/nvm.egg-info/not-zip-safe
--rw-------   0 jiko      (1000) jiko      (1000)     1013 2023-05-03 19:28:09.000000 nvm-0.0.2/nvm.egg-info/requires.txt
--rw-------   0 jiko      (1000) jiko      (1000)        4 2023-05-03 19:28:09.000000 nvm-0.0.2/nvm.egg-info/top_level.txt
--rw-rw-r--   0 jiko      (1000) jiko      (1000)      755 2023-05-03 18:32:02.000000 nvm-0.0.2/pyproject.toml
--rw-------   0 jiko      (1000) jiko      (1000)      414 2023-05-03 18:32:02.000000 nvm-0.0.2/requirements_dev.txt
--rw-------   0 jiko      (1000) jiko      (1000)      546 2023-05-03 19:28:10.041162 nvm-0.0.2/setup.cfg
--rw-------   0 jiko      (1000) jiko      (1000)     2578 2023-05-03 18:32:02.000000 nvm-0.0.2/setup.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-03 19:28:10.041162 nvm-0.0.2/tests/
--rw-------   0 jiko      (1000) jiko      (1000)       33 2023-05-03 18:32:02.000000 nvm-0.0.2/tests/__init__.py
--rw-------   0 jiko      (1000) jiko      (1000)      554 2023-05-03 18:32:02.000000 nvm-0.0.2/tests/test_nvm.py
--rw-------   0 jiko      (1000) jiko      (1000)      533 2023-05-03 18:32:02.000000 nvm-0.0.2/tox.ini
--rw-------   0 jiko      (1000) jiko      (1000)    83607 2023-05-03 18:32:02.000000 nvm-0.0.2/versioneer.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-04 02:36:01.126451 nvm-0.0.4/
+-rw-------   0 jiko      (1000) jiko      (1000)      292 2023-05-03 18:32:02.000000 nvm-0.0.4/.editorconfig
+-rw-------   0 jiko      (1000) jiko      (1000)       29 2023-05-03 18:32:02.000000 nvm-0.0.4/.gitattributes
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-04 02:36:01.122451 nvm-0.0.4/.github/
+-rw-------   0 jiko      (1000) jiko      (1000)      314 2023-05-03 18:32:02.000000 nvm-0.0.4/.github/ISSUE_TEMPLATE.md
+-rw-------   0 jiko      (1000) jiko      (1000)     1249 2023-05-04 01:10:13.000000 nvm-0.0.4/.gitignore
+-rw-------   0 jiko      (1000) jiko      (1000)      151 2023-05-03 18:32:02.000000 nvm-0.0.4/AUTHORS.rst
+-rw-------   0 jiko      (1000) jiko      (1000)     3466 2023-05-03 18:32:02.000000 nvm-0.0.4/CONTRIBUTING.rst
+-rw-------   0 jiko      (1000) jiko      (1000)       89 2023-05-03 18:32:02.000000 nvm-0.0.4/HISTORY.rst
+-rw-------   0 jiko      (1000) jiko      (1000)     1534 2023-05-03 18:32:02.000000 nvm-0.0.4/LICENSE
+-rw-------   0 jiko      (1000) jiko      (1000)      316 2023-05-03 18:32:02.000000 nvm-0.0.4/MANIFEST.in
+-rw-------   0 jiko      (1000) jiko      (1000)     3032 2023-05-03 20:09:42.000000 nvm-0.0.4/Makefile
+-rw-------   0 jiko      (1000) jiko      (1000)     1715 2023-05-04 02:36:01.126451 nvm-0.0.4/PKG-INFO
+-rw-------   0 jiko      (1000) jiko      (1000)      748 2023-05-03 18:44:59.000000 nvm-0.0.4/README.rst
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-04 02:36:01.122451 nvm-0.0.4/bin/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-03 18:32:02.000000 nvm-0.0.4/bin/.gitkeep
+-rw-------   0 jiko      (1000) jiko      (1000)      425 2023-05-03 18:32:02.000000 nvm-0.0.4/bin/nvm.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-04 02:36:01.122451 nvm-0.0.4/data/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-03 18:32:02.000000 nvm-0.0.4/data/.gitkeep
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-04 02:36:01.122451 nvm-0.0.4/data/emacs-logo/
+-rw-------   0 jiko      (1000) jiko      (1000)     9818 2023-05-03 18:32:02.000000 nvm-0.0.4/data/emacs-logo/emacs-128x128.png
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)    13358 2023-05-03 18:32:02.000000 nvm-0.0.4/data/emacs-logo/emacs.svg
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-04 02:36:01.122451 nvm-0.0.4/docs/
+-rw-------   0 jiko      (1000) jiko      (1000)      606 2023-05-03 18:32:02.000000 nvm-0.0.4/docs/Makefile
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-04 02:36:01.118451 nvm-0.0.4/docs/build/
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-04 02:36:01.118451 nvm-0.0.4/docs/build/html/
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-04 02:36:01.122451 nvm-0.0.4/docs/build/html/_static/
+-rw-------   0 jiko      (1000) jiko      (1000)      313 2023-05-03 15:23:48.000000 nvm-0.0.4/docs/build/html/_static/check-solid.svg
+-rw-------   0 jiko      (1000) jiko      (1000)      411 2023-05-03 15:23:48.000000 nvm-0.0.4/docs/build/html/_static/copy-button.svg
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-04 02:36:01.122451 nvm-0.0.4/docs/build/html/_static/css/
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-04 02:36:01.122451 nvm-0.0.4/docs/build/html/_static/css/fonts/
+-rw-------   0 jiko      (1000) jiko      (1000)   444379 2023-05-03 15:23:49.000000 nvm-0.0.4/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-------   0 jiko      (1000) jiko      (1000)      286 2023-05-03 15:23:35.000000 nvm-0.0.4/docs/build/html/_static/file.png
+-rw-------   0 jiko      (1000) jiko      (1000)       90 2023-05-03 15:23:35.000000 nvm-0.0.4/docs/build/html/_static/minus.png
+-rw-------   0 jiko      (1000) jiko      (1000)       90 2023-05-03 15:23:35.000000 nvm-0.0.4/docs/build/html/_static/plus.png
+-rw-------   0 jiko      (1000) jiko      (1000)      526 2023-05-03 19:24:06.000000 nvm-0.0.4/docs/requirements.txt
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-04 02:36:01.122451 nvm-0.0.4/docs/source/
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-04 02:36:01.122451 nvm-0.0.4/docs/source/_static/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-03 18:32:02.000000 nvm-0.0.4/docs/source/_static/.gitkeep
+-rw-------   0 jiko      (1000) jiko      (1000)       31 2023-05-03 18:32:02.000000 nvm-0.0.4/docs/source/authors.rst
+-rwx------   0 jiko      (1000) jiko      (1000)     5541 2023-05-04 00:55:18.000000 nvm-0.0.4/docs/source/conf.py
+-rw-------   0 jiko      (1000) jiko      (1000)       36 2023-05-03 18:32:02.000000 nvm-0.0.4/docs/source/contributing.rst
+-rw-------   0 jiko      (1000) jiko      (1000)       31 2023-05-03 18:32:02.000000 nvm-0.0.4/docs/source/history.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      319 2023-05-03 18:32:02.000000 nvm-0.0.4/docs/source/index.rst
+-rw-------   0 jiko      (1000) jiko      (1000)     1086 2023-05-03 18:32:02.000000 nvm-0.0.4/docs/source/installation.rst
+-rw-------   0 jiko      (1000) jiko      (1000)       46 2023-05-04 01:17:49.000000 nvm-0.0.4/docs/source/modules.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      331 2023-05-04 00:48:09.000000 nvm-0.0.4/docs/source/nvm.aux_log.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      331 2023-05-03 20:38:41.000000 nvm-0.0.4/docs/source/nvm.aux_str.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      331 2023-05-03 23:04:50.000000 nvm-0.0.4/docs/source/nvm.aux_sys.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      366 2023-05-04 01:17:49.000000 nvm-0.0.4/docs/source/nvm.rst
+-rw-------   0 jiko      (1000) jiko      (1000)       30 2023-05-03 18:32:02.000000 nvm-0.0.4/docs/source/readme.rst
+-rw-------   0 jiko      (1000) jiko      (1000)       61 2023-05-03 18:32:02.000000 nvm-0.0.4/docs/source/usage.rst
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-04 02:36:01.126451 nvm-0.0.4/nvm/
+-rw-------   0 jiko      (1000) jiko      (1000)      455 2023-05-04 02:13:00.000000 nvm-0.0.4/nvm/__init__.py
+-rw-------   0 jiko      (1000) jiko      (1000)      497 2023-05-04 02:36:01.126451 nvm-0.0.4/nvm/_version.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-04 02:36:01.126451 nvm-0.0.4/nvm/aux_log/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)       51 2023-05-04 00:33:55.000000 nvm-0.0.4/nvm/aux_log/__init__.py
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)     5073 2023-05-04 01:17:45.000000 nvm-0.0.4/nvm/aux_log/aux_log.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-04 02:36:01.126451 nvm-0.0.4/nvm/aux_pandas/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)      105 2023-05-04 02:17:41.000000 nvm-0.0.4/nvm/aux_pandas/__init__.py
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)     1588 2023-05-04 02:26:33.000000 nvm-0.0.4/nvm/aux_pandas/aux_pandas.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-04 02:36:01.126451 nvm-0.0.4/nvm/aux_str/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)      146 2023-05-03 21:40:50.000000 nvm-0.0.4/nvm/aux_str/__init__.py
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)     5218 2023-05-03 23:59:43.000000 nvm-0.0.4/nvm/aux_str/aux_str.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-04 02:36:01.126451 nvm-0.0.4/nvm/aux_sys/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)       51 2023-05-03 23:08:53.000000 nvm-0.0.4/nvm/aux_sys/__init__.py
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)     1341 2023-05-04 00:31:05.000000 nvm-0.0.4/nvm/aux_sys/aux_sys.py
+-rw-------   0 jiko      (1000) jiko      (1000)       66 2023-05-03 18:32:02.000000 nvm-0.0.4/nvm/nvm.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-04 02:36:01.126451 nvm-0.0.4/nvm.egg-info/
+-rw-------   0 jiko      (1000) jiko      (1000)     1715 2023-05-04 02:36:00.000000 nvm-0.0.4/nvm.egg-info/PKG-INFO
+-rw-------   0 jiko      (1000) jiko      (1000)     1411 2023-05-04 02:36:01.000000 nvm-0.0.4/nvm.egg-info/SOURCES.txt
+-rw-------   0 jiko      (1000) jiko      (1000)        1 2023-05-04 02:36:00.000000 nvm-0.0.4/nvm.egg-info/dependency_links.txt
+-rw-------   0 jiko      (1000) jiko      (1000)       37 2023-05-04 02:36:00.000000 nvm-0.0.4/nvm.egg-info/entry_points.txt
+-rw-------   0 jiko      (1000) jiko      (1000)        1 2023-05-04 02:36:00.000000 nvm-0.0.4/nvm.egg-info/not-zip-safe
+-rw-------   0 jiko      (1000) jiko      (1000)     1013 2023-05-04 02:36:00.000000 nvm-0.0.4/nvm.egg-info/requires.txt
+-rw-------   0 jiko      (1000) jiko      (1000)        4 2023-05-04 02:36:00.000000 nvm-0.0.4/nvm.egg-info/top_level.txt
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)      755 2023-05-03 18:32:02.000000 nvm-0.0.4/pyproject.toml
+-rw-------   0 jiko      (1000) jiko      (1000)      414 2023-05-03 18:32:02.000000 nvm-0.0.4/requirements_dev.txt
+-rw-------   0 jiko      (1000) jiko      (1000)      673 2023-05-04 02:36:01.126451 nvm-0.0.4/setup.cfg
+-rw-------   0 jiko      (1000) jiko      (1000)     2578 2023-05-03 18:32:02.000000 nvm-0.0.4/setup.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-04 02:36:01.126451 nvm-0.0.4/tests/
+-rw-------   0 jiko      (1000) jiko      (1000)       33 2023-05-03 18:32:02.000000 nvm-0.0.4/tests/__init__.py
+-rw-------   0 jiko      (1000) jiko      (1000)      554 2023-05-03 18:32:02.000000 nvm-0.0.4/tests/test_nvm.py
+-rw-------   0 jiko      (1000) jiko      (1000)      533 2023-05-03 18:32:02.000000 nvm-0.0.4/tox.ini
+-rw-------   0 jiko      (1000) jiko      (1000)    83607 2023-05-03 18:32:02.000000 nvm-0.0.4/versioneer.py
```

### Comparing `nvm-0.0.2/.gitignore` & `nvm-0.0.4/.gitignore`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+
+logs/
+arch/
+arch*
+temp/
+temp*
+
 .travis.yml
 
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
```

### Comparing `nvm-0.0.2/CONTRIBUTING.rst` & `nvm-0.0.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nvm-0.0.2/LICENSE` & `nvm-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nvm-0.0.2/Makefile` & `nvm-0.0.4/Makefile`

 * *Files 10% similar despite different names*

```diff
@@ -45,20 +45,21 @@
 
 clean-test: ## remove test and coverage artifacts
 	rm -fr .tox/
 	rm -f .coverage
 	rm -fr htmlcov/
 	rm -fr .pytest_cache
 
-lint/flake8: ## check style with flake8
-	flake8 nvm tests
-lint/black: ## check style with black
-	black --check nvm tests
+lint-flake8: ## check style with flake8
+	flake8 nvm tests --exit-zero --count --statistics
 
-lint: lint/flake8 lint/black ## check style
+lint-black: ## check style with black
+	black --check nvm tests || true
+
+lint: lint-flake8 lint-black ## check style
 
 test: ## run tests quickly with the default Python
 	pytest -W "ignore::DeprecationWarning" -v
 
 test-all: ## run tests on every Python version with tox
 	tox
```

### Comparing `nvm-0.0.2/PKG-INFO` & `nvm-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvm
-Version: 0.0.2
+Version: 0.0.4
 Summary: Plenty little helpers.
 Home-page: https://github.com/cogsys-io/nvm
 Author: cogsys.io
 Author-email: cogsys@cogsys.io
 License: GNU General Public License v3
 Keywords: nvm
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nvm-0.0.2/README.rst` & `nvm-0.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `nvm-0.0.2/data/emacs-logo/emacs-128x128.png` & `nvm-0.0.4/data/emacs-logo/emacs-128x128.png`

 * *Files identical despite different names*

### Comparing `nvm-0.0.2/data/emacs-logo/emacs.svg` & `nvm-0.0.4/data/emacs-logo/emacs.svg`

 * *Files identical despite different names*

### Comparing `nvm-0.0.2/docs/Makefile` & `nvm-0.0.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nvm-0.0.2/docs/build/html/_static/css/fonts/fontawesome-webfont.svg` & `nvm-0.0.4/docs/build/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `nvm-0.0.2/docs/requirements.txt` & `nvm-0.0.4/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `nvm-0.0.2/docs/source/conf.py` & `nvm-0.0.4/docs/source/conf.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,16 +34,31 @@
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named "sphinx.ext.*") or your custom ones.
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.viewcode",
     "sphinx_copybutton",
+    # "numpydoc",
+    "sphinx.ext.napoleon",
+    "sphinx.ext.mathjax",
 ]
 
+# numpydoc
+numpydoc_show_class_members = True
+
+# Control napoleon
+napoleon_google_docstring = False
+napolean_include_init_with_doc = True
+napoleon_use_ivar = True
+napoleon_use_param = False
+
+# Control autodoc
+autoclass_content = "both"  # include init doc with class
+
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 #
 # source_suffix = [".rst", ".md"]
```

### Comparing `nvm-0.0.2/docs/source/installation.rst` & `nvm-0.0.4/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `nvm-0.0.2/nvm.egg-info/PKG-INFO` & `nvm-0.0.4/nvm.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvm
-Version: 0.0.2
+Version: 0.0.4
 Summary: Plenty little helpers.
 Home-page: https://github.com/cogsys-io/nvm
 Author: cogsys.io
 Author-email: cogsys@cogsys.io
 License: GNU General Public License v3
 Keywords: nvm
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nvm-0.0.2/nvm.egg-info/SOURCES.txt` & `nvm-0.0.4/nvm.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -31,23 +31,34 @@
 docs/source/authors.rst
 docs/source/conf.py
 docs/source/contributing.rst
 docs/source/history.rst
 docs/source/index.rst
 docs/source/installation.rst
 docs/source/modules.rst
+docs/source/nvm.aux_log.rst
+docs/source/nvm.aux_str.rst
+docs/source/nvm.aux_sys.rst
 docs/source/nvm.rst
 docs/source/readme.rst
 docs/source/usage.rst
 docs/source/_static/.gitkeep
 nvm/__init__.py
 nvm/_version.py
 nvm/nvm.py
 nvm.egg-info/PKG-INFO
 nvm.egg-info/SOURCES.txt
 nvm.egg-info/dependency_links.txt
 nvm.egg-info/entry_points.txt
 nvm.egg-info/not-zip-safe
 nvm.egg-info/requires.txt
 nvm.egg-info/top_level.txt
+nvm/aux_log/__init__.py
+nvm/aux_log/aux_log.py
+nvm/aux_pandas/__init__.py
+nvm/aux_pandas/aux_pandas.py
+nvm/aux_str/__init__.py
+nvm/aux_str/aux_str.py
+nvm/aux_sys/__init__.py
+nvm/aux_sys/aux_sys.py
 tests/__init__.py
 tests/test_nvm.py
```

### Comparing `nvm-0.0.2/nvm.egg-info/requires.txt` & `nvm-0.0.4/nvm.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `nvm-0.0.2/pyproject.toml` & `nvm-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nvm-0.0.2/setup.py` & `nvm-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `nvm-0.0.2/tests/test_nvm.py` & `nvm-0.0.4/tests/test_nvm.py`

 * *Files identical despite different names*

### Comparing `nvm-0.0.2/tox.ini` & `nvm-0.0.4/tox.ini`

 * *Files identical despite different names*

### Comparing `nvm-0.0.2/versioneer.py` & `nvm-0.0.4/versioneer.py`

 * *Files identical despite different names*

