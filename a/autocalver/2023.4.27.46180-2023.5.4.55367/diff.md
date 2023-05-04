# Comparing `tmp/autocalver-2023.4.27.46180.tar.gz` & `tmp/autocalver-2023.5.4.55367.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autocalver-2023.4.27.46180.tar", last modified: Thu Apr 27 12:50:07 2023, max compression
+gzip compressed data, was "autocalver-2023.5.4.55367.tar", last modified: Thu May  4 15:23:16 2023, max compression
```

## Comparing `autocalver-2023.4.27.46180.tar` & `autocalver-2023.5.4.55367.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:50:07.956436 autocalver-2023.4.27.46180/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-27 12:49:55.000000 autocalver-2023.4.27.46180/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-27 12:49:55.000000 autocalver-2023.4.27.46180/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-04-27 12:50:07.956436 autocalver-2023.4.27.46180/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-04-27 12:49:55.000000 autocalver-2023.4.27.46180/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-27 12:50:07.000000 autocalver-2023.4.27.46180/git-log-head
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-27 12:49:55.000000 autocalver-2023.4.27.46180/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 12:50:07.956436 autocalver-2023.4.27.46180/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:50:07.952436 autocalver-2023.4.27.46180/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:50:07.952436 autocalver-2023.4.27.46180/src/autocalver/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-27 12:49:55.000000 autocalver-2023.4.27.46180/src/autocalver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-04-27 12:49:55.000000 autocalver-2023.4.27.46180/src/autocalver/integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:50:07.956436 autocalver-2023.4.27.46180/src/autocalver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-04-27 12:50:07.000000 autocalver-2023.4.27.46180/src/autocalver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-27 12:50:07.000000 autocalver-2023.4.27.46180/src/autocalver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 12:50:07.000000 autocalver-2023.4.27.46180/src/autocalver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-27 12:50:07.000000 autocalver-2023.4.27.46180/src/autocalver.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-27 12:50:07.000000 autocalver-2023.4.27.46180/src/autocalver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-27 12:50:07.000000 autocalver-2023.4.27.46180/src/autocalver.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:50:07.956436 autocalver-2023.4.27.46180/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-04-27 12:49:55.000000 autocalver-2023.4.27.46180/tests/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:23:16.893697 autocalver-2023.5.4.55367/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-04 15:23:05.000000 autocalver-2023.5.4.55367/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-04 15:23:05.000000 autocalver-2023.5.4.55367/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-05-04 15:23:16.893697 autocalver-2023.5.4.55367/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-05-04 15:23:05.000000 autocalver-2023.5.4.55367/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-04 15:23:16.000000 autocalver-2023.5.4.55367/git-log-head
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-04 15:23:05.000000 autocalver-2023.5.4.55367/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 15:23:16.893697 autocalver-2023.5.4.55367/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:23:16.889697 autocalver-2023.5.4.55367/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:23:16.893697 autocalver-2023.5.4.55367/src/autocalver/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-04 15:23:05.000000 autocalver-2023.5.4.55367/src/autocalver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-05-04 15:23:05.000000 autocalver-2023.5.4.55367/src/autocalver/integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:23:16.893697 autocalver-2023.5.4.55367/src/autocalver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-05-04 15:23:16.000000 autocalver-2023.5.4.55367/src/autocalver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-04 15:23:16.000000 autocalver-2023.5.4.55367/src/autocalver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 15:23:16.000000 autocalver-2023.5.4.55367/src/autocalver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-04 15:23:16.000000 autocalver-2023.5.4.55367/src/autocalver.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-04 15:23:16.000000 autocalver-2023.5.4.55367/src/autocalver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-04 15:23:16.000000 autocalver-2023.5.4.55367/src/autocalver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:23:16.893697 autocalver-2023.5.4.55367/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-05-04 15:23:05.000000 autocalver-2023.5.4.55367/tests/test_integration.py
```

### Comparing `autocalver-2023.4.27.46180/LICENSE` & `autocalver-2023.5.4.55367/LICENSE`

 * *Files identical despite different names*

### Comparing `autocalver-2023.4.27.46180/PKG-INFO` & `autocalver-2023.5.4.55367/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,13 @@
-Metadata-Version: 2.1
-Name: autocalver
-Version: 2023.4.27.46180
-Description-Content-Type: text/markdown
-Provides-Extra: tests
-Provides-Extra: lint
-Provides-Extra: mypy
-Provides-Extra: docs
-License-File: LICENSE
-
 # autocalver
 
