# Comparing `tmp/widgetron-0.1.8.tar.gz` & `tmp/widgetron-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "widgetron-0.1.8.tar", last modified: Wed Apr 26 20:30:27 2023, max compression
+gzip compressed data, was "widgetron-0.1.9.tar", last modified: Thu May  4 17:02:39 2023, max compression
```

## Comparing `widgetron-0.1.8.tar` & `widgetron-0.1.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:30:27.380339 widgetron-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-26 20:28:38.000000 widgetron-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-04-26 20:30:27.380339 widgetron-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-04-26 20:28:38.000000 widgetron-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-26 20:30:27.380339 widgetron-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-26 20:28:38.000000 widgetron-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:30:27.376339 widgetron-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:30:27.376339 widgetron-0.1.8/src/widgetron/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-26 20:28:38.000000 widgetron-0.1.8/src/widgetron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8049 2023-04-26 20:28:38.000000 widgetron-0.1.8/src/widgetron/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-04-26 20:28:38.000000 widgetron-0.1.8/src/widgetron/args.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:30:27.376339 widgetron-0.1.8/src/widgetron/icons/
--rw-r--r--   0 runner    (1001) docker     (123)    40675 2023-04-26 20:28:38.000000 widgetron-0.1.8/src/widgetron/icons/widgetron.icns
--rw-r--r--   0 runner    (1001) docker     (123)    11635 2023-04-26 20:28:38.000000 widgetron-0.1.8/src/widgetron/icons/widgetron.ico
--rw-r--r--   0 runner    (1001) docker     (123)    23698 2023-04-26 20:28:38.000000 widgetron-0.1.8/src/widgetron/icons/widgetron.png
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-26 20:28:38.000000 widgetron-0.1.8/src/widgetron/jinja_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-04-26 20:28:38.000000 widgetron-0.1.8/src/widgetron/parse_args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:30:27.376339 widgetron-0.1.8/src/widgetron/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:30:27.376339 widgetron-0.1.8/src/widgetron/templates/constructor/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-26 20:28:38.000000 widgetron-0.1.8/src/widgetron/templates/constructor/construct.yaml_template
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-26 20:28:38.000000 widgetron-0.1.8/src/widgetron/templates/constructor/post_install.sh_template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:30:27.376339 widgetron-0.1.8/src/widgetron/templates/electron/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-26 20:28:38.000000 widgetron-0.1.8/src/widgetron/templates/electron/index.html_template
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-04-26 20:28:38.000000 widgetron-0.1.8/src/widgetron/templates/electron/main.js_template
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-26 20:28:38.000000 widgetron-0.1.8/src/widgetron/templates/electron/package.json_template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:30:27.376339 widgetron-0.1.8/src/widgetron/templates/recipe/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-26 20:28:38.000000 widgetron-0.1.8/src/widgetron/templates/recipe/bld.bat_template
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-26 20:28:38.000000 widgetron-0.1.8/src/widgetron/templates/recipe/meta.yaml_template
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-26 20:28:38.000000 widgetron-0.1.8/src/widgetron/templates/recipe/widgetron_shortcut.json_template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:30:27.376339 widgetron-0.1.8/src/widgetron/templates/server/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-26 20:28:38.000000 widgetron-0.1.8/src/widgetron/templates/server/setup.cfg_template
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-26 20:28:38.000000 widgetron-0.1.8/src/widgetron/templates/server/setup.py_template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:30:27.380339 widgetron-0.1.8/src/widgetron/templates/server/widgetron_app/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-26 20:28:38.000000 widgetron-0.1.8/src/widgetron/templates/server/widgetron_app/__init__.py_template
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-26 20:28:38.000000 widgetron-0.1.8/src/widgetron/templates/server/widgetron_app/__main__.pyw_template
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-04-26 20:28:38.000000 widgetron-0.1.8/src/widgetron/templates/server/widgetron_app/cli.py_template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:30:27.380339 widgetron-0.1.8/src/widgetron/templates/server/widgetron_app/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-04-26 20:28:38.000000 widgetron-0.1.8/src/widgetron/templates/server/widgetron_app/notebooks/debug.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:30:27.376339 widgetron-0.1.8/src/widgetron.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-04-26 20:30:27.000000 widgetron-0.1.8/src/widgetron.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-26 20:30:27.000000 widgetron-0.1.8/src/widgetron.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 20:30:27.000000 widgetron-0.1.8/src/widgetron.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-26 20:30:27.000000 widgetron-0.1.8/src/widgetron.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 20:30:27.000000 widgetron-0.1.8/src/widgetron.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-26 20:30:27.000000 widgetron-0.1.8/src/widgetron.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-26 20:30:27.000000 widgetron-0.1.8/src/widgetron.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:02:39.113972 widgetron-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-04 17:00:56.000000 widgetron-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-05-04 17:02:39.113972 widgetron-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-04 17:00:56.000000 widgetron-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-04 17:02:39.117972 widgetron-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-04 17:00:56.000000 widgetron-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:02:39.109972 widgetron-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:02:39.113972 widgetron-0.1.9/src/widgetron/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-04 17:00:56.000000 widgetron-0.1.9/src/widgetron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10870 2023-05-04 17:00:56.000000 widgetron-0.1.9/src/widgetron/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9302 2023-05-04 17:00:56.000000 widgetron-0.1.9/src/widgetron/args.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:02:39.113972 widgetron-0.1.9/src/widgetron/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)    40675 2023-05-04 17:00:56.000000 widgetron-0.1.9/src/widgetron/icons/widgetron.icns
+-rw-r--r--   0 runner    (1001) docker     (123)    11635 2023-05-04 17:00:56.000000 widgetron-0.1.9/src/widgetron/icons/widgetron.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    23698 2023-05-04 17:00:56.000000 widgetron-0.1.9/src/widgetron/icons/widgetron.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-04 17:00:56.000000 widgetron-0.1.9/src/widgetron/jinja_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-04 17:00:56.000000 widgetron-0.1.9/src/widgetron/parse_args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:02:39.113972 widgetron-0.1.9/src/widgetron/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:02:39.113972 widgetron-0.1.9/src/widgetron/templates/constructor/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-04 17:00:56.000000 widgetron-0.1.9/src/widgetron/templates/constructor/construct.yaml_template
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-04 17:00:56.000000 widgetron-0.1.9/src/widgetron/templates/constructor/post_install.sh_template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:02:39.113972 widgetron-0.1.9/src/widgetron/templates/electron/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-04 17:00:56.000000 widgetron-0.1.9/src/widgetron/templates/electron/index.html_template
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-05-04 17:00:56.000000 widgetron-0.1.9/src/widgetron/templates/electron/main.js_template
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-04 17:00:56.000000 widgetron-0.1.9/src/widgetron/templates/electron/package.json_template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:02:39.113972 widgetron-0.1.9/src/widgetron/templates/recipe/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-04 17:00:56.000000 widgetron-0.1.9/src/widgetron/templates/recipe/bld.bat_template
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-04 17:00:56.000000 widgetron-0.1.9/src/widgetron/templates/recipe/meta.yaml_template
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-04 17:00:56.000000 widgetron-0.1.9/src/widgetron/templates/recipe/widgetron_shortcut.json_template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:02:39.113972 widgetron-0.1.9/src/widgetron/templates/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-04 17:00:56.000000 widgetron-0.1.9/src/widgetron/templates/server/setup.cfg_template
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-04 17:00:56.000000 widgetron-0.1.9/src/widgetron/templates/server/setup.py_template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:02:39.113972 widgetron-0.1.9/src/widgetron/templates/server/widgetron_app/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-04 17:00:56.000000 widgetron-0.1.9/src/widgetron/templates/server/widgetron_app/__init__.py_template
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-04 17:00:56.000000 widgetron-0.1.9/src/widgetron/templates/server/widgetron_app/__main__.pyw_template
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-05-04 17:00:56.000000 widgetron-0.1.9/src/widgetron/templates/server/widgetron_app/cli.py_template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:02:39.113972 widgetron-0.1.9/src/widgetron/templates/server/widgetron_app/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-05-04 17:00:56.000000 widgetron-0.1.9/src/widgetron/templates/server/widgetron_app/notebooks/debug.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:02:39.113972 widgetron-0.1.9/src/widgetron.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-05-04 17:02:39.000000 widgetron-0.1.9/src/widgetron.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-04 17:02:39.000000 widgetron-0.1.9/src/widgetron.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 17:02:39.000000 widgetron-0.1.9/src/widgetron.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-04 17:02:39.000000 widgetron-0.1.9/src/widgetron.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 17:02:38.000000 widgetron-0.1.9/src/widgetron.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-04 17:02:39.000000 widgetron-0.1.9/src/widgetron.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-04 17:02:39.000000 widgetron-0.1.9/src/widgetron.egg-info/top_level.txt
```

### Comparing `widgetron-0.1.8/LICENSE` & `widgetron-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `widgetron-0.1.8/PKG-INFO` & `widgetron-0.1.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: widgetron
-Version: 0.1.8
+Version: 0.1.9
 Summary: Application builder for ipython notebooks
 Author: Joel Stansbury
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: Markdown
 License-File: LICENSE
 
@@ -20,46 +20,42 @@
 pip install widgetron
 widgetron -h
 ```
 
 ### How it Works
 
 1. Builds and packages a minimal electron interface to navigate to
