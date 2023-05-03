# Comparing `tmp/Flask-Limiter-3.3.0.tar.gz` & `tmp/Flask-Limiter-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-Limiter-3.3.0.tar", last modified: Mon Feb 27 02:11:33 2023, max compression
+gzip compressed data, was "Flask-Limiter-3.3.1.tar", last modified: Wed May  3 23:50:02 2023, max compression
```

## Comparing `Flask-Limiter-3.3.0.tar` & `Flask-Limiter-3.3.1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 02:11:33.058814 Flask-Limiter-3.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/CLASSIFIERS
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/CONTRIBUTIONS.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 02:11:33.042812 Flask-Limiter-3.3.0/Flask_Limiter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5952 2023-02-27 02:11:33.000000 Flask-Limiter-3.3.0/Flask_Limiter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-02-27 02:11:33.000000 Flask-Limiter-3.3.0/Flask_Limiter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 02:11:33.000000 Flask-Limiter-3.3.0/Flask_Limiter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-02-27 02:11:33.000000 Flask-Limiter-3.3.0/Flask_Limiter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 02:11:32.000000 Flask-Limiter-3.3.0/Flask_Limiter.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-02-27 02:11:33.000000 Flask-Limiter-3.3.0/Flask_Limiter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-27 02:11:33.000000 Flask-Limiter-3.3.0/Flask_Limiter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    17611 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5952 2023-02-27 02:11:33.058814 Flask-Limiter-3.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 02:11:33.042812 Flask-Limiter-3.3.0/doc/
--rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 02:11:33.046813 Flask-Limiter-3.3.0/doc/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 02:11:33.054813 Flask-Limiter-3.3.0/doc/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/doc/source/_static/colors.css
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/doc/source/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/doc/source/_static/limiter.css
--rw-r--r--   0 runner    (1001) docker     (123)    27408 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/doc/source/_static/logo-og.png
--rw-r--r--   0 runner    (1001) docker     (123)    47774 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/doc/source/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)   183556 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/doc/source/_static/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15123 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/doc/source/_static/tap-icon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    15350 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/doc/source/_static/tap-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)   161289 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/doc/source/_static/tap-icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)    20934 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/doc/source/_static/tap-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/doc/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/doc/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/doc/source/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    10957 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/doc/source/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/doc/source/development.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14292 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/doc/source/misc.rst
--rw-r--r--   0 runner    (1001) docker     (123)    17227 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/doc/source/recipes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/doc/source/strategies.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/doc/source/theme_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 02:11:33.058814 Flask-Limiter-3.3.0/flask_limiter/
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/flask_limiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/flask_limiter/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-02-27 02:11:33.058814 Flask-Limiter-3.3.0/flask_limiter/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    22131 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/flask_limiter/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/flask_limiter/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 02:11:33.054813 Flask-Limiter-3.3.0/flask_limiter/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/flask_limiter/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/flask_limiter/contrib/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/flask_limiter/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    46697 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/flask_limiter/extension.py
--rw-r--r--   0 runner    (1001) docker     (123)    10493 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/flask_limiter/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/flask_limiter/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/flask_limiter/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/flask_limiter/util.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/flask_limiter/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5525 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/flask_limiter/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 02:11:33.054813 Flask-Limiter-3.3.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/requirements/main.txt
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-02-27 02:11:33.058814 Flask-Limiter-3.3.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1412 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 02:11:33.058814 Flask-Limiter-3.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    18681 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/tests/test_blueprints.py
--rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/tests/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/tests/test_context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    30256 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    11651 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/tests/test_error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)    24695 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/tests/test_flask_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/tests/test_regressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)    81180 2023-02-27 02:11:22.000000 Flask-Limiter-3.3.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:50:02.670694 Flask-Limiter-3.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/CLASSIFIERS
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/CONTRIBUTIONS.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:50:02.658694 Flask-Limiter-3.3.1/Flask_Limiter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-05-03 23:50:02.000000 Flask-Limiter-3.3.1/Flask_Limiter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-05-03 23:50:02.000000 Flask-Limiter-3.3.1/Flask_Limiter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 23:50:02.000000 Flask-Limiter-3.3.1/Flask_Limiter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-03 23:50:02.000000 Flask-Limiter-3.3.1/Flask_Limiter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 23:50:02.000000 Flask-Limiter-3.3.1/Flask_Limiter.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-03 23:50:02.000000 Flask-Limiter-3.3.1/Flask_Limiter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-03 23:50:02.000000 Flask-Limiter-3.3.1/Flask_Limiter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-05-03 23:50:02.670694 Flask-Limiter-3.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:50:02.658694 Flask-Limiter-3.3.1/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:50:02.658694 Flask-Limiter-3.3.1/doc/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:50:02.662694 Flask-Limiter-3.3.1/doc/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/doc/source/_static/colors.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/doc/source/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/doc/source/_static/limiter.css
+-rw-r--r--   0 runner    (1001) docker     (123)    27408 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/doc/source/_static/logo-og.png
+-rw-r--r--   0 runner    (1001) docker     (123)    47774 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/doc/source/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)   183556 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/doc/source/_static/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15123 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/doc/source/_static/tap-icon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    15350 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/doc/source/_static/tap-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)   161289 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/doc/source/_static/tap-icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    20934 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/doc/source/_static/tap-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/doc/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/doc/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/doc/source/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11025 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/doc/source/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/doc/source/development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14292 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/doc/source/misc.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    17227 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/doc/source/recipes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/doc/source/strategies.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/doc/source/theme_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:50:02.674694 Flask-Limiter-3.3.1/flask_limiter/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/flask_limiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/flask_limiter/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-03 23:50:02.674694 Flask-Limiter-3.3.1/flask_limiter/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22131 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/flask_limiter/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/flask_limiter/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:50:02.666694 Flask-Limiter-3.3.1/flask_limiter/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/flask_limiter/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/flask_limiter/contrib/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/flask_limiter/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46871 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/flask_limiter/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10493 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/flask_limiter/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/flask_limiter/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/flask_limiter/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/flask_limiter/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/flask_limiter/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5525 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/flask_limiter/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:50:02.670694 Flask-Limiter-3.3.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/requirements/main.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-03 23:50:02.670694 Flask-Limiter-3.3.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1412 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:50:02.670694 Flask-Limiter-3.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    18681 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/tests/test_blueprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/tests/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/tests/test_context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30256 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11651 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/tests/test_error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24695 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/tests/test_flask_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/tests/test_regressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81180 2023-05-03 23:49:53.000000 Flask-Limiter-3.3.1/versioneer.py
```

### Comparing `Flask-Limiter-3.3.0/Flask_Limiter.egg-info/PKG-INFO` & `Flask-Limiter-3.3.1/Flask_Limiter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: Flask-Limiter
-Version: 3.3.0
+Version: 3.3.1
 Summary: Rate limiting for flask applications
 Home-page: https://flask-limiter.readthedocs.org
 Author: Ali-Akber Saifee
 Author-email: ali@indydevs.org
 License: MIT
 Project-URL: Source, https://github.com/alisaifee/flask-limiter
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
+Classifier: Framework :: Flask
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `Flask-Limiter-3.3.0/Flask_Limiter.egg-info/SOURCES.txt` & `Flask-Limiter-3.3.1/Flask_Limiter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.3.0/HISTORY.rst` & `Flask-Limiter-3.3.1/HISTORY.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,22 @@
 .. :changelog:
 
 Changelog
 =========
 
+v3.3.1
+------
+Release Date: 2023-05-03
+
+* Chores
+
+  * Improve default limits documentation
+  * Update documentation dependencies
+  * Fix typing compatibility errors in headers
+
 v3.3.0
 ------
 Release Date: 2023-02-26
 
 * Bug Fix
 
   * Ensure per route limits are preferred (over application limits)
@@ -51,14 +61,18 @@
   * Remove deprecated config variable RATELIMIT_STORAGE_URL
   * Remove legacy backward compatibility path for flask < 2
 
 * Features
 
   * Allow scoping regular limit decorators / context managers
 
+v3.3.1
+------
+Release Date: 2023-05-03
+
 v3.3.0
 ------
 Release Date: 2023-02-26
 
 v3.2.0
 ------
 Release Date: 2023-02-15
@@ -78,14 +92,18 @@
   * Enforce key_func as a required argument
 
 * Chores
 
   * Simplify registration of decorated function & blueprint limits
 
 
+v3.3.1
+------
+Release Date: 2023-05-03
+
 v3.3.0
 ------
 Release Date: 2023-02-26
 
 v3.2.0
 ------
 Release Date: 2023-02-15
@@ -857,14 +875,15 @@
 
 
 
 
 
 
 
+
```

