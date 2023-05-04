# Comparing `tmp/mkpkg-0.9.0.tar.gz` & `tmp/mkpkg-2023.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mkpkg-0.9.0.tar", last modified: Sun Aug 18 16:06:47 2019, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `mkpkg-0.9.0.tar` & `mkpkg-2023.5.1.tar`

### file list

```diff
@@ -1,52 +1,49 @@
-drwxr-xr-x   0 julian     (501) staff       (20)        0 2019-08-18 16:06:47.000000 mkpkg-0.9.0/
--rw-r--r--   0 julian     (501) staff       (20)     2245 2019-08-18 16:06:47.000000 mkpkg-0.9.0/PKG-INFO
-drwxr-xr-x   0 julian     (501) staff       (20)        0 2019-08-18 16:06:47.000000 mkpkg-0.9.0/mkpkg.egg-info/
--rw-r--r--   0 julian     (501) staff       (20)     2245 2019-08-18 16:06:47.000000 mkpkg-0.9.0/mkpkg.egg-info/PKG-INFO
--rw-r--r--   0 julian     (501) staff       (20)      978 2019-08-18 16:06:47.000000 mkpkg-0.9.0/mkpkg.egg-info/SOURCES.txt
--rw-r--r--   0 julian     (501) staff       (20)       43 2019-08-18 16:06:47.000000 mkpkg-0.9.0/mkpkg.egg-info/entry_points.txt
--rw-r--r--   0 julian     (501) staff       (20)       70 2019-08-18 16:06:47.000000 mkpkg-0.9.0/mkpkg.egg-info/requires.txt
--rw-r--r--   0 julian     (501) staff       (20)        6 2019-08-18 16:06:47.000000 mkpkg-0.9.0/mkpkg.egg-info/top_level.txt
--rw-r--r--   0 julian     (501) staff       (20)        1 2019-08-18 16:06:47.000000 mkpkg-0.9.0/mkpkg.egg-info/dependency_links.txt
--rw-r--r--   0 julian     (501) staff       (20)      150 2019-06-18 13:18:30.000000 mkpkg-0.9.0/codecov.yml
--rw-r--r--   0 julian     (501) staff       (20)       59 2019-07-07 14:16:07.000000 mkpkg-0.9.0/test-requirements.txt
--rw-r--r--   0 julian     (501) staff       (20)       88 2019-07-04 14:57:07.000000 mkpkg-0.9.0/MANIFEST.in
--rw-r--r--   0 julian     (501) staff       (20)       59 2019-06-18 13:18:30.000000 mkpkg-0.9.0/.coveragerc
-drwxr-xr-x   0 julian     (501) staff       (20)        0 2019-08-18 16:06:47.000000 mkpkg-0.9.0/docs/
--rw-r--r--   0 julian     (501) staff       (20)      211 2019-06-18 13:18:32.000000 mkpkg-0.9.0/docs/index.rst
--rw-r--r--   0 julian     (501) staff       (20)       53 2019-06-18 13:18:30.000000 mkpkg-0.9.0/docs/requirements.txt
--rw-r--r--   0 julian     (501) staff       (20)      580 2019-06-18 13:18:32.000000 mkpkg-0.9.0/docs/Makefile
--rw-r--r--   0 julian     (501) staff       (20)     5855 2019-08-02 00:08:04.000000 mkpkg-0.9.0/docs/conf.py
--rw-r--r--   0 julian     (501) staff       (20)        0 2019-06-21 12:39:36.000000 mkpkg-0.9.0/docs/spelling_wordlist.txt
--rw-r--r--   0 julian     (501) staff       (20)     1057 2019-06-18 13:18:30.000000 mkpkg-0.9.0/COPYING
--rw-r--r--   0 julian     (501) staff       (20)       57 2019-06-18 13:18:30.000000 mkpkg-0.9.0/setup.py
--rw-r--r--   0 julian     (501) staff       (20)     3026 2019-08-04 00:40:51.000000 mkpkg-0.9.0/tox.ini
--rw-r--r--   0 julian     (501) staff       (20)      140 2019-06-18 13:18:30.000000 mkpkg-0.9.0/.testr.conf
--rw-r--r--   0 julian     (501) staff       (20)      994 2019-08-18 16:06:47.000000 mkpkg-0.9.0/setup.cfg
--rw-r--r--   0 julian     (501) staff       (20)     1180 2019-07-21 20:41:45.000000 mkpkg-0.9.0/README.rst
-drwxr-xr-x   0 julian     (501) staff       (20)        0 2019-08-18 16:06:47.000000 mkpkg-0.9.0/mkpkg/
--rw-r--r--   0 julian     (501) staff       (20)    11001 2019-07-21 20:45:45.000000 mkpkg-0.9.0/mkpkg/_cli.py
-drwxr-xr-x   0 julian     (501) staff       (20)        0 2019-08-18 16:06:47.000000 mkpkg-0.9.0/mkpkg/tests/
--rw-r--r--   0 julian     (501) staff       (20)        0 2019-06-18 13:18:30.000000 mkpkg-0.9.0/mkpkg/tests/__init__.py
--rw-r--r--   0 julian     (501) staff       (20)     5560 2019-08-18 16:06:44.000000 mkpkg-0.9.0/mkpkg/tests/test_integration.py
-drwxr-xr-x   0 julian     (501) staff       (20)        0 2019-08-18 16:06:47.000000 mkpkg-0.9.0/mkpkg/template/
--rw-r--r--   0 julian     (501) staff       (20)      150 2019-07-05 01:45:37.000000 mkpkg-0.9.0/mkpkg/template/codecov.yml
--rw-r--r--   0 julian     (501) staff       (20)       72 2019-07-05 01:43:26.000000 mkpkg-0.9.0/mkpkg/template/.coveragerc.j2
--rw-r--r--   0 julian     (501) staff       (20)     1265 2019-07-09 00:58:39.000000 mkpkg-0.9.0/mkpkg/template/setup.cfg.j2
--rw-r--r--   0 julian     (501) staff       (20)      122 2019-07-09 01:38:16.000000 mkpkg-0.9.0/mkpkg/template/tests.py.j2
--rw-r--r--   0 julian     (501) staff       (20)       66 2019-07-04 15:11:18.000000 mkpkg-0.9.0/mkpkg/template/MANIFEST.in
-drwxr-xr-x   0 julian     (501) staff       (20)        0 2019-08-18 16:06:47.000000 mkpkg-0.9.0/mkpkg/template/docs/
--rw-r--r--   0 julian     (501) staff       (20)       75 2019-07-17 20:53:02.000000 mkpkg-0.9.0/mkpkg/template/docs/index.rst.j2
--rw-r--r--   0 julian     (501) staff       (20)       53 2019-07-04 15:15:53.000000 mkpkg-0.9.0/mkpkg/template/docs/requirements.txt
--rw-r--r--   0 julian     (501) staff       (20)     1050 2019-07-21 20:47:33.000000 mkpkg-0.9.0/mkpkg/template/README.rst.j2
--rw-r--r--   0 julian     (501) staff       (20)       57 2019-07-04 15:13:00.000000 mkpkg-0.9.0/mkpkg/template/setup.py
--rw-r--r--   0 julian     (501) staff       (20)     2536 2019-08-18 16:05:55.000000 mkpkg-0.9.0/mkpkg/template/tox.ini.j2
--rw-r--r--   0 julian     (501) staff       (20)      140 2019-07-04 15:14:41.000000 mkpkg-0.9.0/mkpkg/template/.testr.conf
--rw-r--r--   0 julian     (501) staff       (20)      194 2019-07-17 20:53:02.000000 mkpkg-0.9.0/mkpkg/template/.travis.yml.j2
--rw-r--r--   0 julian     (501) staff       (20)     1129 2019-07-05 13:43:30.000000 mkpkg-0.9.0/mkpkg/template/COPYING.j2
-drwxr-xr-x   0 julian     (501) staff       (20)        0 2019-08-18 16:06:47.000000 mkpkg-0.9.0/mkpkg/template/package/
--rw-r--r--   0 julian     (501) staff       (20)      181 2019-07-05 13:32:57.000000 mkpkg-0.9.0/mkpkg/template/package/__init__.py
--rw-r--r--   0 julian     (501) staff       (20)      163 2019-07-07 20:32:40.000000 mkpkg-0.9.0/mkpkg/template/package/_cli.py.j2
--rw-r--r--   0 julian     (501) staff       (20)       48 2019-07-07 14:28:41.000000 mkpkg-0.9.0/mkpkg/template/package/__main__.py.j2
--rw-r--r--   0 julian     (501) staff       (20)      181 2019-06-18 13:18:30.000000 mkpkg-0.9.0/mkpkg/__init__.py
--rw-r--r--   0 julian     (501) staff       (20)       35 2019-07-05 15:55:59.000000 mkpkg-0.9.0/mkpkg/__main__.py
--rw-r--r--   0 julian     (501) staff       (20)      161 2019-07-17 20:53:02.000000 mkpkg-0.9.0/.travis.yml
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/.coveragerc
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/.flake8
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/.readthedocs.yml
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/.testr.conf
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/codecov.yml
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/test-requirements.txt
+-rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/tox.ini
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/.github/FUNDING.yml
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/.github/SECURITY.md
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/.github/dependabot.yml
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/.github/release.yml
+-rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/docs/Makefile
+-rw-r--r--   0        0        0     5960 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/docs/conf.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/docs/index.rst
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/docs/requirements.in
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/docs/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/docs/spelling_wordlist.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/mkpkg/__init__.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/mkpkg/__main__.py
+-rw-r--r--   0        0        0    11770 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/mkpkg/_cli.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/mkpkg/template/.coveragerc.j2
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/mkpkg/template/.flake8
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/mkpkg/template/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/mkpkg/template/.testr.conf
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/mkpkg/template/COPYING.j2
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/mkpkg/template/README.rst.j2
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/mkpkg/template/codecov.yml
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/mkpkg/template/pyproject.toml.j2
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/mkpkg/template/tests.py.j2
+-rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/mkpkg/template/tox.ini.j2
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/mkpkg/template/.github/FUNDING.yml
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/mkpkg/template/.github/SECURITY.md.j2
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/mkpkg/template/.github/dependabot.yml
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/mkpkg/template/.github/release.yml
+-rw-r--r--   0        0        0     3576 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/mkpkg/template/.github/workflows/ci.yml.j2
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/mkpkg/template/docs/index.rst
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/mkpkg/template/docs/requirements.in
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/mkpkg/template/package/__init__.py.j2
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/mkpkg/template/package/__main__.py.j2
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/mkpkg/template/package/_build.py.j2
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/mkpkg/template/package/_cli.py.j2
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/mkpkg/tests/__init__.py
+-rw-r--r--   0        0        0     7293 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/mkpkg/tests/test_integration.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/COPYING
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/README.rst
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/pyproject.toml
+-rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `mkpkg-0.9.0/PKG-INFO` & `mkpkg-2023.5.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,55 +1,58 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: mkpkg
-Version: 0.9.0
-Summary: UNKNOWN
-Home-page: https://github.com/Julian/mkpkg
+Version: 2023.5.1
+Summary: A package @Julian uses to create Python packages.
+Project-URL: Homepage, https://github.com/Julian/mkpkg
+Project-URL: Documentation, https://mkpkg.readthedocs.io/
+Project-URL: Issues, https://github.com/Julian/mkpkg/issues/
+Project-URL: Funding, https://github.com/sponsors/Julian
+Project-URL: Source, https://github.com/Julian/mkpkg
 Author: Julian Berman
 Author-email: Julian+mkpkg@GrayVines.com
