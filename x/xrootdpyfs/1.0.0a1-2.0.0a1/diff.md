# Comparing `tmp/xrootdpyfs-1.0.0a1.tar.gz` & `tmp/xrootdpyfs-2.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xrootdpyfs-1.0.0a1.tar", last modified: Wed Apr 19 14:37:49 2023, max compression
+gzip compressed data, was "xrootdpyfs-2.0.0a1.tar", last modified: Thu May  4 14:59:20 2023, max compression
```

## Comparing `xrootdpyfs-1.0.0a1.tar` & `xrootdpyfs-2.0.0a1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:37:49.918159 xrootdpyfs-1.0.0a1/
--rw-r--r--   0 runner    (1001) docker     (122)      120 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (122)      525 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:37:49.914159 xrootdpyfs-1.0.0a1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:37:49.914159 xrootdpyfs-1.0.0a1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      891 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (122)      194 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (122)     1487 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/CHANGES
--rw-r--r--   0 runner    (1001) docker     (122)     1164 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1802 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      755 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     4313 2023-04-19 14:37:49.918159 xrootdpyfs-1.0.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3718 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:37:49.914159 xrootdpyfs-1.0.0a1/docs/
--rw-r--r--   0 runner    (1001) docker     (122)     7425 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)    10094 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      613 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/run-docker.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      402 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-04-19 14:37:49.918159 xrootdpyfs-1.0.0a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:37:49.914159 xrootdpyfs-1.0.0a1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      640 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:37:49.914159 xrootdpyfs-1.0.0a1/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:37:49.914159 xrootdpyfs-1.0.0a1/tests/data/afolder/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/tests/data/afolder/afile.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:37:49.914159 xrootdpyfs-1.0.0a1/tests/data/bfolder/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/tests/data/bfolder/bfile.txt
--rwxr-xr-x   0 runner    (1001) docker     (122)       10 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/tests/data/binary.dat
--rw-r--r--   0 runner    (1001) docker     (122)      145 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/tests/data/multiline.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/tests/data/testa.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2778 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/tests/perf.py
--rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/tests/test_env.py
--rw-r--r--   0 runner    (1001) docker     (122)    25647 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/tests/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (122)      828 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/tests/test_fs_extras.py
--rw-r--r--   0 runner    (1001) docker     (122)      638 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/tests/test_opener.py
--rw-r--r--   0 runner    (1001) docker     (122)     2100 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    37201 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/tests/test_xrdfile.py
--rw-r--r--   0 runner    (1001) docker     (122)     3366 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/tests/test_xrdflags.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:37:49.914159 xrootdpyfs-1.0.0a1/xrootdpyfs/
--rw-r--r--   0 runner    (1001) docker     (122)     5188 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/xrootdpyfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2198 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/xrootdpyfs/env.py
--rw-r--r--   0 runner    (1001) docker     (122)    28590 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/xrootdpyfs/fs.py
--rw-r--r--   0 runner    (1001) docker     (122)     1534 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/xrootdpyfs/opener.py
--rw-r--r--   0 runner    (1001) docker     (122)     1631 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/xrootdpyfs/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    14539 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/xrootdpyfs/xrdfile.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:37:49.914159 xrootdpyfs-1.0.0a1/xrootdpyfs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4313 2023-04-19 14:37:49.000000 xrootdpyfs-1.0.0a1/xrootdpyfs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      950 2023-04-19 14:37:49.000000 xrootdpyfs-1.0.0a1/xrootdpyfs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-19 14:37:49.000000 xrootdpyfs-1.0.0a1/xrootdpyfs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       94 2023-04-19 14:37:49.000000 xrootdpyfs-1.0.0a1/xrootdpyfs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-19 14:37:49.000000 xrootdpyfs-1.0.0a1/xrootdpyfs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      114 2023-04-19 14:37:49.000000 xrootdpyfs-1.0.0a1/xrootdpyfs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-04-19 14:37:49.000000 xrootdpyfs-1.0.0a1/xrootdpyfs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 14:59:20.576154 xrootdpyfs-2.0.0a1/
+-rw-r--r--   0 runner    (1001) docker     (122)       77 2023-05-04 14:59:14.000000 xrootdpyfs-2.0.0a1/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (122)      525 2023-05-04 14:59:14.000000 xrootdpyfs-2.0.0a1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-05-04 14:59:14.000000 xrootdpyfs-2.0.0a1/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 14:59:20.568154 xrootdpyfs-2.0.0a1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 14:59:20.572154 xrootdpyfs-2.0.0a1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      891 2023-05-04 14:59:14.000000 xrootdpyfs-2.0.0a1/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      842 2023-05-04 14:59:14.000000 xrootdpyfs-2.0.0a1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      194 2023-05-04 14:59:14.000000 xrootdpyfs-2.0.0a1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (122)     1589 2023-05-04 14:59:14.000000 xrootdpyfs-2.0.0a1/CHANGES
+-rw-r--r--   0 runner    (1001) docker     (122)     1164 2023-05-04 14:59:14.000000 xrootdpyfs-2.0.0a1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1802 2023-05-04 14:59:14.000000 xrootdpyfs-2.0.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      755 2023-05-04 14:59:14.000000 xrootdpyfs-2.0.0a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4313 2023-05-04 14:59:20.576154 xrootdpyfs-2.0.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3718 2023-05-04 14:59:14.000000 xrootdpyfs-2.0.0a1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 14:59:20.572154 xrootdpyfs-2.0.0a1/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     7425 2023-05-04 14:59:14.000000 xrootdpyfs-2.0.0a1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)    10094 2023-05-04 14:59:14.000000 xrootdpyfs-2.0.0a1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      613 2023-05-04 14:59:14.000000 xrootdpyfs-2.0.0a1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-05-04 14:59:14.000000 xrootdpyfs-2.0.0a1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-05-04 14:59:14.000000 xrootdpyfs-2.0.0a1/run-docker.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      427 2023-05-04 14:59:14.000000 xrootdpyfs-2.0.0a1/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-05-04 14:59:20.576154 xrootdpyfs-2.0.0a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-05-04 14:59:14.000000 xrootdpyfs-2.0.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 14:59:20.572154 xrootdpyfs-2.0.0a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      640 2023-05-04 14:59:14.000000 xrootdpyfs-2.0.0a1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 14:59:20.576154 xrootdpyfs-2.0.0a1/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 14:59:20.576154 xrootdpyfs-2.0.0a1/tests/data/afolder/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-04 14:59:14.000000 xrootdpyfs-2.0.0a1/tests/data/afolder/afile.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 14:59:20.576154 xrootdpyfs-2.0.0a1/tests/data/bfolder/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-04 14:59:14.000000 xrootdpyfs-2.0.0a1/tests/data/bfolder/bfile.txt
+-rwxr-xr-x   0 runner    (1001) docker     (122)       10 2023-05-04 14:59:14.000000 xrootdpyfs-2.0.0a1/tests/data/binary.dat
+-rw-r--r--   0 runner    (1001) docker     (122)      145 2023-05-04 14:59:14.000000 xrootdpyfs-2.0.0a1/tests/data/multiline.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-04 14:59:14.000000 xrootdpyfs-2.0.0a1/tests/data/testa.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2778 2023-05-04 14:59:14.000000 xrootdpyfs-2.0.0a1/tests/perf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-05-04 14:59:14.000000 xrootdpyfs-2.0.0a1/tests/test_env.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25647 2023-05-04 14:59:14.000000 xrootdpyfs-2.0.0a1/tests/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (122)      828 2023-05-04 14:59:14.000000 xrootdpyfs-2.0.0a1/tests/test_fs_extras.py
+-rw-r--r--   0 runner    (1001) docker     (122)      638 2023-05-04 14:59:14.000000 xrootdpyfs-2.0.0a1/tests/test_opener.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2100 2023-05-04 14:59:14.000000 xrootdpyfs-2.0.0a1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    37269 2023-05-04 14:59:14.000000 xrootdpyfs-2.0.0a1/tests/test_xrdfile.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3452 2023-05-04 14:59:14.000000 xrootdpyfs-2.0.0a1/tests/test_xrdflags.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 14:59:20.576154 xrootdpyfs-2.0.0a1/xrootdpyfs/
+-rw-r--r--   0 runner    (1001) docker     (122)     5188 2023-05-04 14:59:14.000000 xrootdpyfs-2.0.0a1/xrootdpyfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2198 2023-05-04 14:59:14.000000 xrootdpyfs-2.0.0a1/xrootdpyfs/env.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29220 2023-05-04 14:59:15.000000 xrootdpyfs-2.0.0a1/xrootdpyfs/fs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1534 2023-05-04 14:59:15.000000 xrootdpyfs-2.0.0a1/xrootdpyfs/opener.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1631 2023-05-04 14:59:15.000000 xrootdpyfs-2.0.0a1/xrootdpyfs/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14539 2023-05-04 14:59:15.000000 xrootdpyfs-2.0.0a1/xrootdpyfs/xrdfile.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 14:59:20.576154 xrootdpyfs-2.0.0a1/xrootdpyfs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4313 2023-05-04 14:59:20.000000 xrootdpyfs-2.0.0a1/xrootdpyfs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      950 2023-05-04 14:59:20.000000 xrootdpyfs-2.0.0a1/xrootdpyfs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-04 14:59:20.000000 xrootdpyfs-2.0.0a1/xrootdpyfs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       94 2023-05-04 14:59:20.000000 xrootdpyfs-2.0.0a1/xrootdpyfs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-04 14:59:20.000000 xrootdpyfs-2.0.0a1/xrootdpyfs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      114 2023-05-04 14:59:20.000000 xrootdpyfs-2.0.0a1/xrootdpyfs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-05-04 14:59:20.000000 xrootdpyfs-2.0.0a1/xrootdpyfs.egg-info/top_level.txt
```

### Comparing `xrootdpyfs-1.0.0a1/.editorconfig` & `xrootdpyfs-2.0.0a1/.editorconfig`

 * *Files identical despite different names*

### Comparing `xrootdpyfs-1.0.0a1/.github/workflows/pypi-publish.yml` & `xrootdpyfs-2.0.0a1/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `xrootdpyfs-1.0.0a1/CHANGES` & `xrootdpyfs-2.0.0a1/CHANGES`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Changes
 =======
 