### Comparing `Flask-Limiter-3.3.0/LICENSE.txt` & `Flask-Limiter-3.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.3.0/PKG-INFO` & `Flask-Limiter-3.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: Flask-Limiter
-Version: 3.3.0
+Version: 3.3.1
 Summary: Rate limiting for flask applications
 Home-page: https://flask-limiter.readthedocs.org
 Author: Ali-Akber Saifee
 Author-email: ali@indydevs.org
 License: MIT
 Project-URL: Source, https://github.com/alisaifee/flask-limiter
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
+Classifier: Framework :: Flask
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `Flask-Limiter-3.3.0/README.rst` & `Flask-Limiter-3.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.3.0/doc/Makefile` & `Flask-Limiter-3.3.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.3.0/doc/source/_static/custom.css` & `Flask-Limiter-3.3.1/doc/source/_static/custom.css`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.3.0/doc/source/_static/logo-og.png` & `Flask-Limiter-3.3.1/doc/source/_static/logo-og.png`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.3.0/doc/source/_static/logo.png` & `Flask-Limiter-3.3.1/doc/source/_static/logo.png`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.3.0/doc/source/_static/logo.svg` & `Flask-Limiter-3.3.1/doc/source/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.3.0/doc/source/_static/tap-icon.ico` & `Flask-Limiter-3.3.1/doc/source/_static/tap-icon.ico`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.3.0/doc/source/_static/tap-icon.png` & `Flask-Limiter-3.3.1/doc/source/_static/tap-icon.png`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.3.0/doc/source/_static/tap-icon.svg` & `Flask-Limiter-3.3.1/doc/source/_static/tap-icon.svg`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.3.0/doc/source/_static/tap-logo.png` & `Flask-Limiter-3.3.1/doc/source/_static/tap-logo.png`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.3.0/doc/source/cli.rst` & `Flask-Limiter-3.3.1/doc/source/cli.rst`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.3.0/doc/source/conf.py` & `Flask-Limiter-3.3.1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.3.0/doc/source/configuration.rst` & `Flask-Limiter-3.3.1/doc/source/configuration.rst`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,16 @@
      - The cost of a hit to the application wide shared limit as an integer or a function
        that takes no parameters and returns the cost as an integer (Default: 1)
    * - .. data:: RATELIMIT_DEFAULT
 
        Constructor argument: :paramref:`~flask_limiter.Limiter.default_limits`
 
      - A comma (or some other delimiter) separated string that will be used to