-   `localhost:8866` and boot up the `jupyter lab` server
-2. Copies a notebook (specified by `-f`) into a template python
-   package
+   `localhost:8866` and boot up the `jupyter lab` server.
+2. Copies a notebook or directory of notebooks (specified by `-nb`) into a
+   template python package.
 3. Copies the entire contents of the built electron application into the
    template python package.
-4. Optionally copies a source code directory (specified by `-src`), if
-   provided, into the template python package.
-
-   -  The package specifies `**` for package_data so be sure to clean
-      out any `__pycache__` folders and other garbage.
-   -  Must be a valid python package (i.e. the folder must contain
-      `__init__.py`)
-
-5. Makes a conda-package out of the python package template to hold the
-   notebook, electron app, and source code if provided.
-6. Builds an installer
-
-   -  Conda dependencies are specified with the `-deps` parameter (see
-      example).
+4. Makes a conda-package out of the python package template to hold the
+   notebook and packaged electron app.
+5. Builds an installer using conda/constructor.
 
 ### Development Guide
 Before you run `widgetron`
-1. Create a conda environment yaml to define your dependencies
+1. Conda dependencies are specified using one of the following paradigms. (pip dependencies are ignored)
 
-   - pip dependencies are not supported
+   - `dependencies` and `channels`. 2 lists of strings identifying which packages
+      to search for and which channels are searched.
+      e.g. `widgetron . -nb my_notebook.ipynb --dependencies numpy matplotlib --channels conda-forge`
+      `jupyterlab`, `conda`, and `menuinst` (if Windows) are included by default.
+   - `environment`. Pre-built conda environment which must contain `jupyterlab`
+      `conda` and `menuinst` (if Windows).
+   - `explicit_lock`. Lockfile representing the exact package urls to be included
+      in the environment. This env will be built within the widgetron work directory
+      and the installer will be built from that env. This option allows the
+      creatioin of a Software Bill of Materials (SBOM) for the conda packages.
 