+[![PyPI version](https://badge.fury.io/py/autocalver.svg)](https://badge.fury.io/py/autocalver)
+![GitHub Actions Status](https://github.com/moshez/autocalver/actions/workflows/pr-main.yml/badge.svg)
+[![Documentation Status](https://readthedocs.org/projects/autocalver/badge/?version=latest)](https://autocalver.readthedocs.io/en/latest/?badge=latest)
+
 Tired of
 "bumping versions"?
 Sick of commits,
 pull requests,
 tags,
 and a lot of manual work just to release
 the code that is already in the main branch?
@@ -41,15 +35,16 @@
 `pyproject.toml`:
 
 ```toml
 [build-system]
 requires = ["setuptools>=45", "wheel", "autocalver"]
 ```
 
-Note that
+Note that,
+by default,
 `autocalver`
 will
 *not*
 run any version-control commands.
 Before using
 `autocalver`,
 run a command to pull a prefix of the commit log,
@@ -63,18 +58,18 @@
 git log -n 1 --date=iso > git-log-head
 ```
 
 One advantage of separating the stages like that is that it is possible
 to have the package builder itself running in an environent that does not
 have access to the version control metadata,
 only the source files and the prefix of the commit log.
-Failing to produce the log will cause the package build to fail.
 
 The tool overrides the version in the
-`setup.cfg`.
+`setup.cfg`,
+if any.
 Configuration is done via
 `pyproject.toml`.
 For example,
 a configuration appropriate to
 pipeline CI might be:
 
 ```toml
@@ -157,7 +152,20 @@
 is there,
 missing any of the other variables
 will cause an
 *error*
 during the build,
 as a non-existing build
 is better than a broken when.
+
+## Automatically fetching the latest commit
+
+Defining the optional field
+`log_command`
+will run the command
+if the file is unavailable
+at package build time.
+It will create the file
+for next time.
+Note that if the file is
+"out of date",
+it needs to be manually removed.
```

### Comparing `autocalver-2023.4.27.46180/README.md` & `autocalver-2023.5.4.55367/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,23 @@
+Metadata-Version: 2.1
+Name: autocalver
+Version: 2023.5.4.55367
+Description-Content-Type: text/markdown
+Provides-Extra: tests
+Provides-Extra: lint
+Provides-Extra: mypy
+Provides-Extra: docs
+License-File: LICENSE
+
 # autocalver
 
+[![PyPI version](https://badge.fury.io/py/autocalver.svg)](https://badge.fury.io/py/autocalver)
+![GitHub Actions Status](https://github.com/moshez/autocalver/actions/workflows/pr-main.yml/badge.svg)
+[![Documentation Status](https://readthedocs.org/projects/autocalver/badge/?version=latest)](https://autocalver.readthedocs.io/en/latest/?badge=latest)
+
 Tired of
 "bumping versions"?
 Sick of commits,
 pull requests,
 tags,
 and a lot of manual work just to release
 the code that is already in the main branch?
@@ -31,15 +45,16 @@
 `pyproject.toml`:
 
 ```toml
 [build-system]
 requires = ["setuptools>=45", "wheel", "autocalver"]
 ```
 
-Note that
+Note that,
+by default,
 `autocalver`
 will
 *not*
 run any version-control commands.
 Before using
 `autocalver`,
 run a command to pull a prefix of the commit log,
@@ -53,18 +68,18 @@
 git log -n 1 --date=iso > git-log-head
 ```
 
 One advantage of separating the stages like that is that it is possible
 to have the package builder itself running in an environent that does not
 have access to the version control metadata,
 only the source files and the prefix of the commit log.
-Failing to produce the log will cause the package build to fail.
 
 The tool overrides the version in the
-`setup.cfg`.
+`setup.cfg`,
+if any.
 Configuration is done via
 `pyproject.toml`.
 For example,
 a configuration appropriate to
 pipeline CI might be:
 
 ```toml
@@ -147,7 +162,20 @@
 is there,
 missing any of the other variables
 will cause an
 *error*
 during the build,
 as a non-existing build
 is better than a broken when.
+
+## Automatically fetching the latest commit
+
+Defining the optional field
+`log_command`
+will run the command
+if the file is unavailable
+at package build time.
+It will create the file
+for next time.
+Note that if the file is
+"out of date",
+it needs to be manually removed.
```

### Comparing `autocalver-2023.4.27.46180/pyproject.toml` & `autocalver-2023.5.4.55367/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autocalver-2023.4.27.46180/src/autocalver/integration.py` & `autocalver-2023.5.4.55367/src/autocalver/integration.py`

 * *Files identical despite different names*

### Comparing `autocalver-2023.4.27.46180/src/autocalver.egg-info/PKG-INFO` & `autocalver-2023.5.4.55367/src/autocalver.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 Metadata-Version: 2.1
 Name: autocalver
-Version: 2023.4.27.46180
+Version: 2023.5.4.55367
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: lint
 Provides-Extra: mypy
 Provides-Extra: docs
 License-File: LICENSE
 
 # autocalver
 
+[![PyPI version](https://badge.fury.io/py/autocalver.svg)](https://badge.fury.io/py/autocalver)
+![GitHub Actions Status](https://github.com/moshez/autocalver/actions/workflows/pr-main.yml/badge.svg)
+[![Documentation Status](https://readthedocs.org/projects/autocalver/badge/?version=latest)](https://autocalver.readthedocs.io/en/latest/?badge=latest)
+
 Tired of
 "bumping versions"?
 Sick of commits,
 pull requests,
 tags,
 and a lot of manual work just to release
 the code that is already in the main branch?
@@ -41,15 +45,16 @@
 `pyproject.toml`:
 
 ```toml
 [build-system]
 requires = ["setuptools>=45", "wheel", "autocalver"]
 ```
 
-Note that
+Note that,
+by default,
 `autocalver`
 will
 *not*
 run any version-control commands.
 Before using
 `autocalver`,
 run a command to pull a prefix of the commit log,
@@ -63,18 +68,18 @@
 git log -n 1 --date=iso > git-log-head
 ```
 
 One advantage of separating the stages like that is that it is possible
 to have the package builder itself running in an environent that does not
 have access to the version control metadata,
 only the source files and the prefix of the commit log.
-Failing to produce the log will cause the package build to fail.
 
 The tool overrides the version in the
-`setup.cfg`.
+`setup.cfg`,
+if any.
 Configuration is done via
 `pyproject.toml`.
 For example,
 a configuration appropriate to
 pipeline CI might be:
 
 ```toml
@@ -157,7 +162,20 @@
 is there,
 missing any of the other variables
 will cause an
 *error*
 during the build,
 as a non-existing build
 is better than a broken when.
+
+## Automatically fetching the latest commit
+
+Defining the optional field
+`log_command`
+will run the command
+if the file is unavailable
+at package build time.
+It will create the file
+for next time.
+Note that if the file is
+"out of date",
+it needs to be manually removed.
```

### Comparing `autocalver-2023.4.27.46180/tests/test_integration.py` & `autocalver-2023.5.4.55367/tests/test_integration.py`

 * *Files identical despite different names*