-       apply a default limit on all routes. If not provided, the default limits can be
+       apply a default limit on all routes that are otherwise not decorated with
+       an explicit rate limit. If not provided, the default limits can be
        passed to the :class:`~flask_limiter.Limiter` constructor as well (the values passed to the
        constructor take precedence over those in the config).
        :ref:`ratelimit-string` for details.
    * - .. data:: RATELIMIT_DEFAULTS_PER_METHOD
 
        Constructor argument: :paramref:`~flask_limiter.Limiter.default_limits_per_method`
```

### Comparing `Flask-Limiter-3.3.0/doc/source/development.rst` & `Flask-Limiter-3.3.1/doc/source/development.rst`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.3.0/doc/source/index.rst` & `Flask-Limiter-3.3.1/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.3.0/doc/source/recipes.rst` & `Flask-Limiter-3.3.1/doc/source/recipes.rst`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.3.0/doc/source/strategies.rst` & `Flask-Limiter-3.3.1/doc/source/strategies.rst`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.3.0/doc/source/theme_config.py` & `Flask-Limiter-3.3.1/doc/source/theme_config.py`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.3.0/flask_limiter/commands.py` & `Flask-Limiter-3.3.1/flask_limiter/commands.py`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.3.0/flask_limiter/constants.py` & `Flask-Limiter-3.3.1/flask_limiter/constants.py`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.3.0/flask_limiter/errors.py` & `Flask-Limiter-3.3.1/flask_limiter/errors.py`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.3.0/flask_limiter/extension.py` & `Flask-Limiter-3.3.1/flask_limiter/extension.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,16 +66,16 @@
     """
     The :class:`Limiter` class initializes the Flask-Limiter extension.
 
     :param key_func: a callable that returns the domain to rate limit
       by.
     :param app: :class:`flask.Flask` instance to initialize the extension with.
     :param default_limits: a variable list of strings or callables
-     returning strings denoting default limits to apply to all routes.
-     :ref:`ratelimit-string` for  more details.
+     returning strings denoting default limits to apply to all routes that are
+     not explicitely decorated with a limit. :ref:`ratelimit-string` for  more details.
     :param default_limits_per_method: whether default limits are applied
      per method, per route or as a combination of all method per route.
     :param default_limits_exempt_when: a function that should return
      True/False to decide if the default limits should be skipped
     :param default_limits_deduct_when: a function that receives the
      current :class:`flask.Response` object and returns True/False to decide
      if a deduction should be made from the default rate limit(s)
@@ -805,15 +805,15 @@
         for lim, args in self.context.conditional_deductions.items():
             if lim.deduct_when and lim.deduct_when(response):
                 try:
                     self.limiter.hit(lim.limit, *args, cost=lim.cost)
                 except Exception as err:
                     if self._swallow_errors:
                         self.logger.exception(
-                            "Failed to deduct rate limit. " "Swallowing error"
+                            "Failed to deduct rate limit. Swallowing error"
                         )
                     else:
                         raise err
 
     def __inject_headers(
         self, response: flask.wrappers.Response
     ) -> flask.wrappers.Response:
@@ -828,17 +828,20 @@
             try:
                 reset_at = header_limit.reset_at
                 response.headers.add(
                     self._header_mapping[HeaderNames.LIMIT],
                     str(header_limit.limit.amount),
                 )
                 response.headers.add(
-                    self._header_mapping[HeaderNames.REMAINING], header_limit.remaining
+                    self._header_mapping[HeaderNames.REMAINING],
+                    str(header_limit.remaining),
+                )
+                response.headers.add(
+                    self._header_mapping[HeaderNames.RESET], str(reset_at)
                 )
-                response.headers.add(self._header_mapping[HeaderNames.RESET], reset_at)
 
                 # response may have an existing retry after
                 existing_retry_after_header = response.headers.get("Retry-After")
 
                 if existing_retry_after_header is not None:
                     # might be in http-date format
                     retry_after: Optional[Union[float, datetime.datetime]] = parse_date(
@@ -854,17 +857,19 @@
                         retry_after = time.mktime(retry_after.timetuple())
 
                     reset_at = max(int(retry_after), reset_at)
 
                 # set the header instead of using add
                 response.headers.set(
                     self._header_mapping[HeaderNames.RETRY_AFTER],
-                    self._retry_after == "http-date"
-                    and http_date(reset_at)
-                    or int(reset_at - time.time()),
+                    str(
+                        http_date(reset_at)
+                        if self._retry_after == "http-date"
+                        else int(reset_at - time.time())
+                    ),
                 )
             except Exception as e:  # noqa: E722
                 if self._in_memory_fallback_enabled and not self._storage_dead:
                     self.logger.warning(
                         "Rate limit storage unreachable - falling back to"
                         " in-memory storage"
                     )
```