-2. If you want to create a Software Bill of Materials (SBOM), then you'll need to also lock this environment
-   and provide the lockfile to the `explicit_lock` parameter.
-
-3. Create a `pyproject.toml` or `setup.cfg` and follow the examples to see
+2. Create a `pyproject.toml` or `setup.cfg` and follow the examples to see
    how these should be formatted.
-4. If you have additional source code to include there are two options for how to do so
+
+3. If you have additional source code to include there are two options for how to do so
 
    - (Recommended) create a conda package (using `conda-build`) and add it to the `-deps` argument.
    - (Easy, and dangerous) Include the raw source files
 
       - If your `--notebook` argument is a single notebook, then point the `-src` parameter to the root of your python module.
       - If your `--notebook` argument is a directory, then your source code must be placed inside this directory and be relatively importable.
       - __Warning__: this includes __EVERYTHING__ so delete your `__pycache__`s and `.env`s etc.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `widgetron-0.1.8/README.md` & `widgetron-0.1.9/src/widgetron.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: widgetron
+Version: 0.1.9
+Summary: Application builder for ipython notebooks
+Author: Joel Stansbury
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: Markdown
+License-File: LICENSE
+
 <img src="https://user-images.githubusercontent.com/48299585/213842033-c0c19779-84b9-4a07-83a0-9b75ef4b3971.JPG" alt="drawing" width="500"/>
 
 This command line utility builds a standalone executable installer for a
 single ipython notebook. It is intended for applications built with
 ipywidgets.
 
 ## Quickstart
@@ -10,46 +20,42 @@
 pip install widgetron
 widgetron -h
 ```
 
 ### How it Works
 
 1. Builds and packages a minimal electron interface to navigate to
-   `localhost:8866` and boot up the `jupyter lab` server
-2. Copies a notebook (specified by `-f`) into a template python
-   package
+   `localhost:8866` and boot up the `jupyter lab` server.
+2. Copies a notebook or directory of notebooks (specified by `-nb`) into a
+   template python package.
 3. Copies the entire contents of the built electron application into the
    template python package.
-4. Optionally copies a source code directory (specified by `-src`), if
-   provided, into the template python package.
-
-   -  The package specifies `**` for package_data so be sure to clean
-      out any `__pycache__` folders and other garbage.
-   -  Must be a valid python package (i.e. the folder must contain
-      `__init__.py`)
-
-5. Makes a conda-package out of the python package template to hold the
-   notebook, electron app, and source code if provided.
-6. Builds an installer
-
-   -  Conda dependencies are specified with the `-deps` parameter (see
-      example).
+4. Makes a conda-package out of the python package template to hold the
+   notebook and packaged electron app.
+5. Builds an installer using conda/constructor.
 
 ### Development Guide
 Before you run `widgetron`
-1. Create a conda environment yaml to define your dependencies
-
-   - pip dependencies are not supported
+1. Conda dependencies are specified using one of the following paradigms. (pip dependencies are ignored)
 