-License: UNKNOWN
-Description: =====
-        mkpkg
-        =====
-        
-        |PyPI| |Pythons| |Travis| |AppVeyor| |Codecov| |ReadTheDocs|
-        
-        .. |PyPI| image:: https://img.shields.io/pypi/v/mkpkg.svg
-           :alt: PyPI version
-           :target: https://pypi.org/project/mkpkg/
-        
-        .. |Pythons| image:: https://img.shields.io/pypi/pyversions/mkpkg.svg
-           :alt: Supported Python versions
-           :target: https://pypi.org/project/mkpkg/
-        
-        .. |Travis| image:: https://travis-ci.org/Julian/mkpkg.svg?branch=master
-           :alt: Travis build status
-           :target: https://travis-ci.org/Julian/mkpkg
-        
-        .. |AppVeyor| image:: https://ci.appveyor.com/api/projects/status/n0ddnkcr1xh2j1fu?svg=true
-           :alt: AppVeyor build status
-           :target: https://ci.appveyor.com/project/Julian/mkpkg
-        
-        .. |Codecov| image:: https://codecov.io/gh/Julian/mkpkg/branch/master/graph/badge.svg
-           :alt: Codecov Code coverage
-           :target: https://codecov.io/gh/Julian/mkpkg
-        
-        .. |ReadTheDocs| image:: https://readthedocs.org/projects/mkpkg/badge/?version=stable&style=flat
-           :alt: ReadTheDocs status
-           :target: https://mkpkg.readthedocs.io/en/stable/
-        
-        
-        A package I (`Julian <https://github.com/Julian>`_) use to create Python packages.
-        
-        It’s here for myself, but feel free to use it if you’d like.
-        
-Platform: UNKNOWN
+License: MIT
+License-File: COPYING
+Keywords: packaging,templating
 Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.8