### Comparing `Flask-Limiter-3.3.0/flask_limiter/manager.py` & `Flask-Limiter-3.3.1/flask_limiter/manager.py`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.3.0/flask_limiter/util.py` & `Flask-Limiter-3.3.1/flask_limiter/util.py`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.3.0/flask_limiter/wrappers.py` & `Flask-Limiter-3.3.1/flask_limiter/wrappers.py`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.3.0/setup.cfg` & `Flask-Limiter-3.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.3.0/setup.py` & `Flask-Limiter-3.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.3.0/tests/test_blueprints.py` & `Flask-Limiter-3.3.1/tests/test_blueprints.py`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.3.0/tests/test_commands.py` & `Flask-Limiter-3.3.1/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.3.0/tests/test_configuration.py` & `Flask-Limiter-3.3.1/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.3.0/tests/test_context_manager.py` & `Flask-Limiter-3.3.1/tests/test_context_manager.py`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.3.0/tests/test_decorators.py` & `Flask-Limiter-3.3.1/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.3.0/tests/test_error_handling.py` & `Flask-Limiter-3.3.1/tests/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.3.0/tests/test_flask_ext.py` & `Flask-Limiter-3.3.1/tests/test_flask_ext.py`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.3.0/tests/test_regressions.py` & `Flask-Limiter-3.3.1/tests/test_regressions.py`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.3.0/tests/test_storage.py` & `Flask-Limiter-3.3.1/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.3.0/tests/test_views.py` & `Flask-Limiter-3.3.1/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `Flask-Limiter-3.3.0/versioneer.py` & `Flask-Limiter-3.3.1/versioneer.py`

 * *Files identical despite different names*