+Version 2.0.0a1 (released 2023-05-03)
+
+- upgrade xrootd to version 5.
+- fix testing xrootd responses
+
 Version 1.0.0a1 (released 2023-04-19)
 
 - Upgrade pyfs to version 2.
 - Improve module's files organization and code formatting.
 
 Version 0.2.2 (released 2021-12-13)
```

### Comparing `xrootdpyfs-1.0.0a1/CONTRIBUTING.rst` & `xrootdpyfs-2.0.0a1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `xrootdpyfs-1.0.0a1/LICENSE` & `xrootdpyfs-2.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `xrootdpyfs-1.0.0a1/MANIFEST.in` & `xrootdpyfs-2.0.0a1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `xrootdpyfs-1.0.0a1/PKG-INFO` & `xrootdpyfs-2.0.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xrootdpyfs
-Version: 1.0.0a1
+Version: 2.0.0a1
 Summary: XRootDPyFS is a PyFilesystem interface for XRootD.
 Home-page: https://github.com/inveniosoftware/xrootdpyfs
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: BSD
 Keywords: xrootdpyfs
 Platform: any
```

### Comparing `xrootdpyfs-1.0.0a1/README.rst` & `xrootdpyfs-2.0.0a1/README.rst`

 * *Files identical despite different names*