-2. If you want to create a Software Bill of Materials (SBOM), then you'll need to also lock this environment
-   and provide the lockfile to the `explicit_lock` parameter.
+   - `dependencies` and `channels`. 2 lists of strings identifying which packages
+      to search for and which channels are searched.
+      e.g. `widgetron . -nb my_notebook.ipynb --dependencies numpy matplotlib --channels conda-forge`
+      `jupyterlab`, `conda`, and `menuinst` (if Windows) are included by default.
+   - `environment`. Pre-built conda environment which must contain `jupyterlab`
+      `conda` and `menuinst` (if Windows).
+   - `explicit_lock`. Lockfile representing the exact package urls to be included
+      in the environment. This env will be built within the widgetron work directory
+      and the installer will be built from that env. This option allows the
+      creatioin of a Software Bill of Materials (SBOM) for the conda packages.
 
-3. Create a `pyproject.toml` or `setup.cfg` and follow the examples to see
+2. Create a `pyproject.toml` or `setup.cfg` and follow the examples to see
    how these should be formatted.
-4. If you have additional source code to include there are two options for how to do so
+
+3. If you have additional source code to include there are two options for how to do so
 
    - (Recommended) create a conda package (using `conda-build`) and add it to the `-deps` argument.
    - (Easy, and dangerous) Include the raw source files
 
       - If your `--notebook` argument is a single notebook, then point the `-src` parameter to the root of your python module.
       - If your `--notebook` argument is a directory, then your source code must be placed inside this directory and be relatively importable.
       - __Warning__: this includes __EVERYTHING__ so delete your `__pycache__`s and `.env`s etc.