+Requires-Dist: click
+Requires-Dist: jinja2
+Requires-Dist: sphinx
+Description-Content-Type: text/x-rst
+
+=========
+``mkpkg``
+=========
+
+|PyPI| |Pythons| |CI| |ReadTheDocs|
+
+.. |PyPI| image:: https://img.shields.io/pypi/v/mkpkg.svg
+   :alt: PyPI version
+   :target: https://pypi.org/project/mkpkg/
+
+.. |Pythons| image:: https://img.shields.io/pypi/pyversions/mkpkg.svg
+   :alt: Supported Python versions
+   :target: https://pypi.org/project/mkpkg/
+
+.. |CI| image:: https://github.com/Julian/mkpkg/workflows/CI/badge.svg
+  :alt: Build status
+  :target: https://github.com/Julian/mkpkg/actions?query=workflow%3ACI
+
+.. |ReadTheDocs| image:: https://readthedocs.org/projects/mkpkg/badge/?version=stable&style=flat
+   :alt: ReadTheDocs status
+   :target: https://mkpkg.readthedocs.io/en/stable/
+
+
+A package I (`Julian <https://github.com/Julian>`_) use to create Python packages.
+
+It’s here for myself, but feel free to use it if you’d like.
```

### Comparing `mkpkg-0.9.0/docs/Makefile` & `mkpkg-2023.5.1/docs/Makefile`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
 
 .PHONY: help Makefile
 
 # Catch-all target: route all unknown targets to Sphinx using the new
 # "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
 %: Makefile
-	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
+	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
```

### Comparing `mkpkg-0.9.0/docs/conf.py` & `mkpkg-2023.5.1/docs/conf.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,195 +1,213 @@
-# -*- coding: utf-8 -*-
 #
 # Configuration file for the Sphinx documentation builder.
 #
 # This file does only contain a selection of the most common options. For a
 # full list see the documentation:
 # http://www.sphinx-doc.org/en/master/config
 
-# -- Path setup --------------------------------------------------------------
-
-# If extensions (or modules to document with autodoc) are in another directory,
-# add these directories to sys.path here. If the directory is relative to the
-# documentation root, use os.path.abspath to make it absolute, like shown here.
-#
-# import os
-# import sys
-# sys.path.insert(0, os.path.abspath('.'))
-
+import importlib.metadata
+import re
 
 # -- Project information -----------------------------------------------------
 
-project = u'mkpkg'
-copyright = u'2019, Julian Berman'
-author = u'Julian Berman'
-
-# The short X.Y version
-version = u''
-# The full version, including alpha/beta/rc tags
-release = u''
+project = "mkpkg"
+author = "Julian Berman"
+copyright = "2019, " + author
+
+# version: The short X.Y version
+# release: The full version, including alpha/beta/rc tags.
+release = importlib.metadata.version("mkpkg")
+version = release.partition("-")[0]
 
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
-# needs_sphinx = '1.0'
+# needs_sphinx = "1.0"
+
+default_role = "any"
 
 # Add any Sphinx extension module names here, as strings. They can be
-# extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
+# extensions coming with Sphinx (named "sphinx.ext.*") or your custom
 # ones.
 extensions = [
-    'sphinx.ext.autodoc',
-    'sphinx.ext.autosectionlabel',
-    'sphinx.ext.coverage',
-    'sphinx.ext.doctest',
-    'sphinx.ext.intersphinx',
-    'sphinx.ext.viewcode',
-    'sphinx.ext.napoleon',
-    'sphinxcontrib.spelling',
+    "sphinx.ext.autodoc",
+    "sphinx.ext.autosectionlabel",
+    "sphinx.ext.coverage",
+    "sphinx.ext.doctest",
+    "sphinx.ext.intersphinx",
+    "sphinx.ext.napoleon",
+    "sphinx.ext.viewcode",
+    "sphinxcontrib.spelling",
 ]
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
+templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 #
-# source_suffix = ['.rst', '.md']
-source_suffix = '.rst'
+# source_suffix = [".rst", ".md"]
+source_suffix = ".rst"
 
 # The master toctree document.
-master_doc = 'index'
+master_doc = "index"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = None
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
-exclude_patterns = [u'_build', 'Thumbs.db', '.DS_Store']
+exclude_patterns = ["_build", "_static", "Thumbs.db", ".DS_Store"]
 
 # The name of the Pygments (syntax highlighting) style to use.
-pygments_style = None
+pygments_style = "sphinx"
 
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = 'alabaster'
+html_theme = "furo"
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 #
 # html_theme_options = {}
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
+# html_static_path = ["_static"]
 
 # Custom sidebar templates, must be a dictionary that maps document names
 # to template names.
 #
 # The default sidebars (for documents that don't match any pattern) are
 # defined by theme itself.  Builtin themes are using these templates by
-# default: ``['localtoc.html', 'relations.html', 'sourcelink.html',
-# 'searchbox.html']``.
+# default: ``["localtoc.html", "relations.html", "sourcelink.html",
+# "searchbox.html"]``.
 #
 # html_sidebars = {}
 
 
 # -- Options for HTMLHelp output ---------------------------------------------
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = 'mkpkgdoc'
+htmlhelp_basename = "mkpkgdoc"
 
 
 # -- Options for LaTeX output ------------------------------------------------
 
 latex_elements = {
-    # The paper size ('letterpaper' or 'a4paper').
+    # The paper size ("letterpaper" or "a4paper").
     #
-    # 'papersize': 'letterpaper',
-
-    # The font size ('10pt', '11pt' or '12pt').
+    # "papersize": "letterpaper",
+    # The font size ("10pt", "11pt" or "12pt").
     #
-    # 'pointsize': '10pt',
-
+    # "pointsize": "10pt",
     # Additional stuff for the LaTeX preamble.
     #
-    # 'preamble': '',
-
+    # "preamble": "",
     # Latex figure (float) alignment
     #
-    # 'figure_align': 'htbp',
+    # "figure_align": "htbp",
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title,
 #  author, documentclass [howto, manual, or own class]).
 latex_documents = [
-    (master_doc, 'mkpkg.tex', u'mkpkg Documentation',
-     u'Julian Berman', 'manual'),
+    (
+        master_doc,
+        "mkpkg.tex",
+        "mkpkg Documentation",
+        author,
+        "manual",
+    ),
 ]
 
 
 # -- Options for manual page output ------------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
 man_pages = [
-    (master_doc, 'mkpkg', u'mkpkg Documentation',
-     [author], 1)
+    (
+        master_doc,
+        "mkpkg",
+        "mkpkg Documentation",
+        [author],
+        1,
+    ),
 ]
 
 
 # -- Options for Texinfo output ----------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
-    (master_doc, 'mkpkg', u'mkpkg Documentation',
-     author, 'mkpkg', 'One line description of project.',
-     'Miscellaneous'),
+    (
+        master_doc,
+        "mkpkg",
+        "mkpkg Documentation",
+        author,
+        "mkpkg",
+        "",
+        "Miscellaneous",
+    ),
 ]
 
 
 # -- Options for Epub output -------------------------------------------------
 
 # Bibliographic Dublin Core info.
 epub_title = project
 
 # The unique identifier of the text. This can be a ISBN number
 # or the project homepage.
 #
-# epub_identifier = ''
+# epub_identifier = ""
 
 # A unique identification for the text.
 #
-# epub_uid = ''
+# epub_uid = ""
 
 # A list of files that should not be packed into the epub file.