### Comparing `xrootdpyfs-1.0.0a1/docs/Makefile` & `xrootdpyfs-2.0.0a1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `xrootdpyfs-1.0.0a1/docs/conf.py` & `xrootdpyfs-2.0.0a1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `xrootdpyfs-1.0.0a1/docs/index.rst` & `xrootdpyfs-2.0.0a1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `xrootdpyfs-1.0.0a1/setup.cfg` & `xrootdpyfs-2.0.0a1/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -19,22 +19,22 @@
 [options]
 include_package_data = True
 packages = find:
 python_requires = >=3.6
 zip_safe = False
 install_requires = 
 	fs>=2.0.10,<3.0
-	xrootd>=4.8.4,<5.0.0
+	xrootd>=5.0.0,<6.0.0
 
 [options.extras_require]
 tests = 
 	mock>=4.0.0
 	pytest-black>=0.3.0
 	pytest-invenio>=1.4.5
-	Sphinx==4.2.0
+	Sphinx>=4.2.0
 
 [options.entry_points]
 fs.opener = 
 	root = xrootdpyfs.opener:XRootDPyOpener
 	roots = xrootdpyfs.opener:XRootDPyOpener
 
 [aliases]
```

### Comparing `xrootdpyfs-1.0.0a1/tests/conftest.py` & `xrootdpyfs-2.0.0a1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `xrootdpyfs-1.0.0a1/tests/perf.py` & `xrootdpyfs-2.0.0a1/tests/perf.py`

 * *Files identical despite different names*

