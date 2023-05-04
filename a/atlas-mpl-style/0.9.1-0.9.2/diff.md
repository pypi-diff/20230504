# Comparing `tmp/atlas-mpl-style-0.9.1.tar.gz` & `tmp/atlas-mpl-style-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/atlas-mpl-style-0.9.1.tar", last modified: Tue Dec 17 09:31:07 2019, max compression
+gzip compressed data, was "dist/atlas-mpl-style-0.9.2.tar", last modified: Sat Feb  1 09:53:20 2020, max compression
```

## Comparing `atlas-mpl-style-0.9.1.tar` & `atlas-mpl-style-0.9.2.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 beojan    (1000) beojan    (1000)        0 2019-12-17 09:31:07.860626 atlas-mpl-style-0.9.1/
--rw-r--r--   0 beojan    (1000) beojan    (1000)      370 2019-05-02 14:07:09.000000 atlas-mpl-style-0.9.1/.readthedocs.yml
--rw-r--r--   0 beojan    (1000) beojan    (1000)    34893 2017-12-07 15:21:10.000000 atlas-mpl-style-0.9.1/LICENSE.md
--rw-r--r--   0 beojan    (1000) beojan    (1000)       66 2018-01-31 11:06:03.000000 atlas-mpl-style-0.9.1/MANIFEST.in
--rw-r--r--   0 beojan    (1000) beojan    (1000)     2042 2019-12-17 09:31:07.860626 atlas-mpl-style-0.9.1/PKG-INFO
--rw-r--r--   0 beojan    (1000) beojan    (1000)     1056 2019-12-17 09:30:40.000000 atlas-mpl-style-0.9.1/README.rst
-drwxr-xr-x   0 beojan    (1000) beojan    (1000)        0 2019-12-17 09:31:07.854626 atlas-mpl-style-0.9.1/atlas_mpl_style/
--rw-r--r--   0 beojan    (1000) beojan    (1000)     8128 2019-12-17 09:17:50.000000 atlas-mpl-style-0.9.1/atlas_mpl_style/__init__.py
-drwxr-xr-x   0 beojan    (1000) beojan    (1000)        0 2019-12-17 09:31:07.855626 atlas-mpl-style-0.9.1/atlas_mpl_style/stylesheets/
--rw-r--r--   0 beojan    (1000) beojan    (1000)     1174 2019-12-17 09:19:48.000000 atlas-mpl-style-0.9.1/atlas_mpl_style/stylesheets/atlas.mplstyle
--rw-r--r--   0 beojan    (1000) beojan    (1000)     1247 2019-11-06 13:47:12.000000 atlas-mpl-style-0.9.1/atlas_mpl_style/stylesheets/paper.mplstyle
--rw-r--r--   0 beojan    (1000) beojan    (1000)     1229 2019-11-06 13:58:49.000000 atlas-mpl-style-0.9.1/atlas_mpl_style/stylesheets/print.mplstyle
-drwxr-xr-x   0 beojan    (1000) beojan    (1000)        0 2019-12-17 09:31:07.855626 atlas-mpl-style-0.9.1/atlas_mpl_style.egg-info/
--rw-r--r--   0 beojan    (1000) beojan    (1000)     2042 2019-12-17 09:31:06.000000 atlas-mpl-style-0.9.1/atlas_mpl_style.egg-info/PKG-INFO
--rw-r--r--   0 beojan    (1000) beojan    (1000)     1683 2019-12-17 09:31:06.000000 atlas-mpl-style-0.9.1/atlas_mpl_style.egg-info/SOURCES.txt
--rw-r--r--   0 beojan    (1000) beojan    (1000)        1 2019-12-17 09:31:06.000000 atlas-mpl-style-0.9.1/atlas_mpl_style.egg-info/dependency_links.txt
--rw-r--r--   0 beojan    (1000) beojan    (1000)       14 2019-12-17 09:31:06.000000 atlas-mpl-style-0.9.1/atlas_mpl_style.egg-info/requires.txt
--rw-r--r--   0 beojan    (1000) beojan    (1000)       16 2019-12-17 09:31:06.000000 atlas-mpl-style-0.9.1/atlas_mpl_style.egg-info/top_level.txt
-drwxr-xr-x   0 beojan    (1000) beojan    (1000)        0 2019-12-17 09:31:07.856626 atlas-mpl-style-0.9.1/docs/
--rw-r--r--   0 beojan    (1000) beojan    (1000)      580 2019-05-02 12:37:59.000000 atlas-mpl-style-0.9.1/docs/Makefile
-drwxr-xr-x   0 beojan    (1000) beojan    (1000)        0 2019-12-17 09:31:07.859626 atlas-mpl-style-0.9.1/docs/_colors/
--rw-r--r--   0 beojan    (1000) beojan    (1000)      435 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.1/docs/_colors/atlas:onesigma.png
--rw-r--r--   0 beojan    (1000) beojan    (1000)      437 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.1/docs/_colors/atlas:twosigma.png
--rw-r--r--   0 beojan    (1000) beojan    (1000)      439 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.1/docs/_colors/on:bg.png
--rw-r--r--   0 beojan    (1000) beojan    (1000)      439 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.1/docs/_colors/on:bgAlt.png
--rw-r--r--   0 beojan    (1000) beojan    (1000)      438 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.1/docs/_colors/on:blue.png
--rw-r--r--   0 beojan    (1000) beojan    (1000)      438 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.1/docs/_colors/on:brown.png
--rw-r--r--   0 beojan    (1000) beojan    (1000)      436 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.1/docs/_colors/on:cyan.png
--rw-r--r--   0 beojan    (1000) beojan    (1000)      439 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.1/docs/_colors/on:fg.png
--rw-r--r--   0 beojan    (1000) beojan    (1000)      439 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.1/docs/_colors/on:fgAlt.png
--rw-r--r--   0 beojan    (1000) beojan    (1000)      439 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.1/docs/_colors/on:green.png
--rw-r--r--   0 beojan    (1000) beojan    (1000)      438 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.1/docs/_colors/on:orange.png
--rw-r--r--   0 beojan    (1000) beojan    (1000)      437 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.1/docs/_colors/on:pink.png
--rw-r--r--   0 beojan    (1000) beojan    (1000)      438 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.1/docs/_colors/on:red.png
--rw-r--r--   0 beojan    (1000) beojan    (1000)      438 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.1/docs/_colors/on:yellow.png
--rw-r--r--   0 beojan    (1000) beojan    (1000)      436 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.1/docs/_colors/paper:bg.png
--rw-r--r--   0 beojan    (1000) beojan    (1000)      436 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.1/docs/_colors/paper:bgAlt.png
--rw-r--r--   0 beojan    (1000) beojan    (1000)      436 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.1/docs/_colors/paper:blue.png
--rw-r--r--   0 beojan    (1000) beojan    (1000)      436 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.1/docs/_colors/paper:fg.png
--rw-r--r--   0 beojan    (1000) beojan    (1000)      435 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.1/docs/_colors/paper:green.png
--rw-r--r--   0 beojan    (1000) beojan    (1000)      436 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.1/docs/_colors/paper:lightBlue.png
--rw-r--r--   0 beojan    (1000) beojan    (1000)      436 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.1/docs/_colors/paper:olive.png
--rw-r--r--   0 beojan    (1000) beojan    (1000)      436 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.1/docs/_colors/paper:orange.png
--rw-r--r--   0 beojan    (1000) beojan    (1000)      436 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.1/docs/_colors/paper:pink.png
--rw-r--r--   0 beojan    (1000) beojan    (1000)      436 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.1/docs/_colors/paper:purple.png
--rw-r--r--   0 beojan    (1000) beojan    (1000)      436 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.1/docs/_colors/paper:red.png
--rw-r--r--   0 beojan    (1000) beojan    (1000)      435 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.1/docs/_colors/paper:yellow.png
--rw-r--r--   0 beojan    (1000) beojan    (1000)      437 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.1/docs/_colors/series2:blue.png
--rw-r--r--   0 beojan    (1000) beojan    (1000)      435 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.1/docs/_colors/series2:green.png
--rw-r--r--   0 beojan    (1000) beojan    (1000)      436 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.1/docs/_colors/series2:purple.png
--rw-r--r--   0 beojan    (1000) beojan    (1000)      437 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.1/docs/_colors/series2:red.png
--rw-r--r--   0 beojan    (1000) beojan    (1000)      437 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.1/docs/_colors/series2:yellow.png
--rw-r--r--   0 beojan    (1000) beojan    (1000)      439 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.1/docs/_colors/series:blue.png
--rw-r--r--   0 beojan    (1000) beojan    (1000)      438 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.1/docs/_colors/series:cyan.png
--rw-r--r--   0 beojan    (1000) beojan    (1000)      438 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.1/docs/_colors/series:green.png
--rw-r--r--   0 beojan    (1000) beojan    (1000)      438 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.1/docs/_colors/series:olive.png
--rw-r--r--   0 beojan    (1000) beojan    (1000)      439 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.1/docs/_colors/series:orange.png
--rw-r--r--   0 beojan    (1000) beojan    (1000)      439 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.1/docs/_colors/series:pink.png
--rw-r--r--   0 beojan    (1000) beojan    (1000)      439 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.1/docs/_colors/series:purple.png
--rw-r--r--   0 beojan    (1000) beojan    (1000)      438 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.1/docs/_colors/series:turquoise.png
--rw-r--r--   0 beojan    (1000) beojan    (1000)      433 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.1/docs/_colors/transparent.png
--rw-r--r--   0 beojan    (1000) beojan    (1000)      100 2019-05-02 12:46:57.000000 atlas-mpl-style-0.9.1/docs/atlas-mpl-style.rst
--rw-r--r--   0 beojan    (1000) beojan    (1000)     9130 2019-05-02 13:16:57.000000 atlas-mpl-style-0.9.1/docs/colors.rst
--rw-r--r--   0 beojan    (1000) beojan    (1000)     1928 2019-05-02 14:16:15.000000 atlas-mpl-style-0.9.1/docs/conf.py
--rw-r--r--   0 beojan    (1000) beojan    (1000)      527 2019-05-02 14:16:04.000000 atlas-mpl-style-0.9.1/docs/index.rst
--rw-r--r--   0 beojan    (1000) beojan    (1000)      787 2019-05-02 12:37:59.000000 atlas-mpl-style-0.9.1/docs/make.bat
--rw-r--r--   0 beojan    (1000) beojan    (1000)       20 2019-05-02 14:02:21.000000 atlas-mpl-style-0.9.1/docs/requirements.txt
--rw-r--r--   0 beojan    (1000) beojan    (1000)     1063 2019-05-02 13:52:56.000000 atlas-mpl-style-0.9.1/docs/styles.rst
--rw-r--r--   0 beojan    (1000) beojan    (1000)       38 2019-12-17 09:31:07.860626 atlas-mpl-style-0.9.1/setup.cfg
--rw-r--r--   0 beojan    (1000) beojan    (1000)     2779 2019-12-17 09:29:38.000000 atlas-mpl-style-0.9.1/setup.py
+drwxr-xr-x   0 beojan    (1000) beojan    (1000)        0 2020-02-01 09:53:20.860234 atlas-mpl-style-0.9.2/
+-rw-r--r--   0 beojan    (1000) beojan    (1000)      370 2019-05-02 14:07:09.000000 atlas-mpl-style-0.9.2/.readthedocs.yml
+-rw-r--r--   0 beojan    (1000) beojan    (1000)    34893 2017-12-07 15:21:10.000000 atlas-mpl-style-0.9.2/LICENSE.md
+-rw-r--r--   0 beojan    (1000) beojan    (1000)       66 2018-01-31 11:06:03.000000 atlas-mpl-style-0.9.2/MANIFEST.in
+-rw-r--r--   0 beojan    (1000) beojan    (1000)     2042 2020-02-01 09:53:20.860234 atlas-mpl-style-0.9.2/PKG-INFO
+-rw-r--r--   0 beojan    (1000) beojan    (1000)     1056 2019-12-17 09:30:40.000000 atlas-mpl-style-0.9.2/README.rst
+drwxr-xr-x   0 beojan    (1000) beojan    (1000)        0 2020-02-01 09:53:20.850234 atlas-mpl-style-0.9.2/atlas_mpl_style/
+-rw-r--r--   0 beojan    (1000) beojan    (1000)     8139 2020-02-01 09:51:32.000000 atlas-mpl-style-0.9.2/atlas_mpl_style/__init__.py
+drwxr-xr-x   0 beojan    (1000) beojan    (1000)        0 2020-02-01 09:53:20.850234 atlas-mpl-style-0.9.2/atlas_mpl_style/stylesheets/
+-rw-r--r--   0 beojan    (1000) beojan    (1000)     1174 2019-12-17 09:19:48.000000 atlas-mpl-style-0.9.2/atlas_mpl_style/stylesheets/atlas.mplstyle
+-rw-r--r--   0 beojan    (1000) beojan    (1000)     1247 2019-11-06 13:47:12.000000 atlas-mpl-style-0.9.2/atlas_mpl_style/stylesheets/paper.mplstyle
+-rw-r--r--   0 beojan    (1000) beojan    (1000)     1229 2019-11-06 13:58:49.000000 atlas-mpl-style-0.9.2/atlas_mpl_style/stylesheets/print.mplstyle
+drwxr-xr-x   0 beojan    (1000) beojan    (1000)        0 2020-02-01 09:53:20.850234 atlas-mpl-style-0.9.2/atlas_mpl_style.egg-info/
+-rw-r--r--   0 beojan    (1000) beojan    (1000)     2042 2020-02-01 09:53:20.000000 atlas-mpl-style-0.9.2/atlas_mpl_style.egg-info/PKG-INFO
+-rw-r--r--   0 beojan    (1000) beojan    (1000)     1683 2020-02-01 09:53:20.000000 atlas-mpl-style-0.9.2/atlas_mpl_style.egg-info/SOURCES.txt
+-rw-r--r--   0 beojan    (1000) beojan    (1000)        1 2020-02-01 09:53:20.000000 atlas-mpl-style-0.9.2/atlas_mpl_style.egg-info/dependency_links.txt
+-rw-r--r--   0 beojan    (1000) beojan    (1000)       14 2020-02-01 09:53:20.000000 atlas-mpl-style-0.9.2/atlas_mpl_style.egg-info/requires.txt
+-rw-r--r--   0 beojan    (1000) beojan    (1000)       16 2020-02-01 09:53:20.000000 atlas-mpl-style-0.9.2/atlas_mpl_style.egg-info/top_level.txt
+drwxr-xr-x   0 beojan    (1000) beojan    (1000)        0 2020-02-01 09:53:20.850234 atlas-mpl-style-0.9.2/docs/
+-rw-r--r--   0 beojan    (1000) beojan    (1000)      580 2019-05-02 12:37:59.000000 atlas-mpl-style-0.9.2/docs/Makefile
+drwxr-xr-x   0 beojan    (1000) beojan    (1000)        0 2020-02-01 09:53:20.860234 atlas-mpl-style-0.9.2/docs/_colors/
+-rw-r--r--   0 beojan    (1000) beojan    (1000)      435 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.2/docs/_colors/atlas:onesigma.png
+-rw-r--r--   0 beojan    (1000) beojan    (1000)      437 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.2/docs/_colors/atlas:twosigma.png
+-rw-r--r--   0 beojan    (1000) beojan    (1000)      439 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.2/docs/_colors/on:bg.png
+-rw-r--r--   0 beojan    (1000) beojan    (1000)      439 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.2/docs/_colors/on:bgAlt.png
+-rw-r--r--   0 beojan    (1000) beojan    (1000)      438 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.2/docs/_colors/on:blue.png
+-rw-r--r--   0 beojan    (1000) beojan    (1000)      438 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.2/docs/_colors/on:brown.png
+-rw-r--r--   0 beojan    (1000) beojan    (1000)      436 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.2/docs/_colors/on:cyan.png
+-rw-r--r--   0 beojan    (1000) beojan    (1000)      439 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.2/docs/_colors/on:fg.png
+-rw-r--r--   0 beojan    (1000) beojan    (1000)      439 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.2/docs/_colors/on:fgAlt.png
+-rw-r--r--   0 beojan    (1000) beojan    (1000)      439 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.2/docs/_colors/on:green.png
+-rw-r--r--   0 beojan    (1000) beojan    (1000)      438 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.2/docs/_colors/on:orange.png
+-rw-r--r--   0 beojan    (1000) beojan    (1000)      437 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.2/docs/_colors/on:pink.png
+-rw-r--r--   0 beojan    (1000) beojan    (1000)      438 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.2/docs/_colors/on:red.png
+-rw-r--r--   0 beojan    (1000) beojan    (1000)      438 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.2/docs/_colors/on:yellow.png
+-rw-r--r--   0 beojan    (1000) beojan    (1000)      436 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.2/docs/_colors/paper:bg.png
+-rw-r--r--   0 beojan    (1000) beojan    (1000)      436 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.2/docs/_colors/paper:bgAlt.png
+-rw-r--r--   0 beojan    (1000) beojan    (1000)      436 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.2/docs/_colors/paper:blue.png
+-rw-r--r--   0 beojan    (1000) beojan    (1000)      436 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.2/docs/_colors/paper:fg.png
+-rw-r--r--   0 beojan    (1000) beojan    (1000)      435 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.2/docs/_colors/paper:green.png
+-rw-r--r--   0 beojan    (1000) beojan    (1000)      436 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.2/docs/_colors/paper:lightBlue.png
+-rw-r--r--   0 beojan    (1000) beojan    (1000)      436 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.2/docs/_colors/paper:olive.png
+-rw-r--r--   0 beojan    (1000) beojan    (1000)      436 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.2/docs/_colors/paper:orange.png
+-rw-r--r--   0 beojan    (1000) beojan    (1000)      436 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.2/docs/_colors/paper:pink.png
+-rw-r--r--   0 beojan    (1000) beojan    (1000)      436 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.2/docs/_colors/paper:purple.png
+-rw-r--r--   0 beojan    (1000) beojan    (1000)      436 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.2/docs/_colors/paper:red.png
+-rw-r--r--   0 beojan    (1000) beojan    (1000)      435 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.2/docs/_colors/paper:yellow.png
+-rw-r--r--   0 beojan    (1000) beojan    (1000)      437 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.2/docs/_colors/series2:blue.png
+-rw-r--r--   0 beojan    (1000) beojan    (1000)      435 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.2/docs/_colors/series2:green.png
+-rw-r--r--   0 beojan    (1000) beojan    (1000)      436 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.2/docs/_colors/series2:purple.png
+-rw-r--r--   0 beojan    (1000) beojan    (1000)      437 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.2/docs/_colors/series2:red.png
+-rw-r--r--   0 beojan    (1000) beojan    (1000)      437 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.2/docs/_colors/series2:yellow.png
+-rw-r--r--   0 beojan    (1000) beojan    (1000)      439 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.2/docs/_colors/series:blue.png
+-rw-r--r--   0 beojan    (1000) beojan    (1000)      438 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.2/docs/_colors/series:cyan.png
+-rw-r--r--   0 beojan    (1000) beojan    (1000)      438 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.2/docs/_colors/series:green.png
+-rw-r--r--   0 beojan    (1000) beojan    (1000)      438 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.2/docs/_colors/series:olive.png
+-rw-r--r--   0 beojan    (1000) beojan    (1000)      439 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.2/docs/_colors/series:orange.png
+-rw-r--r--   0 beojan    (1000) beojan    (1000)      439 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.2/docs/_colors/series:pink.png
+-rw-r--r--   0 beojan    (1000) beojan    (1000)      439 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.2/docs/_colors/series:purple.png
+-rw-r--r--   0 beojan    (1000) beojan    (1000)      438 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.2/docs/_colors/series:turquoise.png
+-rw-r--r--   0 beojan    (1000) beojan    (1000)      433 2019-05-02 13:29:02.000000 atlas-mpl-style-0.9.2/docs/_colors/transparent.png
+-rw-r--r--   0 beojan    (1000) beojan    (1000)      100 2019-05-02 12:46:57.000000 atlas-mpl-style-0.9.2/docs/atlas-mpl-style.rst
+-rw-r--r--   0 beojan    (1000) beojan    (1000)     9130 2019-05-02 13:16:57.000000 atlas-mpl-style-0.9.2/docs/colors.rst
+-rw-r--r--   0 beojan    (1000) beojan    (1000)     1928 2019-05-02 14:16:15.000000 atlas-mpl-style-0.9.2/docs/conf.py
+-rw-r--r--   0 beojan    (1000) beojan    (1000)      527 2019-05-02 14:16:04.000000 atlas-mpl-style-0.9.2/docs/index.rst
+-rw-r--r--   0 beojan    (1000) beojan    (1000)      787 2019-05-02 12:37:59.000000 atlas-mpl-style-0.9.2/docs/make.bat
+-rw-r--r--   0 beojan    (1000) beojan    (1000)       20 2019-05-02 14:02:21.000000 atlas-mpl-style-0.9.2/docs/requirements.txt
+-rw-r--r--   0 beojan    (1000) beojan    (1000)     1063 2019-05-02 13:52:56.000000 atlas-mpl-style-0.9.2/docs/styles.rst
+-rw-r--r--   0 beojan    (1000) beojan    (1000)       38 2020-02-01 09:53:20.860234 atlas-mpl-style-0.9.2/setup.cfg
+-rw-r--r--   0 beojan    (1000) beojan    (1000)     2779 2020-02-01 09:51:49.000000 atlas-mpl-style-0.9.2/setup.py
```

### Comparing `atlas-mpl-style-0.9.1/LICENSE.md` & `atlas-mpl-style-0.9.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `atlas-mpl-style-0.9.1/PKG-INFO` & `atlas-mpl-style-0.9.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: atlas-mpl-style
-Version: 0.9.1
+Version: 0.9.2
 Summary: ATLAS style for Matplotlib 2.0+
 Home-page: https://github.com/beojan/atlas-mpl
 Author: Beojan Stanislaus
 Author-email: beojan.stanislaus@cern.ch
 License: GPL v3+
 Description: ATLAS Matplotlib Style
         ======================
```

