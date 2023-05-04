# Comparing `tmp/thonny-autosave-0.0.2.tar.gz` & `tmp/thonny-autosave-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thonny-autosave-0.0.2.tar", last modified: Thu May  4 00:06:45 2023, max compression
+gzip compressed data, was "thonny-autosave-0.0.6.tar", last modified: Thu May  4 00:43:02 2023, max compression
```

## Comparing `thonny-autosave-0.0.2.tar` & `thonny-autosave-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:06:45.873522 thonny-autosave-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:06:45.873522 thonny-autosave-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:06:45.873522 thonny-autosave-0.0.2/.github/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-05-04 00:06:36.000000 thonny-autosave-0.0.2/.github/scripts/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:06:45.873522 thonny-autosave-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-04 00:06:36.000000 thonny-autosave-0.0.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-04 00:06:36.000000 thonny-autosave-0.0.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-04 00:06:36.000000 thonny-autosave-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-04 00:06:45.873522 thonny-autosave-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-04 00:06:36.000000 thonny-autosave-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-04 00:06:36.000000 thonny-autosave-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-04 00:06:45.873522 thonny-autosave-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:06:45.873522 thonny-autosave-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:06:45.873522 thonny-autosave-0.0.2/src/thonny-autosave/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 00:06:36.000000 thonny-autosave-0.0.2/src/thonny-autosave/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-04 00:06:36.000000 thonny-autosave-0.0.2/src/thonny-autosave/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:06:45.873522 thonny-autosave-0.0.2/src/thonny_autosave.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-04 00:06:45.000000 thonny-autosave-0.0.2/src/thonny_autosave.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-04 00:06:45.000000 thonny-autosave-0.0.2/src/thonny_autosave.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 00:06:45.000000 thonny-autosave-0.0.2/src/thonny_autosave.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-04 00:06:45.000000 thonny-autosave-0.0.2/src/thonny_autosave.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-04 00:06:45.000000 thonny-autosave-0.0.2/src/thonny_autosave.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:43:02.429878 thonny-autosave-0.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:43:02.429878 thonny-autosave-0.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:43:02.429878 thonny-autosave-0.0.6/.github/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-05-04 00:42:52.000000 thonny-autosave-0.0.6/.github/scripts/release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:43:02.429878 thonny-autosave-0.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-04 00:42:52.000000 thonny-autosave-0.0.6/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-04 00:42:52.000000 thonny-autosave-0.0.6/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-04 00:42:52.000000 thonny-autosave-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-04 00:43:02.429878 thonny-autosave-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-04 00:42:52.000000 thonny-autosave-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-04 00:42:52.000000 thonny-autosave-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-04 00:43:02.429878 thonny-autosave-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:43:02.429878 thonny-autosave-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:43:02.429878 thonny-autosave-0.0.6/src/thonny_autosave.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-04 00:43:02.000000 thonny-autosave-0.0.6/src/thonny_autosave.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-04 00:43:02.000000 thonny-autosave-0.0.6/src/thonny_autosave.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 00:43:02.000000 thonny-autosave-0.0.6/src/thonny_autosave.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 00:43:02.000000 thonny-autosave-0.0.6/src/thonny_autosave.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:43:02.429878 thonny-autosave-0.0.6/src/thonnycontrib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:43:02.429878 thonny-autosave-0.0.6/src/thonnycontrib/thonny-autosave/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 00:42:52.000000 thonny-autosave-0.0.6/src/thonnycontrib/thonny-autosave/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-04 00:42:52.000000 thonny-autosave-0.0.6/src/thonnycontrib/thonny-autosave/app.py
```

### Comparing `thonny-autosave-0.0.2/.github/scripts/release.py` & `thonny-autosave-0.0.6/.github/scripts/release.py`

 * *Files identical despite different names*

### Comparing `thonny-autosave-0.0.2/LICENSE` & `thonny-autosave-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `thonny-autosave-0.0.2/setup.cfg` & `thonny-autosave-0.0.6/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 [metadata]
 name = thonny-autosave
 description = Adds a checkbox to the File menu of Thonny editor, when activated , automatically saves current file every 10 seconds.
+long_description = "# thonny-autosave
+	Adds a checkbox to the File menu of Thonny editor, when activated , Automatically saves current file every 10 seconds
+	![image](https://user-images.githubusercontent.com/3520243/236076489-a0196681-a98d-4d80-8539-ce45723606da.png)"
 long_description_content_type = text/markdown
 url = https://github.com/selmen2004/thonny-autosave
 project_urls = 
 	Bug Tracker = https://github.com/selmen2004/thonny-autosave/issues
 	Changelog = https://github.com/selmen2004/thonny-autosave/releases
 classifiers = 
 	Programming Language :: Python :: 3
@@ -16,15 +19,11 @@
 	= src
 packages = find:
 python_requires = >=3.6
 
 [options.packages.find]
 where = src
 
-[options.entry_points]
-console_scripts = 
-	gha_python_packaging_demo = gha_python_packaging_demo.app:entry_point
-
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `thonny-autosave-0.0.2/src/thonny-autosave/app.py` & `thonny-autosave-0.0.6/src/thonnycontrib/thonny-autosave/app.py`

 * *Files identical despite different names*