-epub_exclude_files = ['search.html']
+epub_exclude_files = ["search.html"]
 
 
 # -- Extension configuration -------------------------------------------------
 
 # Prefix each section label with the name of the document it is in
 # autosectionlabel_prefix_document = False
 
 # Limit the depth that autogenerated refs are created for
 # autosectionlabel_maxdepth = None
 
 # -- Options for intersphinx extension ---------------------------------------
 
 # Example configuration for intersphinx: refer to the Python standard library.
-intersphinx_mapping = {'https://docs.python.org/': None}
+intersphinx_mapping = {"https://docs.python.org/": None}
+
+# -- Options for the linkcheck builder ------------------------------------
+
+
+def entire_domain(host):
+    return r"http.?://" + re.escape(host) + r"($|/.*)"
+
+
+linkcheck_ignore = [
+    "https://github.com/Julian/mkpkg/actions",
+    "https://github.com/Julian/mkpkg/workflows/CI/badge.svg",
+]
```

### Comparing `mkpkg-0.9.0/COPYING` & `mkpkg-2023.5.1/COPYING`

 * *Files identical despite different names*

### Comparing `mkpkg-0.9.0/tox.ini` & `mkpkg-2023.5.1/tox.ini`

 * *Files 24% similar despite different names*

```diff
@@ -1,108 +1,89 @@
 [tox]
+min_version = 4.0.9
 envlist =
-    py36
-    py37
-    pypy2
-    pypy3
+    py{38,39,310,311,py3}-{build,audit,tests}
     readme
-    safety
     secrets
     style
-    docs-{html,doctest,linkcheck,spelling,style}
+    docs-{dirhtml,doctest,linkcheck,spelling,style}
 skipsdist = True
 
 [testenv]
-setenv =
 changedir = {envtmpdir}
-commands =
-    {envbindir}/pip install {toxinidir}
-    {envbindir}/trial {posargs:mkpkg}
-    {envpython} -m doctest {toxinidir}/README.rst
-deps =
-    -r{toxinidir}/test-requirements.txt
-    twisted
-    codecov,coverage: coverage
-
-[testenv:coverage]
+passenv = CI, GITHUB_STEP_SUMMARY
 setenv =
-    {[testenv]setenv}
-    COVERAGE_FILE={envtmpdir}/coverage-data
-commands =
-    {envbindir}/pip install {toxinidir}
-    {envbindir}/coverage run --rcfile={toxinidir}/.coveragerc {envbindir}/trial mkpkg
-    {envbindir}/coverage report --rcfile={toxinidir}/.coveragerc --show-missing
-    {envbindir}/coverage html --directory={envtmpdir}/htmlcov --rcfile={toxinidir}/.coveragerc {posargs}
+    TOX_PARALLEL_NO_SPINNER = 1
 
-[testenv:readme]
-changedir = {toxinidir}
-deps = readme_renderer
-commands =
-    {envbindir}/python setup.py check --restructuredtext --strict
+    coverage,ghcoverage: MAYBE_COVERAGE=coverage run -m
+    coverage,ghcoverage: COVERAGE_RCFILE={toxinidir}/.coveragerc
+    coverage,ghcoverage: COVERAGE_DEBUG_FILE={envtmpdir}/coverage-debug
+    coverage,ghcoverage: COVERAGE_FILE={envtmpdir}/coverage-data
+args_are_paths = false
+commands =
+    build: {envpython} -m build {toxinidir} --outdir {envtmpdir}/dist
+    !build: {envpython} -m pip install --disable-pip-version-check {toxinidir}
+
+    audit: {envpython} -m pip_audit
+
+    tests,coverage,ghcoverage: {envpython} -m {env:MAYBE_COVERAGE:} virtue {posargs:mkpkg}
+    tests: {envpython} -m doctest {toxinidir}/README.rst
+
+    coverage: {envpython} -m coverage report --show-missing
+    coverage: {envpython} -m coverage html --directory={envtmpdir}/htmlcov
+deps =
+    audit: pip-audit
+    build: build
+    tests,coverage,ghcoverage: virtue
+    tests,coverage,ghcoverage: -r{toxinidir}/test-requirements.txt
+    coverage,ghcoverage: coverage
+
+[testenv:bandit]
+deps = bandit
+commands = {envpython} -m bandit --recursive {toxinidir}/mkpkg
 
-[testenv:safety]
-deps = safety
+[testenv:readme]
+deps =
+    build
+    twine
 commands =