### Comparing `atlas-mpl-style-0.9.1/README.rst` & `atlas-mpl-style-0.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `atlas-mpl-style-0.9.1/atlas_mpl_style/__init__.py` & `atlas-mpl-style-0.9.2/atlas_mpl_style/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,25 +144,25 @@
     """
     global _atlas_label
     _style.use("atlas")
     _atlas_label = atlasLabel
     _mpl.rcParams["font.size"] = 16
     _mpl.rcParams["xtick.minor.visible"] = True
     _mpl.rcParams["ytick.minor.visible"] = True
-    _mpl.rcParams["text.latex.preamble"] = [
+    _mpl.rcParams["text.latex.preamble"] = "\n".join([
         r"\usepackage[LGR,T1]{fontenc}",
         r"\usepackage{tgheros}",
         r"\renewcommand{\familydefault}{\sfdefault}",
         r"\usepackage{amsmath}",
         r"\usepackage[symbolgreek,symbolmax]{mathastext}",
         r"\usepackage{physics}",
         r"\usepackage{siunitx}",
         r"\setlength{\parindent}{0pt}",
         r"\def\mathdefault{}"
-    ]
+    ])
 
 
 def set_xlabel(label, ax=None, *args, **kwargs):
     """
     Set x label in ATLAS style (right aligned).
 
     Additional parameters are passed through to `ax.set_xlabel`.