### Comparing `xrootdpyfs-1.0.0a1/tests/test_env.py` & `xrootdpyfs-2.0.0a1/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `xrootdpyfs-1.0.0a1/tests/test_fs.py` & `xrootdpyfs-2.0.0a1/tests/test_fs.py`

 * *Files identical despite different names*

### Comparing `xrootdpyfs-1.0.0a1/tests/test_fs_extras.py` & `xrootdpyfs-2.0.0a1/tests/test_fs_extras.py`

 * *Files identical despite different names*

### Comparing `xrootdpyfs-1.0.0a1/tests/test_opener.py` & `xrootdpyfs-2.0.0a1/tests/test_opener.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,12 +11,12 @@
 from conftest import mkurl
 from fs.opener import open_fs
 
 
 def test_open_fs_create(tmppath):
     """Test open with create."""
     rooturl = mkurl(tmppath)
-    fs = open_fs(rooturl + "/non-existing")
+    fs = open_fs(f"{rooturl}/non-existing")
     assert fs.listdir("./")
     assert not fs.exists("/non-existing")
     fs = open_fs(rooturl + "/non-existing", create=True)
     assert fs.exists("/non-existing")
```

### Comparing `xrootdpyfs-1.0.0a1/tests/test_utils.py` & `xrootdpyfs-2.0.0a1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `xrootdpyfs-1.0.0a1/tests/test_xrdfile.py` & `xrootdpyfs-2.0.0a1/tests/test_xrdfile.py`

 * *Files 0% similar despite different names*

```diff
@@ -625,15 +625,17 @@
     fb = get_copy_file(fd)
     fp, dummy = fd["full_path"], fd["contents"]
     fp2 = fb["full_path"]
 
     unicodestr = "æøå"
 
     pfile = open(fp2, "w")  # default encoding is ANSI
-    pytest.raises(UnicodeEncodeError, pfile.write, unicodestr)
+    # unicode is handled by default in python 3
+    # pytest.raises(UnicodeEncodeError, pfile.write, unicodestr)
+    pfile.close()
     xfile = XRootDPyFile(mkurl(fp), "w", encoding="ascii")
     pytest.raises(UnicodeEncodeError, xfile.write, unicodestr)
     xfile.close()
 
 
 def test_readwrite_unicode(tmppath):
     """Test read/write a unicode str in unicode files."""
```

### Comparing `xrootdpyfs-1.0.0a1/tests/test_xrdflags.py` & `xrootdpyfs-2.0.0a1/tests/test_xrdflags.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 # xrootdpyfs is free software; you can redistribute it and/or modify it under
 # the terms of the Revised BSD License; see LICENSE file for more details.
 
 """Test of XRootD File Flags."""
 
 from os.path import join
 
+import pytest
 from conftest import mkurl
 from XRootD import client as xclient
 from XRootD.client.flags import OpenFlags
 
 
 # If "test" is in its name then pytest picks it up.
 def tstfile_a(p):
@@ -46,14 +47,15 @@
     # Can we truncate?
     statmsg, res = xf.truncate(0)
     print((statmsg,))
     assert not statmsg.ok
     assert statmsg.error
 
 
+@pytest.mark.skip("OpenFlags.APPEND not used anywhere in the codebase")
 def test_APPEND(tmppath):
     fname, fconts = tstfile_a(tmppath)
     ffpath = join(tmppath, fname)
     xf = xclient.File()
     xf.open(mkurl(ffpath), OpenFlags.APPEND)
     assert xf