-    {envbindir}/pip install {toxinidir}
-    {envbindir}/safety check
+    {envpython} -m build --outdir {envtmpdir}/dist {toxinidir}
+    {envpython} -m twine check {envtmpdir}/dist/*
 
 [testenv:secrets]
 deps = detect-secrets
 commands = {envbindir}/detect-secrets scan {toxinidir}
 
 [testenv:style]
-basepython = python2
-deps = ebb-lint
-commands =
-    {envbindir}/flake8 {posargs} --max-complexity 12 {toxinidir}/mkpkg {toxinidir}/setup.py
-
-[testenv:docs-html]
-changedir = docs
-whitelist_externals = make
-commands = make -f {toxinidir}/docs/Makefile BUILDDIR={envtmpdir}/build SPHINXOPTS='-a -c {toxinidir}/docs/ -n -T -W {posargs}' html
 deps =
-    -r{toxinidir}/docs/requirements.txt
-    {toxinidir}
+    flake8
+    flake8-broken-line
+    flake8-bugbear
+    flake8-commas
+    flake8-quotes
+    flake8-tidy-imports
+commands =
+    {envpython} -m flake8 {posargs} {toxinidir}/mkpkg
+
+[testenv:docs-dirhtml]
+commands = {envpython} -m sphinx -b dirhtml {toxinidir}/docs/ {envtmpdir}/build {posargs:-a -n -q -T -W}
+deps = -r{toxinidir}/docs/requirements.txt
 
 [testenv:docs-doctest]
-changedir = docs
-whitelist_externals = make
-commands = make -f {toxinidir}/docs/Makefile BUILDDIR={envtmpdir}/build SPHINXOPTS='-a -c {toxinidir}/docs/ -n -T -W {posargs}' doctest
-deps =
-    -r{toxinidir}/docs/requirements.txt
-    {toxinidir}
+commands = {envpython} -m sphinx -b doctest {toxinidir}/docs/ {envtmpdir}/build {posargs:-a -n -q -T -W}
+deps = {[testenv:docs-dirhtml]deps}
 
 [testenv:docs-linkcheck]
-changedir = docs
-whitelist_externals = make
-commands = make -f {toxinidir}/docs/Makefile BUILDDIR={envtmpdir}/build SPHINXOPTS='-a -c {toxinidir}/docs/ -n -T -W {posargs}' linkcheck
-deps =
-    -r{toxinidir}/docs/requirements.txt
-    {toxinidir}
+commands = {envpython} -m sphinx -b linkcheck {toxinidir}/docs/ {envtmpdir}/build {posargs:-a -n -q -T -W}
+deps = {[testenv:docs-dirhtml]deps}
 
 [testenv:docs-spelling]
-changedir = docs
-whitelist_externals = make
-commands = make -f {toxinidir}/docs/Makefile BUILDDIR={envtmpdir}/build SPHINXOPTS='-a -c {toxinidir}/docs/ -n -T -W {posargs}' spelling
-deps =
-    -r{toxinidir}/docs/requirements.txt
-    {toxinidir}
+commands = {envpython} -m sphinx -b spelling {toxinidir}/docs/ {envtmpdir}/build {posargs:-a -n -T -W}
+deps = {[testenv:docs-dirhtml]deps}
 
 [testenv:docs-style]
-changedir = docs
-commands = doc8 {posargs} {toxinidir}/docs
+commands =
+  doc8 --max-line-length 1000 --ignore-path {toxinidir}/docs/requirements.txt {posargs} {toxinidir}/docs
 deps =
     doc8
     pygments
     pygments-github-lexers
-
-[testenv:codecov]
-passenv = CODECOV* CI TRAVIS TRAVIS_*
-setenv =
-    {[testenv]setenv}
-    COVERAGE_DEBUG_FILE={envtmpdir}/coverage-debug
-    COVERAGE_FILE={envtmpdir}/coverage-data
-commands =
-    {envbindir}/pip install {toxinidir}
-    {envbindir}/coverage run --rcfile={toxinidir}/.coveragerc {envbindir}/trial mkpkg
-    {envbindir}/coverage xml -o {envtmpdir}/coverage.xml
-    {envbindir}/codecov --required --disable gcov --file {envtmpdir}/coverage.xml
```

### Comparing `mkpkg-0.9.0/README.rst` & `mkpkg-2023.5.1/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,24 @@
-=====
-mkpkg
-=====
+=========
+``mkpkg``
+=========
 
-|PyPI| |Pythons| |Travis| |AppVeyor| |Codecov| |ReadTheDocs|
+|PyPI| |Pythons| |CI| |ReadTheDocs|
 
 .. |PyPI| image:: https://img.shields.io/pypi/v/mkpkg.svg
    :alt: PyPI version
    :target: https://pypi.org/project/mkpkg/
 
 .. |Pythons| image:: https://img.shields.io/pypi/pyversions/mkpkg.svg
    :alt: Supported Python versions
    :target: https://pypi.org/project/mkpkg/
 
-.. |Travis| image:: https://travis-ci.org/Julian/mkpkg.svg?branch=master
-   :alt: Travis build status
-   :target: https://travis-ci.org/Julian/mkpkg
-
-.. |AppVeyor| image:: https://ci.appveyor.com/api/projects/status/n0ddnkcr1xh2j1fu?svg=true
-   :alt: AppVeyor build status
-   :target: https://ci.appveyor.com/project/Julian/mkpkg
-
-.. |Codecov| image:: https://codecov.io/gh/Julian/mkpkg/branch/master/graph/badge.svg
-   :alt: Codecov Code coverage
-   :target: https://codecov.io/gh/Julian/mkpkg
+.. |CI| image:: https://github.com/Julian/mkpkg/workflows/CI/badge.svg
+  :alt: Build status
+  :target: https://github.com/Julian/mkpkg/actions?query=workflow%3ACI
 
 .. |ReadTheDocs| image:: https://readthedocs.org/projects/mkpkg/badge/?version=stable&style=flat
    :alt: ReadTheDocs status
    :target: https://mkpkg.readthedocs.io/en/stable/
 
 
 A package I (`Julian <https://github.com/Julian>`_) use to create Python packages.
```

### Comparing `mkpkg-0.9.0/mkpkg/_cli.py` & `mkpkg-2023.5.1/mkpkg/_cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,61 +1,52 @@
-#! /usr/bin/env python2
-
 from datetime import datetime
-import configparser
-import io
+from pathlib import Path
+from random import randint
+from textwrap import dedent
 import os
 import pwd
-import sys
 import subprocess
+import sys
 import textwrap
 
-try:
-    from pathlib import Path
-except ImportError:
-    from pathlib2 import Path
-
 import click
 import jinja2
 
-
 STATUS_CLASSIFIERS = {
     "planning": "Development Status :: 1 - Planning",
     "prealpha": "Development Status :: 2 - Pre-Alpha",
     "alpha": "Development Status :: 3 - Alpha",
     "beta": "Development Status :: 4 - Beta",
     "stable": "Development Status :: 5 - Production/Stable",
     "mature": "Development Status :: 6 - Mature",
     "inactive": "Development Status :: 7 - Inactive",
 }
 VERSION_CLASSIFIERS = {
-    "pypy": "Programming Language :: Python :: 2.7",
-    "pypy3": "Programming Language :: Python :: 3.6",
-
+    "pypy2": "Programming Language :: Python :: 2.7",
+    "pypy3": "Programming Language :: Python :: 3.8",
     "py27": "Programming Language :: Python :: 2.7",
     "py35": "Programming Language :: Python :: 3.5",
     "py36": "Programming Language :: Python :: 3.6",
     "py37": "Programming Language :: Python :: 3.7",
     "py38": "Programming Language :: Python :: 3.8",
     "py39": "Programming Language :: Python :: 3.9",
-
+    "py310": "Programming Language :: Python :: 3.10",
+    "py311": "Programming Language :: Python :: 3.11",
+    "py312": "Programming Language :: Python :: 3.12",
     "jython": "Programming Language :: Python :: 2.7",
 }
-TRAVIS_SUPPORTS = {
-    "py27": "2.7",
-    "py35": "3.5",
-    "py36": "3.6",
-    "py37": "3.7",
-    "py38": "3.8",
-    "py39": "3.9",
-}
 TEST_DEPS = {
-    "py.test": ["pytest"],
-    "trial": ["twisted"],
+    "pytest": ["pytest"],
+    "twisted.trial": ["twisted"],
+    "virtue": ["virtue"],
 }
+TEMPLATE = Path(__file__).with_name("template")
+
+PYPI_TOKEN_URL = "https://pypi.org/manage/account/token/"
+READTHEDOCS_IMPORT_URL = "https://readthedocs.org/dashboard/import/manual/"
 
 
 def dedented(*args, **kwargs):
     return textwrap.dedent(*args, **kwargs).lstrip("\n")
 
 
 @click.command()
@@ -80,24 +71,24 @@
     "--readme",
     default="",
     help="a (rst) README for the package",
 )
 @click.option(
     "-t",
     "--test-runner",
-    default="trial",
-    type=click.Choice(["pytest", "trial"]),
+    default="virtue",
+    type=click.Choice(TEST_DEPS.keys()),
     help="the test runner to use",
 )
 @click.option(
     "-s",
     "--supports",
     multiple=True,
     type=click.Choice(sorted(VERSION_CLASSIFIERS)),
-    default=["py36", "py37", "pypy", "pypy3"],
+    default=["py38", "py39", "py310", "py311", "pypy3"],
     help="a version of Python supported by the package",
 )
 @click.option(
     "--status",
     type=click.Choice(STATUS_CLASSIFIERS),
     default="alpha",
     help="the initial package development status",
@@ -118,14 +109,19 @@
 @click.option(
     "--bare/--no-bare",
     "bare",
     default=False,
     help="only create the core source files.",
 )
 @click.option(
+    "--cffi/--no-cffi",
+    default=False,
+    help="include a build script for CFFI modules",
+)
+@click.option(
     "--style/--no-style",
     "style",
     default=True,
     help="(don't) run pyflakes by default in tox runs.",
 )
 @click.option(
     "--init-vcs/--no-init-vcs",
@@ -133,18 +129,20 @@
     help="don't initialize a VCS.",
 )
 @click.option(
     "--closed/--open",
     default=False,
     help="create a closed source package.",
 )
+@click.version_option(prog_name="mkpkg")
 def main(
     name,
     author,
     author_email,
+    cffi,
     cli,
     readme,
     test_runner,
     supports,
     status,
     docs,
     single_module,
@@ -154,258 +152,265 @@
     closed,
 ):
     """
     Oh how exciting! Create a new Python package.
     """
 
     if name.startswith("python-"):
-        package_name = name[len("python-"):]
+        package_name = name[len("python-") :]
+    elif name.endswith(".py"):
+        package_name = name[: -len(".py")]
     else:
         package_name = name
     package_name = package_name.lower().replace("-", "_")
 
-    root = Path(name)
+    env = jinja2.Environment(
+        loader=jinja2.PackageLoader("mkpkg", "template"),
+        undefined=jinja2.StrictUndefined,
+        keep_trailing_newline=True,
+    )
+    env.globals.update(
+        author=author,
+        cffi=cffi,
+        cli=cli,
+        closed=closed,
+        docs=docs,
+        name=name,
+        now=datetime.now(),
+        package_name=package_name,
+        single_module=single_module,
+        style=style,
+        supports=supports,
+        test_runner=test_runner,
+    )
+
     package = Path(package_name)
 
     if single_module:
-        contents = u"py_modules", name
-        tests = u"{toxinidir}/tests.py"
+        tests = "{toxinidir}/tests.py"
 
         if len(cli) > 1:
             sys.exit("Cannot create a single module with multiple CLIs.")
         elif cli:
-            console_scripts = [u"{} = {}:main".format(cli[0], package_name)]
-            script = u"""
-            import click
-
-
-            @click.command()
-            def main():
-                pass
-            """
+            scripts = [f'{cli[0]} = "{package_name}:main"']
+            script = env.get_template("package/_cli.py.j2").render(
+                program_name=cli[0],
+            )
         else:
-            console_scripts = []
-            script = u""
+            scripts = []
+            script = ""
 
+        script_name = package_name + ".py"
         core_source_paths = {
-            package_name + ".py": script,
-            "tests.py": render(
-                "tests.py",
-                name=name,
-                package_name=package_name,
-            ),
+            script_name: script,
+            "tests.py": env.get_template("tests.py.j2").render(),
         }
+        style_paths = ["{toxinidir}/" + script_name, tests]
 
     else:
-        contents = u"packages", u"find:"
         tests = package_name
 
         core_source_paths = {
-            package / "tests" / "__init__.py": u"",
-            package / "__init__.py": template("package", "__init__.py"),
+            package / "tests" / "__init__.py": "",
+            package
+            / "__init__.py": env.get_template(
+                "package/__init__.py.j2",
+            ).render(),
         }
+        style_paths = ["{toxinidir}/" + package_name]
+
+        if cffi:
+            core_source_paths[package / "_build.py"] = env.get_template(
+                "package/_build.py.j2",
+            ).render(cname=_cname(name))
 
         if len(cli) == 1:
-            console_scripts = [
-                "{} = {}._cli:main".format(cli[0], package_name),
-            ]
-            core_source_paths[package / "_cli.py"] = render(
-                "package", "_cli.py",
-                package_name=package_name,
-                cli=cli[0],
-            )
-            core_source_paths[package / "__main__.py"] = render(
-                "package", "__main__.py", package_name=package_name,
-            )
+            scripts = [f'{cli[0]} = "{package_name}._cli:main"']
+            core_source_paths[package / "_cli.py"] = env.get_template(
+                "package/_cli.py.j2",
+            ).render(program_name=cli[0])
+            core_source_paths[package / "__main__.py"] = env.get_template(
+                "package/__main__.py.j2",
+            ).render()
         else:
-            console_scripts = [
-                "{each} = {package_name}._{each}:main".format(
-                    each=each, package_name=package_name,
-                ) for each in cli
+            scripts = [
+                f'{each} = "{package_name}._{each}:main"' for each in cli
             ]
             core_source_paths.update(
                 (
                     package / ("_" + each + ".py"),
-                    render(
-                        "package",
-                        "_cli.py",
-                        package_name=package_name,
-                        cli=each,
+                    env.get_template("package/_cli.py.j2").render(
+                        program_name=each,
                     ),
-                ) for each in cli
+                )
+                for each in cli
             )
 
+    dependencies = []
+    if cffi:
+        dependencies.append("cffi>=1.0.0")
+    if scripts:
+        dependencies.append("click")
+
     files = {
-        "README.rst": render(
-            "README.rst",
-            name=name,
+        "README.rst": env.get_template("README.rst.j2").render(
             contents=readme,
-            closed=closed,
-            docs=docs,
         ),
-        "COPYING": render(
-            "COPYING", now=datetime.now(), author=author, closed=closed,
-        ),
-        "MANIFEST.in": template("MANIFEST.in"),
-        "setup.cfg": render(
-            "setup.cfg",
-            package_name=package_name,
-            contents=contents,
-            name=name,
-            author=author,
-            console_scripts=console_scripts,
-            single_module=single_module,
+        "COPYING": env.get_template("COPYING.j2").render(),
+        "pyproject.toml": env.get_template("pyproject.toml.j2").render(
+            dependencies=dependencies,
+            scripts=scripts,
             author_email=(
-                author_email or u"Julian+" + package_name + u"@GrayVines.com"
+                author_email or "Julian+" + package_name + "@GrayVines.com"
             ),
             status_classifier=STATUS_CLASSIFIERS[status],
             version_classifiers={
                 VERSION_CLASSIFIERS[each]
                 for each in supports
                 if each in VERSION_CLASSIFIERS
             },
-            closed=closed,
-            supports=supports,
             py2=any(
-                version.startswith("py2")
-                or version in {"jython", "pypy"}
+                version.startswith("py2") or version in {"jython", "pypy2"}
                 for version in supports
             ),
             py3=any(
-                version.startswith("py3")
-                or version == "pypy3"
+                version.startswith("py3") or version == "pypy3"
                 for version in supports
             ),
             cpython=any(
-                version not in {"jython", "pypy", "pypy3"}
+                version not in {"jython", "pypy2", "pypy3"}
                 for version in supports
             ),
-            pypy="pypy" in supports or "pypy3" in supports,
+            pypy="pypy2" in supports or "pypy3" in supports,
             jython="jython" in supports,
         ),
-        "setup.py": template("setup.py"),
-        ".coveragerc": render(".coveragerc", package_name=package_name),
-        "tox.ini": render(
-            "tox.ini",
-            name=name,
-            package_name=package_name,
-            supports=supports,
-            closed=closed,
-            docs=docs,
-            style=style,
+        ".coveragerc": env.get_template(".coveragerc.j2").render(),
+        "tox.ini": env.get_template("tox.ini.j2").render(
             test_deps=TEST_DEPS[test_runner],
-            test_runner=test_runner,
             tests=tests,
+            style_paths=style_paths,
         ),
+        ".flake8": template(".flake8"),
+        ".pre-commit-config.yaml": template(".pre-commit-config.yaml"),
         ".testr.conf": template(".testr.conf"),
     }
 
     if not closed:
-        files.update(
-            {
-                ".travis.yml": render(
-                    ".travis.yml",
-                    travis_supports=sorted(
-                        TRAVIS_SUPPORTS.get(each, each)
-                        for each in supports
-                    ),
-                ),
-                "codecov.yml": template("codecov.yml"),
-            },
+        files[".github/workflows/ci.yml"] = env.get_template(
+            ".github/workflows/ci.yml.j2",
+        ).render(
+            schedule_hour=randint(3, 7),
+            schedule_minute=randint(0, 59),
         )
+        files[".github/dependabot.yml"] = template(".github/dependabot.yml")
+        files[".github/FUNDING.yml"] = template(".github/FUNDING.yml")
+        files[".github/SECURITY.md"] = env.get_template(
+            ".github/SECURITY.md.j2",
+        ).render()
 
+    root = Path(name)
     if bare:
         targets = core_source_paths
     else:
         files.update(core_source_paths)
         targets = files
         root.mkdir()
 
     for path, content in targets.items():
         path = root / path
         path.parent.mkdir(parents=True, exist_ok=True)
         path.write_text(dedented(content))
 
     if docs:
         (root / "docs").mkdir()
-        (root / "docs" / "requirements.txt").write_text(
-            template("docs", "requirements.txt"),
+        (root / "docs" / "requirements.in").write_text(
+            template("docs", "requirements.in"),
         )
 
         subprocess.check_call(
             [
                 sys.executable,
-                "-m", "sphinx.cmd.quickstart",
+                "-m",
+                "sphinx.cmd.quickstart",
                 "--quiet",
-                "--project", name,
-                "--author", author,
-                "--release", "",
+                "--project",
+                name,
+                "--author",
+                author,
+                "--release",
+                "",
                 "--ext-autodoc",
                 "--ext-coverage",
                 "--ext-doctest",
                 "--ext-intersphinx",
                 "--ext-viewcode",
-                "--extensions", "sphinx.ext.napoleon",
-                "--extensions", "sphinxcontrib.spelling",
+                "--extensions",
+                "sphinx.ext.napoleon",
+                "--extensions",
+                "sphinxcontrib.spelling",
                 "--makefile",
                 "--no-batchfile",
                 str(root / "docs"),
             ],
         )
-        (root / "docs" / "index.rst").write_text(
-            render("docs", "index.rst", README=files["README.rst"]),
-        )
+
+        # Fix sphinx-quickstart not writing a trailing newline.
+        with root.joinpath("docs", "conf.py").open("a") as file:
+            file.write("\n")
+
+        (root / "docs" / "index.rst").write_text(template("docs", "index.rst"))
+
+        click.echo(f"Set up documentation at: {READTHEDOCS_IMPORT_URL}")
 
     if init_vcs and not bare:
-        subprocess.check_call(["git", "init", name])
+        subprocess.check_call(["git", "init", "--quiet", name])
 
         git_dir = root / ".git"
         subprocess.check_call(
             [
                 "git",
-                "--git-dir", str(git_dir),
-                "--work-tree", name,
-                "add", "COPYING",
-            ])
+                "--git-dir",
+                str(git_dir),
+                "--work-tree",
+                name,
+                "add",
+                "COPYING",
+            ]
+        )
         subprocess.check_call(
             [
                 "git",
-                "--git-dir", str(git_dir),
-                "commit", "-m", "Initial commit",
+                "--git-dir",
+                str(git_dir),
+                "commit",
+                "--quiet",
+                "-m",
+                "Initial commit",
             ],
         )
 
-
-def ini(*sections, **kwargs):
-    """
-    Construct an INI-formatted str with the given contents.
-    """
-
-    lol_python = io.StringIO()
-    parser = configparser.ConfigParser(**kwargs)
-    for section, contents in sections:
-        parser.add_section(section)
-        for option, value in contents:
-            if isinstance(value, list):
-                value = u"\n" + u"\n".join(value)
-            parser.set(section, option, value)
-    parser.write(lol_python)
-    value = lol_python.getvalue().replace(
-        u"\t", u"    ",
-    ).replace(
-        u"= \n", u"=\n",
-    )
-    return value[:-1]
+        if not closed:
+            click.echo(
+                dedent(
+                    f"""
+                    Set up:
+
+                      * a PyPI token from {PYPI_TOKEN_URL} named
+                        'GitHub Actions - {name}'
+
+                    and include them in the GitHub secrets at
+                    https://github.com/Julian/{name}/settings/secrets
+                    """,
+                ),
+            )
 
 
 def template(*segments):
-    path = Path(__file__).with_name("template").joinpath(*segments)
-    return path.read_text()
+    return TEMPLATE.joinpath(*segments).read_text()
 
 
-def render(*segments, **values):
-    segments = segments[:-1] + (segments[-1] + ".j2",)
-    return jinja2.Template(
-        template(*segments),
-        undefined=jinja2.StrictUndefined,
-        keep_trailing_newline=True,
-    ).render(values)
+def _cname(name):
+    if name.endswith("-cffi"):
+        name = name[: -len("-cffi")]
+    if name.startswith("lib"):
+        name = name[len("lib") :]
+    return "_" + name
```

### Comparing `mkpkg-0.9.0/mkpkg/template/README.rst.j2` & `mkpkg-2023.5.1/mkpkg/template/README.rst.j2`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,25 @@
-{{ "=" * name | length }}
-{{ name }}
-{{ "=" * name | length }}
+=={{ "=" * name | length }}==
+``{{ name }}``
+=={{ "=" * name | length }}==
 {% if not closed %}
-|PyPI| |Pythons| |Travis| |Codecov|{% if docs %} |ReadTheDocs|{% endif %}
+|PyPI| |Pythons| |CI|{% if docs %} |ReadTheDocs|{% endif %}
 
 .. |PyPI| image:: https://img.shields.io/pypi/v/{{ name }}.svg
   :alt: PyPI version
   :target: https://pypi.org/project/{{ name }}/
 
 .. |Pythons| image:: https://img.shields.io/pypi/pyversions/{{ name }}.svg
   :alt: Supported Python versions
   :target: https://pypi.org/project/{{ name }}/
 
-.. |Travis| image:: https://travis-ci.org/Julian/{{ name }}.svg?branch=master
-  :alt: Travis build status
-  :target: https://travis-ci.org/Julian/{{ name }}
+.. |CI| image:: https://github.com/Julian/{{ name }}/workflows/CI/badge.svg
+  :alt: Build status
+  :target: https://github.com/Julian/{{ name }}/actions?query=workflow%3ACI
 
-.. |Codecov| image:: https://codecov.io/gh/Julian/{{ name }}/branch/master/graph/badge.svg
-  :alt: Codecov Code coverage
-  :target: https://codecov.io/gh/Julian/{{ name }}
 {% if docs %}
 .. |ReadTheDocs| image:: https://readthedocs.org/projects/{{ name }}/badge/?version=stable&style=flat
   :alt: ReadTheDocs status
   :target: https://{{ name }}.readthedocs.io/en/stable/
 {% endif -%}
 {% endif -%}
 {% if contents %}
```

### Comparing `mkpkg-0.9.0/mkpkg/template/tox.ini.j2` & `mkpkg-2023.5.1/mkpkg/template/tox.ini.j2`

 * *Files 22% similar despite different names*

```diff
@@ -1,87 +1,79 @@
 [tox]
 envlist =
-    {% for env in supports | sort -%}
-    {{ env }}
-    {% endfor -%}
+    {{ '{' }}{{ supports | sort | join(',') }}{{ '}' }}-{build,audit,tests}
     readme
-    safety
     secrets
     {% if style -%}style{%- endif %}
-    {% if docs -%}docs-{html,doctest,linkcheck,spelling,style}{%- endif %}
+    {% if docs -%}docs-{dirhtml,doctest,linkcheck,spelling,style}{%- endif %}
 skipsdist = True
 
 [testenv]
-setenv =
 changedir = {envtmpdir}
-commands =
-    {envbindir}/pip install {toxinidir}
-    {envbindir}/{{ test_runner }} {posargs:{{ tests }}}
-    {envpython} -m doctest {toxinidir}/README.rst
+passenv = CI, GITHUB_STEP_SUMMARY
+setenv =
+    coverage,ghcoverage: MAYBE_COVERAGE=coverage run -m
+    coverage,ghcoverage: COVERAGE_RCFILE={toxinidir}/.coveragerc
+    coverage,ghcoverage: COVERAGE_DEBUG_FILE={envtmpdir}/coverage-debug
+    coverage,ghcoverage: COVERAGE_FILE={envtmpdir}/coverage-data
+args_are_paths = false
+commands =
+    build: {envpython} -m build {toxinidir} --outdir {envtmpdir}/dist
+    !build: {envpython} -m pip install --disable-pip-version-check {toxinidir}
+
+    audit: {envpython} -m pip_audit
+
+    tests,coverage,ghcoverage: {envpython} -m {env:MAYBE_COVERAGE:} {{ test_runner }} {posargs:{{ tests }}}
+    tests: {envpython} -m doctest {toxinidir}/README.rst
+
+    coverage: {envpython} -m coverage report --show-missing
+    coverage: {envpython} -m coverage html --directory={envtmpdir}/htmlcov
 deps =
+    audit: pip-audit
+    build: build
     {% for each in test_deps -%}
-    {{ each }}
+    tests,coverage,ghcoverage: {{ each }}
     {%- endfor %}
-    {% if not closed %}codecov,{% endif %}coverage: coverage
+    coverage,ghcoverage: coverage
 
-[testenv:coverage]
-setenv =
-    {[testenv]setenv}
-    COVERAGE_FILE={envtmpdir}/coverage-data
-commands =
-    {envbindir}/pip install {toxinidir}
-    {envbindir}/coverage run --rcfile={toxinidir}/.coveragerc {envbindir}/{{ test_runner }} {{ tests }}
-    {envbindir}/coverage report --rcfile={toxinidir}/.coveragerc --show-missing
-    {envbindir}/coverage html --directory={envtmpdir}/htmlcov --rcfile={toxinidir}/.coveragerc {posargs}
+[testenv:bandit]
+deps = bandit
+commands = {envpython} -m bandit --recursive {{ tests }}
 
 [testenv:readme]
-changedir = {toxinidir}
-deps = readme_renderer
-commands =
-    {envbindir}/python setup.py check --restructuredtext --strict
-
-[testenv:safety]
-deps = safety
+deps =
+    build
+    twine
 commands =
-    {envbindir}/pip install {toxinidir}
-    {envbindir}/safety check
+    {envpython} -m build --outdir {envtmpdir}/dist {toxinidir}
+    {envpython} -m twine check {envtmpdir}/dist/*
 
 [testenv:secrets]
 deps = detect-secrets
 commands = {envbindir}/detect-secrets scan {toxinidir}
 
 [testenv:style]
-deps = ebb-lint
+deps =
+    flake8
+    flake8-broken-line
+    flake8-bugbear
+    flake8-commas
+    flake8-quotes
+    flake8-tidy-imports
 commands =
-  {envbindir}/flake8 {posargs} --max-complexity 10 {{ tests }} {toxinidir}/setup.py{% if docs %} {toxinidir}/docs
-{% for each in ["html", "doctest", "linkcheck", "spelling"] -%}
+    {envpython} -m flake8 {posargs} --max-complexity 10 {{ style_paths | join(' ') }}{% if cffi %} {toxinidir}/setup.py{% endif %}{% if docs %} {toxinidir}/docs
+{%- for each in ["dirhtml", "doctest", "linkcheck", "spelling"] %}
 
 [testenv:docs-{{ each }}]
-changedir = docs
-whitelist_externals = make
-commands = make -f {toxinidir}/docs/Makefile BUILDDIR={envtmpdir}/build SPHINXOPTS='-a -c {toxinidir}/docs/ -n -T -W {posargs}' {{ each }}
+commands = {envpython} -m sphinx -b {{ each }} {toxinidir}/docs/ {envtmpdir}/build {posargs:-a -n {% if each != 'spelling' %}-q {% endif %}-T -W}
 deps =
     -r{toxinidir}/docs/requirements.txt
-    {toxinidir}
-{% endfor %}
+{%- endfor %}
 
 [testenv:docs-style]
-changedir = docs
-commands = doc8 {posargs} {toxinidir}/docs
+commands =
+  doc8 --max-line-length 1000 --ignore-path {toxinidir}/docs/requirements.txt {posargs} {toxinidir}/docs
 deps =
     doc8
     pygments
     pygments-github-lexers
-{% endif %}
-{% if not closed %}
-[testenv:codecov]
-passenv = CODECOV* CI TRAVIS TRAVIS_*
-setenv =
-    {[testenv]setenv}
-    COVERAGE_DEBUG_FILE={envtmpdir}/coverage-debug
-    COVERAGE_FILE={envtmpdir}/coverage-data
-commands =
-    {envbindir}/pip install {toxinidir}
-    {envbindir}/coverage run --rcfile={toxinidir}/.coveragerc {envbindir}/{{ test_runner }} {{ tests }}
-    {envbindir}/coverage xml -o {envtmpdir}/coverage.xml
-    {envbindir}/codecov --required --disable gcov --file {envtmpdir}/coverage.xml
 {%- endif %}
```

### Comparing `mkpkg-0.9.0/mkpkg/template/COPYING.j2` & `mkpkg-2023.5.1/mkpkg/template/COPYING.j2`

 * *Files identical despite different names*