```

### Comparing `atlas-mpl-style-0.9.1/atlas_mpl_style/stylesheets/atlas.mplstyle` & `atlas-mpl-style-0.9.2/atlas_mpl_style/stylesheets/atlas.mplstyle`

 * *Files identical despite different names*

### Comparing `atlas-mpl-style-0.9.1/atlas_mpl_style/stylesheets/paper.mplstyle` & `atlas-mpl-style-0.9.2/atlas_mpl_style/stylesheets/paper.mplstyle`

 * *Files identical despite different names*

### Comparing `atlas-mpl-style-0.9.1/atlas_mpl_style/stylesheets/print.mplstyle` & `atlas-mpl-style-0.9.2/atlas_mpl_style/stylesheets/print.mplstyle`

 * *Files identical despite different names*

### Comparing `atlas-mpl-style-0.9.1/atlas_mpl_style.egg-info/PKG-INFO` & `atlas-mpl-style-0.9.2/atlas_mpl_style.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: atlas-mpl-style
-Version: 0.9.1
+Version: 0.9.2
 Summary: ATLAS style for Matplotlib 2.0+
 Home-page: https://github.com/beojan/atlas-mpl
 Author: Beojan Stanislaus
 Author-email: beojan.stanislaus@cern.ch
 License: GPL v3+
 Description: ATLAS Matplotlib Style
         ======================