```

### Comparing `xrootdpyfs-1.0.0a1/xrootdpyfs/__init__.py` & `xrootdpyfs-2.0.0a1/xrootdpyfs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,10 +182,10 @@
     b'World'
 """
 
 from .fs import XRootDPyFS
 from .opener import XRootDPyOpener
 from .xrdfile import XRootDPyFile
 
-__version__ = "1.0.0a1"
+__version__ = "2.0.0a1"
 
 __all__ = ("__version__", "XRootDPyFS", "XRootDPyOpener", "XRootDPyFile")
```

### Comparing `xrootdpyfs-1.0.0a1/xrootdpyfs/env.py` & `xrootdpyfs-2.0.0a1/xrootdpyfs/env.py`

 * *Files identical despite different names*

### Comparing `xrootdpyfs-1.0.0a1/xrootdpyfs/fs.py` & `xrootdpyfs-2.0.0a1/xrootdpyfs/fs.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
 
         self.root_url = root_url
         self.base_path = base_path
         self.queryargs = queryargs
         self._client = FileSystem(self.xrd_get_rooturl())
         super().__init__()
 
-    def _p(self, path):
+    def _p(self, path, encoding="utf-8"):
         """Prepend base path to path."""
         # fs.path.join() omits the first '/' in self.base_path.
         # It is resolved by adding on an additional '/' to its return value.
         _path = path
         if isabs(path):
             no_trailing = self.base_path[:-1]
             one_slash = no_trailing[1:]
@@ -143,15 +143,16 @@
             )
             if missing_basepath:
                 _path = relpath(path)
         return "/" + join(self.base_path, _path)
 
     def _raise_status(self, path, status):
         """Raise error based on status."""
-        if status.errno in [3006, 17]:
+        # 3006 - legacy (v4 errno), 17 - POSIX error, 3018 (xrootd v5 errno)
+        if status.errno in [3006, 17, 3018]:
             raise DestinationExists(path=path, msg=status)
         elif status.errno == 3005:
             # Unfortunately only way to determine if the error is due to a
             # directory not being empty, or that a resource is not a directory:
             if status.message.strip().endswith("not a directory"):
                 raise ResourceInvalid(path=path, msg=status)
             else:
@@ -165,14 +166,22 @@
         """Query an xrootd server."""
         status, res = self._client.query(flag, arg)
 
         if not status.ok:
             if status.errno == 3013:
                 raise Unsupported(msg=status)
             raise FSError(msg=status)
+
+        # due to https://github.com/xrootd/xrootd/blob
+        # /39f9e0ae6744c4e068905daf0a10270f443b8619/src/XrdOfs/XrdOfsFSctl.cc#L230
+        # the response contains random bytes due to the way buffer size is allocated
+        # which causes response parsing errors on our python client.
+        # The bytes succeeding the null byte (x00) should be ignored.
+        if b"\x00" in res[-3:-1]:
+            res = res.split(b"\x00")[0]
         return parse_qs(res) if parse else res
 
     def open(
         self,
         path,
         mode="r",
         buffering=-1,
@@ -339,15 +348,16 @@
         """
         flags = MkDirFlags.MAKEPATH if recursive else MkDirFlags.NONE
         mode = AccessMode.NONE
 
         status, _ = self._client.mkdir(self._p(path), flags=flags, mode=mode)
 
         if not status.ok:
-            destination_exists = status.errno == 3006
+            # 3018 introduced in xrootd5, 17 = POSIX error, 3006 - legacy errno
+            destination_exists = status.errno in [3006, 3018, 17]
             if allow_recreate and destination_exists:
                 return True
             self._raise_status(path, status)
         return True
 
     def openbin(self, path, mode="r", buffering=-1, **options):
         """Openbin."""
```

### Comparing `xrootdpyfs-1.0.0a1/xrootdpyfs/opener.py` & `xrootdpyfs-2.0.0a1/xrootdpyfs/opener.py`

 * *Files identical despite different names*

### Comparing `xrootdpyfs-1.0.0a1/xrootdpyfs/utils.py` & `xrootdpyfs-2.0.0a1/xrootdpyfs/utils.py`

 * *Files identical despite different names*

### Comparing `xrootdpyfs-1.0.0a1/xrootdpyfs/xrdfile.py` & `xrootdpyfs-2.0.0a1/xrootdpyfs/xrdfile.py`

 * *Files identical despite different names*

### Comparing `xrootdpyfs-1.0.0a1/xrootdpyfs.egg-info/PKG-INFO` & `xrootdpyfs-2.0.0a1/xrootdpyfs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xrootdpyfs
-Version: 1.0.0a1
+Version: 2.0.0a1
 Summary: XRootDPyFS is a PyFilesystem interface for XRootD.
 Home-page: https://github.com/inveniosoftware/xrootdpyfs
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: BSD
 Keywords: xrootdpyfs
 Platform: any
```

### Comparing `xrootdpyfs-1.0.0a1/xrootdpyfs.egg-info/SOURCES.txt` & `xrootdpyfs-2.0.0a1/xrootdpyfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