@@ -79,8 +85,8 @@
 
 ![image](https://user-images.githubusercontent.com/48299585/211173745-9142808c-6303-4925-b1f2-d7db21430df1.png)
 
 Window
 
 ![image](https://user-images.githubusercontent.com/48299585/211173814-af05502c-2c41-4bd1-ad09-324a9eccef78.png)
 
-Profit
+Profit
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `widgetron-0.1.8/setup.cfg` & `widgetron-0.1.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `widgetron-0.1.8/src/widgetron/__main__.py` & `widgetron-0.1.9/src/widgetron/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+import json
 import os
 import platform
 import re
 import shutil
 import sys
 import zipfile
 from pathlib import Path
-from subprocess import check_call
+from subprocess import check_call, Popen, PIPE
 
 import yaml
 
 from .parse_args import CONFIG
 
 
 def zipdir(path, ziph):
@@ -23,20 +24,21 @@
 
 
 from .jinja_functions import render_templates
 
 HERE = Path(__file__).parent
 PYTHON = Path(sys.executable)
 CONDA_PREFIX = PYTHON.parent
+REQUIRED_PKGS = ["jupyterlab", "conda"]
 
 WIN = platform.system() == "Windows"
 LINUX = platform.system() == "Linux"
 OSX = platform.system() == "Darwin"
 
-CONDA_BUILD = "conda-mambabuild {} -c https://conda.anaconda.org/conda-forge --no-test --no-verify"
+CONDA_BUILD = "conda-mambabuild {} -c https://conda.anaconda.org/conda-forge --no-test --no-verify --output-folder {}"
 DEFAULT_SERVER_COMMAND = ["jupyter", "lab", "--no-browser"]
 
 if WIN:
     DEFAULT_ICON = HERE / "icons/widgetron.ico"
 elif LINUX:
     DEFAULT_ICON = HERE / "icons/widgetron.png"
 elif OSX:
@@ -45,83 +47,97 @@
     raise OSError(f"Unknown platform {platform.system()}")
 
 # Single valued parameters specific to the construc.yaml file
 CONSTRUCTOR_PARAMS = {
     "company": str,
     "installer_filename": str,
     "installer_type": str,
-    "license_file": lambda x:Path(x).absolute(),
+    "license_file": lambda x: Path(x).absolute(),
     "batch_mode": str,
     "signing_identity_name": str,
-    "welcome_image": lambda x:Path(x).absolute(),
-    "header_image": lambda x:Path(x).absolute(),
+    "welcome_image": lambda x: Path(x).absolute(),
+    "header_image": lambda x: Path(x).absolute(),
     "default_image_color": str,
     "welcome_image_text": str,
     "header_image_text": str,
-    "nsis_template": lambda x:Path(x).absolute(),
+    "nsis_template": lambda x: Path(x).absolute(),
     "default_prefix": str,
     "default_prefix_domain_user": str,
-    "default_prefix_all_users": str
+    "default_prefix_all_users": str,
+    "environment": lambda x: Path(x).absolute(),
 }
 
+
+def _validate_env(env):
+    missing = []
+    for pkg in REQUIRED_PKGS:
+        if not _is_installed(env, pkg):
+            missing.append(pkg)
+    if WIN:
+        if not _is_installed(env, "menuinst"):
+            missing.append("menuinst >=1.4.17")
+    return missing
+
+
+def _is_installed(env, library):
+    CONDA = shutil.which("conda")
+    cmd = f"{CONDA} list --prefix {env} -f {library} --no-pip --json".split()
+    p = Popen(cmd, stdout=PIPE, stderr=PIPE)
+    output, err = p.communicate()
+    return bool(json.loads(output))
+
+
+def _install_missing_pkgs(env, pkgs):
+    CONDA = shutil.which("conda")
+    check_call(
+        [CONDA, "install", "--prefix", str(env), "-y", *pkgs, "-c", "conda-forge"]
+    )
+
+
 def parse_arguments():
     kwargs = CONFIG
     kwargs["dependencies"] = kwargs.get("dependencies", [])
-    kwargs["channels"] = kwargs.get("channels", ["https://conda.anaconda.org/conda-forge"])
+    kwargs["channels"] = kwargs.get(
+        "channels", ["https://conda.anaconda.org/conda-forge"]
+    )
 
     if isinstance(kwargs["dependencies"], str):
-        kwargs["dependencies"]=kwargs["dependencies"].strip().split()
+        kwargs["dependencies"] = kwargs["dependencies"].strip().split()
     if isinstance(kwargs["channels"], str):
-        kwargs["channels"]=kwargs["channels"].strip().split()
+        kwargs["channels"] = kwargs["channels"].strip().split()
 
-    if "explicit_lock" in kwargs:
-        with open(kwargs["explicit_lock"], "r") as f:
-            l = f.readline()
-            while "@EXPLICIT" not in l:
-                l = f.readline()
-            kwargs["dependencies"] += [s.strip() for s in f.readlines()]
-        cmd = [
-            "jake",
-            "sbom",
-            "-t=CONDA",
-            f"-f={kwargs['explicit_lock']}",
-            "--output-format=json",
-            f"-o={Path(kwargs['outdir'])/'conda-sbom.json'}"
-        ]
-        print(cmd)
-        check_call(cmd)
     elif "environment_yaml" in kwargs:
         with open(kwargs["environment_yaml"], "r") as f:
             _env = yaml.safe_load(f)
         kwargs["dependencies"] += _env["dependencies"]
-        kwargs["channels"] +=  _env["channels"]
+        kwargs["channels"] += _env["channels"]
 
     kwargs["server_command"] = kwargs.get("server_command", DEFAULT_SERVER_COMMAND)
     if isinstance(kwargs["server_command"], str):
-        kwargs["server_command"]=kwargs["server_command"].strip().split()
+        kwargs["server_command"] = kwargs["server_command"].strip().split()
 
     # cli.py template requires executable and cli args to be separated.
     if kwargs["server_command"][0] == "jupyter":  # "jupyter lab"
-        kwargs["server_executable"] = '-'.join(kwargs["server_command"][:2])
+        kwargs["server_executable"] = "-".join(kwargs["server_command"][:2])
         kwargs["server_command_args"] = kwargs["server_command"][2:]
-    elif 'jupyter-' in kwargs["server_command"][0]:  # "jupyter-lab"
+    elif "jupyter-" in kwargs["server_command"][0]:  # "jupyter-lab"
         kwargs["server_executable"] = kwargs["server_command"][0]
         kwargs["server_command_args"] = kwargs["server_command"][1:]
     else:
         raise ValueError(
             "server command did not follow expected syntax ('jupyter-cmd' or 'jupyter cmd')"
         )
 
     kwargs["url_whitelist"] = kwargs.get("url_whitelist", [])
     if isinstance(kwargs["url_whitelist"], str):
-        kwargs["url_whitelist"]=kwargs["url_whitelist"].strip().split()
+        kwargs["url_whitelist"] = kwargs["url_whitelist"].strip().split()
 
     kwargs["domain_whitelist"] = kwargs.get("domain_whitelist", [])
     if isinstance(kwargs["domain_whitelist"], str):
-        kwargs["domain_whitelist"]=kwargs["domain_whitelist"].strip().split()
+        kwargs["domain_whitelist"] = kwargs["domain_whitelist"].strip().split()
 
     assert isinstance(kwargs["server_command"], list)
     assert "version" in kwargs
 
     kwargs["icon"] = kwargs.get("icon", DEFAULT_ICON)
 
     kwargs["name"] = Path(kwargs["notebook"]).stem
@@ -129,34 +145,86 @@
     pat = re.compile(r"[^a-zA-Z0-9]")
     kwargs["name_nospace"] = pat.sub("_", kwargs["name"])
 
     kwargs["icon_name"] = Path(kwargs["icon"]).name
     kwargs["temp_files"] = Path("widgetron_temp_files")
     kwargs["filename"] = Path(kwargs["notebook"]).name
 
+    if "explicit_lock" in kwargs:
+        assert (
+            "environment" not in kwargs
+        ), "cannot provide env and lock at the same time."
+
+        # Generate SBOM (because we can)
+        cmd = [
+            "jake",
+            "sbom",
+            "-t=CONDA",
+            f"-f={kwargs['explicit_lock']}",
+            "--output-format=json",
+            f"-o={Path(kwargs['outdir'])/'conda-sbom.json'}",
+        ]
+        check_call(cmd)
+
+        # Build the environment and reference the env directory
+        check_call(
+            [
+                "conda",
+                "create",
+                "--file",
+                kwargs["explicit_lock"],
+                "--prefix",
+                kwargs["temp_files"] / ".env",
+            ]
+        )
+        kwargs["environment"] = kwargs["temp_files"] / ".env"
+
+    if "environment" in kwargs:
+        env = kwargs["environment"]
+        missing_pkgs = _validate_env(env)
+        if missing_pkgs:
+            print(
+                "Error: Explicit environment is missing the following required packages"
+            )
+            for m in missing_pkgs:
+                print(f"  - {m}")
+            inp = input(
+                f"Would you like to install them to {env} from conda-forge (y/n)? "
+            )
+            if inp.lower() in ["y", "yes"]:
+                _install_missing_pkgs(env, missing_pkgs)
+            else:
+                sys.exit()
+
     kwargs["constructor_params"] = {
-        p: CONSTRUCTOR_PARAMS[p](kwargs[p])
-        for p in CONSTRUCTOR_PARAMS if p in kwargs
+        p: CONSTRUCTOR_PARAMS[p](kwargs[p]) for p in CONSTRUCTOR_PARAMS if p in kwargs
     }
 
+    if "pkg_output_dir" not in kwargs:
+        kwargs["pkg_output_dir"] = (
+            Path(kwargs["temp_files"]) / "conda_build"
+        ).absolute()
+    else:
+        kwargs["pkg_output_dir"] = Path(kwargs["pkg_output_dir"]).absolute()
+    kwargs["channels"].append(f"file:///{kwargs['pkg_output_dir']}")
     return kwargs
 
 
 def copy_source_code(kwargs):
     # Copy python source into template package
     # notebook dir already exists due to debug notebook
     dest = kwargs["temp_files"] / "server/widgetron_app/notebooks"
     # TODO: alter dest if kwargs["notebook"] is a directory
 
     if "python_source" in kwargs:
         if Path(kwargs["python_source"]).is_dir():
-            shutil.copytree(
-                kwargs["python_source"],
-                dest / Path(kwargs["python_source"]).stem,
-            )
+            dest = dest / Path(kwargs["python_source"]).stem
+            if dest.exists():
+                shutil.rmtree(dest)
+            shutil.copytree(kwargs["python_source"], dest)
         elif Path(kwargs["python_source"]).is_file():
             shutil.copy(
                 kwargs["python_source"],
                 dest,
             )
 
 
@@ -166,40 +234,48 @@
     dest = kwargs["temp_files"] / "server/widgetron_app/notebooks"
     nb = Path(kwargs["notebook"])
 
     if nb.is_file():
         assert nb.suffix.lower() == ".ipynb", f"{nb} is not a notebook"
         shutil.copy(nb, dest)
     else:
+        dest = dest / nb.stem
+        if dest.exists():
+            shutil.rmtree(dest)
         assert list(nb.glob("*.ipynb")), f"No notebooks found in {nb}"
-        shutil.copytree(nb, dest / nb.stem)
+        shutil.copytree(nb, dest)
 
 
 def package_electron_app(kwargs):
     icon = Path(kwargs["icon"]).absolute()
     cwd = Path().absolute()
 
     os.chdir(str(kwargs["temp_files"] / "electron"))
-    os.mkdir("build")
+    Path("build").mkdir(exist_ok=True)
     # assert icon.suffix.lower() == ".png", "WIP: only png currently supported"
     shutil.copy(str(icon), f"build/icon{icon.suffix}")
 
     check_call("npm install .", shell=True)
-    sbom = Path(kwargs['outdir']) / 'npm-sbom.json'
-    cmd = [
-        "npm", "run", "lock", "--",
-        "--output-format", "json",
-        "--output-file", f"{sbom}"
-    ]
-    print(cmd)
-    check_call(cmd, shell=True)
+    sbom = Path(kwargs["outdir"]) / "npm-sbom.json"
     check_call(
         "npm run build",
         shell=True,
     )
+    cmd = [
+        "npm",
+        "run",
+        "lock",
+        "--",
+        "--output-format",
+        "json",
+        "--output-file",
+        f"{sbom}",
+    ]
+    check_call(cmd, shell=True)
+
     if OSX or LINUX:
         dist = "dist"
     elif WIN:
         dist = "dist/win-unpacked"
 
     os.chdir(dist)
 
@@ -222,15 +298,32 @@
     icon = Path(kwargs["icon"])
     shutil.copy(str(icon), kwargs["temp_files"] / f"recipe/{icon.name}")
     kwargs["icon"] = icon.name
 
 
 def build_conda_package(kwargs):
     dir = kwargs["temp_files"] / "recipe"
-    check_call(CONDA_BUILD.format(dir), shell=True)
+    check_call(CONDA_BUILD.format(dir, kwargs["pkg_output_dir"]), shell=True)
+    if "environment" in kwargs:
+        check_call(
+            [
+                "conda",
+                "run",
+                "--prefix",
+                kwargs["environment"],
+                "conda",
+                "install",
+                "-y",
+                "widgetron_app",
+                "-c",
+                f"file:///{Path(kwargs['pkg_output_dir']).absolute()}",
+                "--no-shortcuts",
+                "--force-reinstall",
+            ]
+        )
 
 
 def build_installer(kwargs):
     dir = kwargs["temp_files"] / "constructor"
     check_call(f"constructor {dir} --output-dir {kwargs['outdir']}", shell=True)
```

### Comparing `widgetron-0.1.8/src/widgetron/args.yml` & `widgetron-0.1.9/src/widgetron/args.yml`

 * *Files 12% similar despite different names*

```diff
@@ -15,18 +15,29 @@
     flag: "-nb"
     help: "Path to notebook to convert. (must be .ipynb or a directory)"
 
 version:
     flag: "-v"
     help: "Version number."
 
-environment_yaml:
-    flag: "-env"
-    help: "Path to environment.yml"
-    
+environment:
+    flag: "-environment"
+    help: |
+        Path to pre-built environment.
+        If provided, the dependencies argument is ignored.
+        If provided, the channels argument is ignored.
+        The widgetron_app package will be installed to this environment and the
+        installer will build directly from this env.
+        This option is useful for debugging as you can test it with...
+        `conda activate {environment} && python -m widgetron_app`
+
+pkg_output_dir:
+    flag: "--pkg_output_dir"
+    help: "Where to place intermediate conda packages."
+
 dependencies:
     flag: "-deps"
     nargs: "+"
     help: |
         List of conda packages required to run the widget
         (pip packages are not supported). If environment_yaml or explicit_lock
         are also provided, then those are appended to the list of dependencies.
@@ -40,14 +51,22 @@
         If environment_yaml or explicit_lock are also provided, then those are
         appended to the list of channels.
 
 explicit_lock:
     flag: "-lock"
     help: |
         Path to lock file generated via `conda-lock --kind=explicit`.
+        If provided, the dependencies argument is ignored.
+        If provided, the channels argument is ignored.
+        Widgetron will build the environment using
+        `conda create --file {explicit_lock} --prefix widgetron_temp_files/.env`
+        The widgetron_app package will be installed to this environment and the
+        installer will build directly from this env.
+        This option is useful for debugging as you can test it with...
+        `conda activate widgetron_temp_files/.env && python -m widgetron_app`
 
 python_source:
     flag: "-src"
     help: |
         This is a shortcut to avoid needing to build a conda package for your source code.
         Widgetron is basically a big jinja template, if your notebook has `from my_package import my_widget`
         then you would pass C:/path/to/my_package, and the directory will by copied recursively
```

### Comparing `widgetron-0.1.8/src/widgetron/icons/widgetron.icns` & `widgetron-0.1.9/src/widgetron/icons/widgetron.icns`

 * *Files identical despite different names*

### Comparing `widgetron-0.1.8/src/widgetron/icons/widgetron.ico` & `widgetron-0.1.9/src/widgetron/icons/widgetron.ico`

 * *Files identical despite different names*

### Comparing `widgetron-0.1.8/src/widgetron/icons/widgetron.png` & `widgetron-0.1.9/src/widgetron/icons/widgetron.png`

 * *Files identical despite different names*

### Comparing `widgetron-0.1.8/src/widgetron/jinja_functions.py` & `widgetron-0.1.9/src/widgetron/jinja_functions.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 def render_templates(**kwargs):
     """
     Renders all templates, replacing all instances of {{kw}} with the value
     provided in kwargs.
     """
     outdir = kwargs["temp_files"]
-    outdir.mkdir()
+    outdir.mkdir(exist_ok=True)
 
     for f in TEMPLATES.rglob("*.*"):
         rel = f.relative_to(TEMPLATES)
         intermediate_folders = rel.parts[:-1]
 
         # Create sub-directories in output folder
         for i in range(len(intermediate_folders)):
```

### Comparing `widgetron-0.1.8/src/widgetron/parse_args.py` & `widgetron-0.1.9/src/widgetron/parse_args.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,14 @@
         res["outdir"] = Path(res["outdir"]).absolute()
 
     # Apply defaults as specified in args.yml
     for k, v in defaults.items():
         if k not in res:
             res[k] = v
 
-
     # Override config and defaults with cli args
     res.update({k: v for k, v in kwargs.__dict__.items() if v is not None})
     res["outdir"].mkdir(exist_ok=True)
 
     return res
```

### Comparing `widgetron-0.1.8/src/widgetron/templates/electron/main.js_template` & `widgetron-0.1.9/src/widgetron/templates/electron/main.js_template`

 * *Files identical despite different names*

### Comparing `widgetron-0.1.8/src/widgetron/templates/electron/package.json_template` & `widgetron-0.1.9/src/widgetron/templates/electron/package.json_template`

 * *Files identical despite different names*

### Comparing `widgetron-0.1.8/src/widgetron/templates/server/widgetron_app/cli.py_template` & `widgetron-0.1.9/src/widgetron/templates/server/widgetron_app/cli.py_template`

 * *Files identical despite different names*

### Comparing `widgetron-0.1.8/src/widgetron/templates/server/widgetron_app/notebooks/debug.ipynb` & `widgetron-0.1.9/src/widgetron/templates/server/widgetron_app/notebooks/debug.ipynb`

 * *Files identical despite different names*

### Comparing `widgetron-0.1.8/src/widgetron.egg-info/PKG-INFO` & `widgetron-0.1.9/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: widgetron
-Version: 0.1.8
-Summary: Application builder for ipython notebooks
-Author: Joel Stansbury
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: Markdown
-License-File: LICENSE
-
 <img src="https://user-images.githubusercontent.com/48299585/213842033-c0c19779-84b9-4a07-83a0-9b75ef4b3971.JPG" alt="drawing" width="500"/>
 
 This command line utility builds a standalone executable installer for a
 single ipython notebook. It is intended for applications built with
 ipywidgets.
 
 ## Quickstart
@@ -20,46 +10,42 @@
 pip install widgetron
 widgetron -h
 ```
 
 ### How it Works
 
 1. Builds and packages a minimal electron interface to navigate to
-   `localhost:8866` and boot up the `jupyter lab` server
-2. Copies a notebook (specified by `-f`) into a template python
-   package
+   `localhost:8866` and boot up the `jupyter lab` server.
+2. Copies a notebook or directory of notebooks (specified by `-nb`) into a
+   template python package.
 3. Copies the entire contents of the built electron application into the
    template python package.
-4. Optionally copies a source code directory (specified by `-src`), if
-   provided, into the template python package.
-
-   -  The package specifies `**` for package_data so be sure to clean
-      out any `__pycache__` folders and other garbage.
-   -  Must be a valid python package (i.e. the folder must contain
-      `__init__.py`)
-
-5. Makes a conda-package out of the python package template to hold the
-   notebook, electron app, and source code if provided.
-6. Builds an installer
-
-   -  Conda dependencies are specified with the `-deps` parameter (see
-      example).
+4. Makes a conda-package out of the python package template to hold the
+   notebook and packaged electron app.
+5. Builds an installer using conda/constructor.
 
 ### Development Guide
 Before you run `widgetron`
-1. Create a conda environment yaml to define your dependencies
-
-   - pip dependencies are not supported
+1. Conda dependencies are specified using one of the following paradigms. (pip dependencies are ignored)
 
-2. If you want to create a Software Bill of Materials (SBOM), then you'll need to also lock this environment
-   and provide the lockfile to the `explicit_lock` parameter.
+   - `dependencies` and `channels`. 2 lists of strings identifying which packages
+      to search for and which channels are searched.
+      e.g. `widgetron . -nb my_notebook.ipynb --dependencies numpy matplotlib --channels conda-forge`
+      `jupyterlab`, `conda`, and `menuinst` (if Windows) are included by default.
+   - `environment`. Pre-built conda environment which must contain `jupyterlab`
+      `conda` and `menuinst` (if Windows).
+   - `explicit_lock`. Lockfile representing the exact package urls to be included
+      in the environment. This env will be built within the widgetron work directory
+      and the installer will be built from that env. This option allows the
+      creatioin of a Software Bill of Materials (SBOM) for the conda packages.
 
-3. Create a `pyproject.toml` or `setup.cfg` and follow the examples to see
+2. Create a `pyproject.toml` or `setup.cfg` and follow the examples to see
    how these should be formatted.
-4. If you have additional source code to include there are two options for how to do so
+
+3. If you have additional source code to include there are two options for how to do so
 
    - (Recommended) create a conda package (using `conda-build`) and add it to the `-deps` argument.
    - (Easy, and dangerous) Include the raw source files
 
       - If your `--notebook` argument is a single notebook, then point the `-src` parameter to the root of your python module.
       - If your `--notebook` argument is a directory, then your source code must be placed inside this directory and be relatively importable.
       - __Warning__: this includes __EVERYTHING__ so delete your `__pycache__`s and `.env`s etc.
@@ -89,8 +75,8 @@
 
 ![image](https://user-images.githubusercontent.com/48299585/211173745-9142808c-6303-4925-b1f2-d7db21430df1.png)
 
 Window
 
 ![image](https://user-images.githubusercontent.com/48299585/211173814-af05502c-2c41-4bd1-ad09-324a9eccef78.png)
 
-Profit
+Profit
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `widgetron-0.1.8/src/widgetron.egg-info/SOURCES.txt` & `widgetron-0.1.9/src/widgetron.egg-info/SOURCES.txt`

 * *Files identical despite different names*