```

### Comparing `atlas-mpl-style-0.9.1/atlas_mpl_style.egg-info/SOURCES.txt` & `atlas-mpl-style-0.9.2/atlas_mpl_style.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atlas-mpl-style-0.9.1/docs/Makefile` & `atlas-mpl-style-0.9.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `atlas-mpl-style-0.9.1/docs/colors.rst` & `atlas-mpl-style-0.9.2/docs/colors.rst`

 * *Files identical despite different names*

### Comparing `atlas-mpl-style-0.9.1/docs/conf.py` & `atlas-mpl-style-0.9.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `atlas-mpl-style-0.9.1/docs/index.rst` & `atlas-mpl-style-0.9.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `atlas-mpl-style-0.9.1/docs/make.bat` & `atlas-mpl-style-0.9.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `atlas-mpl-style-0.9.1/docs/styles.rst` & `atlas-mpl-style-0.9.2/docs/styles.rst`

 * *Files identical despite different names*

### Comparing `atlas-mpl-style-0.9.1/setup.py` & `atlas-mpl-style-0.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 setup(
     name='atlas-mpl-style',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.9.1',
+    version='0.9.2',
 
     description='ATLAS style for Matplotlib 2.0+',
     long_description=long_description,
 
     # The project's main homepage.
     url='https://github.com/beojan/atlas-mpl',
```

