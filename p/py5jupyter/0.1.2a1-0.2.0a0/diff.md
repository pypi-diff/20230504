# Comparing `tmp/py5jupyter-0.1.2a1.tar.gz` & `tmp/py5jupyter-0.2.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py5jupyter-0.1.2a1.tar", last modified: Thu May 26 01:15:03 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `py5jupyter-0.1.2a1.tar` & `py5jupyter-0.2.0a0.tar`

### file list

```diff
@@ -1,99 +1,84 @@
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2022-05-26 01:15:03.127727 py5jupyter-0.1.2a1/
--rw-rw-r--   0 jim       (1000) jim       (1000)    24436 2022-05-16 16:28:38.000000 py5jupyter-0.1.2a1/LICENSE
--rw-rw-r--   0 jim       (1000) jim       (1000)      659 2022-05-16 16:33:01.000000 py5jupyter-0.1.2a1/MANIFEST.in
--rw-rw-r--   0 jim       (1000) jim       (1000)     3101 2022-05-26 01:15:03.127727 py5jupyter-0.1.2a1/PKG-INFO
--rw-rw-r--   0 jim       (1000) jim       (1000)     1935 2022-05-23 10:42:02.000000 py5jupyter-0.1.2a1/README.md
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2022-05-26 01:15:03.121727 py5jupyter-0.1.2a1/docs/
--rw-rw-r--   0 jim       (1000) jim       (1000)      612 2022-05-07 11:17:35.000000 py5jupyter-0.1.2a1/docs/Makefile
--rw-rw-r--   0 jim       (1000) jim       (1000)      171 2022-05-07 11:17:35.000000 py5jupyter-0.1.2a1/docs/environment.yml
--rw-rw-r--   0 jim       (1000) jim       (1000)      782 2022-05-07 11:17:35.000000 py5jupyter-0.1.2a1/docs/make.bat
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2022-05-26 01:15:03.122727 py5jupyter-0.1.2a1/docs/source/
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2022-05-26 01:15:03.122727 py5jupyter-0.1.2a1/docs/source/_static/
--rw-rw-r--   0 jim       (1000) jim       (1000)     7481 2022-05-23 11:15:20.000000 py5jupyter-0.1.2a1/docs/source/_static/embed-bundle.js
--rw-rw-r--   0 jim       (1000) jim       (1000)    15456 2022-05-23 11:15:20.000000 py5jupyter-0.1.2a1/docs/source/_static/embed-bundle.js.map
--rw-rw-r--   0 jim       (1000) jim       (1000)      120 2022-05-07 11:17:35.000000 py5jupyter-0.1.2a1/docs/source/_static/helper.js
--rw-rw-r--   0 jim       (1000) jim       (1000)     6297 2022-05-07 11:17:35.000000 py5jupyter-0.1.2a1/docs/source/conf.py
--rw-rw-r--   0 jim       (1000) jim       (1000)      829 2022-05-23 11:14:32.000000 py5jupyter-0.1.2a1/docs/source/develop-install.rst
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2022-05-26 01:15:03.122727 py5jupyter-0.1.2a1/docs/source/examples/
--rw-rw-r--   0 jim       (1000) jim       (1000)      385 2022-05-07 11:17:35.000000 py5jupyter-0.1.2a1/docs/source/examples/index.rst
--rw-rw-r--   0 jim       (1000) jim       (1000)       53 2022-05-07 11:17:35.000000 py5jupyter-0.1.2a1/docs/source/examples/introduction.nblink
--rw-rw-r--   0 jim       (1000) jim       (1000)      618 2022-05-07 11:17:35.000000 py5jupyter-0.1.2a1/docs/source/index.rst
--rw-rw-r--   0 jim       (1000) jim       (1000)     1018 2022-05-07 11:17:35.000000 py5jupyter-0.1.2a1/docs/source/installing.rst
--rw-rw-r--   0 jim       (1000) jim       (1000)      109 2022-05-07 11:17:35.000000 py5jupyter-0.1.2a1/docs/source/introduction.rst
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2022-05-26 01:15:03.124727 py5jupyter-0.1.2a1/examples/
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2022-05-26 01:15:03.125727 py5jupyter-0.1.2a1/examples/.ipynb_checkpoints/
--rw-rw-r--   0 jim       (1000) jim       (1000)     3406 2022-05-13 12:11:37.000000 py5jupyter-0.1.2a1/examples/.ipynb_checkpoints/Camera3D Test-checkpoint.ipynb
--rw-rw-r--   0 jim       (1000) jim       (1000)     3492 2022-05-17 15:12:31.000000 py5jupyter-0.1.2a1/examples/.ipynb_checkpoints/Test-checkpoint.ipynb
--rw-rw-r--   0 jim       (1000) jim       (1000)     1439 2022-05-07 11:39:50.000000 py5jupyter-0.1.2a1/examples/.ipynb_checkpoints/introduction-checkpoint.ipynb
--rw-rw-r--   0 jim       (1000) jim       (1000)     1805 2022-05-15 09:40:20.000000 py5jupyter-0.1.2a1/examples/.ipynb_checkpoints/ipycanvas tests-checkpoint.ipynb
--rw-rw-r--   0 jim       (1000) jim       (1000)     3406 2022-05-13 12:11:37.000000 py5jupyter-0.1.2a1/examples/Camera3D Test.ipynb
--rw-rw-r--   0 jim       (1000) jim       (1000)     3492 2022-05-17 15:12:31.000000 py5jupyter-0.1.2a1/examples/Test.ipynb
--rw-rw-r--   0 jim       (1000) jim       (1000)     1439 2022-05-07 11:39:50.000000 py5jupyter-0.1.2a1/examples/introduction.ipynb
--rw-rw-r--   0 jim       (1000) jim       (1000)     1805 2022-05-15 09:40:20.000000 py5jupyter-0.1.2a1/examples/ipycanvas tests.ipynb
--rw-rw-r--   0 jim       (1000) jim       (1000)      181 2022-05-07 11:17:35.000000 py5jupyter-0.1.2a1/install.json
--rw-rw-r--   0 jim       (1000) jim       (1000)     2880 2022-05-23 11:14:31.000000 py5jupyter-0.1.2a1/package.json
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2022-05-26 01:15:03.125727 py5jupyter-0.1.2a1/py5jupyter/
--rw-rw-r--   0 jim       (1000) jim       (1000)     2615 2022-05-10 13:03:50.000000 py5jupyter-0.1.2a1/py5jupyter/__init__.py
--rw-rw-r--   0 jim       (1000) jim       (1000)      998 2022-05-26 01:07:42.000000 py5jupyter-0.1.2a1/py5jupyter/_version.py
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2022-05-26 01:15:03.125727 py5jupyter-0.1.2a1/py5jupyter/kernels/
--rw-rw-r--   0 jim       (1000) jim       (1000)      920 2022-05-10 13:03:50.000000 py5jupyter-0.1.2a1/py5jupyter/kernels/__init__.py
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2022-05-26 01:15:03.125727 py5jupyter-0.1.2a1/py5jupyter/kernels/py5/
--rw-rw-r--   0 jim       (1000) jim       (1000)      958 2022-05-10 13:03:50.000000 py5jupyter-0.1.2a1/py5jupyter/kernels/py5/__init__.py
--rw-rw-r--   0 jim       (1000) jim       (1000)      973 2022-05-10 13:03:50.000000 py5jupyter-0.1.2a1/py5jupyter/kernels/py5/__main__.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     2782 2022-05-10 13:03:50.000000 py5jupyter-0.1.2a1/py5jupyter/kernels/py5/install.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     2787 2022-05-10 13:03:50.000000 py5jupyter-0.1.2a1/py5jupyter/kernels/py5/kernel.py
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2022-05-26 01:15:03.125727 py5jupyter-0.1.2a1/py5jupyter/kernels/py5bot/
--rw-rw-r--   0 jim       (1000) jim       (1000)      961 2022-05-10 13:03:50.000000 py5jupyter-0.1.2a1/py5jupyter/kernels/py5bot/__init__.py
--rw-rw-r--   0 jim       (1000) jim       (1000)      979 2022-05-10 13:03:50.000000 py5jupyter-0.1.2a1/py5jupyter/kernels/py5bot/__main__.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     2800 2022-05-10 13:03:50.000000 py5jupyter-0.1.2a1/py5jupyter/kernels/py5bot/install.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     3239 2022-05-10 13:03:50.000000 py5jupyter-0.1.2a1/py5jupyter/kernels/py5bot/kernel.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     7748 2022-05-10 13:03:50.000000 py5jupyter-0.1.2a1/py5jupyter/kernels/py5bot/py5bot.py
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2022-05-26 01:15:03.125727 py5jupyter-0.1.2a1/py5jupyter/labextension/
--rw-rw-r--   0 jim       (1000) jim       (1000)    20966 2022-05-26 01:14:46.000000 py5jupyter-0.1.2a1/py5jupyter/labextension/build_log.json
--rw-rw-r--   0 jim       (1000) jim       (1000)     2996 2022-05-26 01:14:47.000000 py5jupyter-0.1.2a1/py5jupyter/labextension/package.json
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2022-05-26 01:15:03.126727 py5jupyter-0.1.2a1/py5jupyter/labextension/static/
--rw-rw-r--   0 jim       (1000) jim       (1000)     2083 2022-05-26 01:14:47.000000 py5jupyter-0.1.2a1/py5jupyter/labextension/static/lib_index_js.488a66c2de85320bc65a.js
--rw-rw-r--   0 jim       (1000) jim       (1000)     2153 2022-05-26 01:14:47.000000 py5jupyter-0.1.2a1/py5jupyter/labextension/static/lib_index_js.488a66c2de85320bc65a.js.map
--rw-rw-r--   0 jim       (1000) jim       (1000)     2293 2022-05-26 01:14:47.000000 py5jupyter-0.1.2a1/py5jupyter/labextension/static/lib_plugin_js.586e3941dfcc287e7351.js
--rw-rw-r--   0 jim       (1000) jim       (1000)     2431 2022-05-26 01:14:47.000000 py5jupyter-0.1.2a1/py5jupyter/labextension/static/lib_plugin_js.586e3941dfcc287e7351.js.map
--rw-rw-r--   0 jim       (1000) jim       (1000)    14328 2022-05-26 01:14:47.000000 py5jupyter-0.1.2a1/py5jupyter/labextension/static/lib_widget_js.d141153e6400998a12a2.js
--rw-rw-r--   0 jim       (1000) jim       (1000)    13199 2022-05-26 01:14:47.000000 py5jupyter-0.1.2a1/py5jupyter/labextension/static/lib_widget_js.d141153e6400998a12a2.js.map
--rw-rw-r--   0 jim       (1000) jim       (1000)    26338 2022-05-26 01:14:47.000000 py5jupyter-0.1.2a1/py5jupyter/labextension/static/remoteEntry.042026d6e03651ecc3fd.js
--rw-rw-r--   0 jim       (1000) jim       (1000)    25133 2022-05-26 01:14:47.000000 py5jupyter-0.1.2a1/py5jupyter/labextension/static/remoteEntry.042026d6e03651ecc3fd.js.map
--rw-rw-r--   0 jim       (1000) jim       (1000)      118 2022-05-26 01:14:46.000000 py5jupyter-0.1.2a1/py5jupyter/labextension/static/style.js
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2022-05-26 01:15:03.126727 py5jupyter-0.1.2a1/py5jupyter/nbextension/
--rw-rw-r--   0 jim       (1000) jim       (1000)      411 2022-05-07 11:17:35.000000 py5jupyter-0.1.2a1/py5jupyter/nbextension/extension.js
--rw-rw-r--   0 jim       (1000) jim       (1000)     7989 2022-05-23 11:15:20.000000 py5jupyter-0.1.2a1/py5jupyter/nbextension/index.js
--rw-rw-r--   0 jim       (1000) jim       (1000)    17061 2022-05-23 11:15:20.000000 py5jupyter-0.1.2a1/py5jupyter/nbextension/index.js.map
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2022-05-26 01:15:03.126727 py5jupyter-0.1.2a1/py5jupyter/tests/
--rw-rw-r--   0 jim       (1000) jim       (1000)        0 2022-05-07 11:17:35.000000 py5jupyter-0.1.2a1/py5jupyter/tests/__init__.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     1409 2022-05-07 11:17:35.000000 py5jupyter-0.1.2a1/py5jupyter/tests/conftest.py
--rw-rw-r--   0 jim       (1000) jim       (1000)      276 2022-05-07 11:17:35.000000 py5jupyter-0.1.2a1/py5jupyter/tests/test_example.py
--rw-rw-r--   0 jim       (1000) jim       (1000)      461 2022-05-07 11:17:35.000000 py5jupyter-0.1.2a1/py5jupyter/tests/test_nbextension_path.py
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2022-05-26 01:15:03.126727 py5jupyter-0.1.2a1/py5jupyter/widgets/
--rw-rw-r--   0 jim       (1000) jim       (1000)      962 2022-05-10 13:03:50.000000 py5jupyter-0.1.2a1/py5jupyter/widgets/__init__.py
--rw-rw-r--   0 jim       (1000) jim       (1000)      974 2022-05-10 13:03:50.000000 py5jupyter-0.1.2a1/py5jupyter/widgets/_frontend.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     5346 2022-05-17 14:45:32.000000 py5jupyter-0.1.2a1/py5jupyter/widgets/sketchportal.py
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2022-05-26 01:15:03.125727 py5jupyter-0.1.2a1/py5jupyter.egg-info/
--rw-rw-r--   0 jim       (1000) jim       (1000)     3101 2022-05-26 01:15:02.000000 py5jupyter-0.1.2a1/py5jupyter.egg-info/PKG-INFO
--rw-rw-r--   0 jim       (1000) jim       (1000)     2559 2022-05-26 01:15:03.000000 py5jupyter-0.1.2a1/py5jupyter.egg-info/SOURCES.txt
--rw-rw-r--   0 jim       (1000) jim       (1000)        1 2022-05-26 01:15:02.000000 py5jupyter-0.1.2a1/py5jupyter.egg-info/dependency_links.txt
--rw-rw-r--   0 jim       (1000) jim       (1000)      196 2022-05-26 01:15:03.000000 py5jupyter-0.1.2a1/py5jupyter.egg-info/requires.txt
--rw-rw-r--   0 jim       (1000) jim       (1000)       11 2022-05-26 01:15:03.000000 py5jupyter-0.1.2a1/py5jupyter.egg-info/top_level.txt
--rw-rw-r--   0 jim       (1000) jim       (1000)       64 2022-05-07 11:17:35.000000 py5jupyter-0.1.2a1/py5jupyter.json
--rw-rw-r--   0 jim       (1000) jim       (1000)      145 2022-05-07 11:17:35.000000 py5jupyter-0.1.2a1/pyproject.toml
--rw-rw-r--   0 jim       (1000) jim       (1000)      127 2022-05-07 11:17:35.000000 py5jupyter-0.1.2a1/pytest.ini
--rw-rw-r--   0 jim       (1000) jim       (1000)      183 2022-05-26 01:15:03.127727 py5jupyter-0.1.2a1/setup.cfg
--rw-rw-r--   0 jim       (1000) jim       (1000)     4142 2022-05-26 01:14:35.000000 py5jupyter-0.1.2a1/setup.py
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2022-05-26 01:15:03.126727 py5jupyter-0.1.2a1/src/
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2022-05-26 01:15:03.126727 py5jupyter-0.1.2a1/src/__tests__/
--rw-rw-r--   0 jim       (1000) jim       (1000)      829 2022-05-07 11:17:35.000000 py5jupyter-0.1.2a1/src/__tests__/index.spec.ts
--rw-rw-r--   0 jim       (1000) jim       (1000)     2856 2022-05-07 11:17:35.000000 py5jupyter-0.1.2a1/src/__tests__/utils.ts
--rw-rw-r--   0 jim       (1000) jim       (1000)     1421 2022-05-10 13:03:50.000000 py5jupyter-0.1.2a1/src/extension.ts
--rw-rw-r--   0 jim       (1000) jim       (1000)      992 2022-05-10 13:03:50.000000 py5jupyter-0.1.2a1/src/index.ts
--rw-rw-r--   0 jim       (1000) jim       (1000)     1967 2022-05-10 13:03:50.000000 py5jupyter-0.1.2a1/src/plugin.ts
--rw-rw-r--   0 jim       (1000) jim       (1000)     1419 2022-05-18 22:08:26.000000 py5jupyter-0.1.2a1/src/utils.ts
--rw-rw-r--   0 jim       (1000) jim       (1000)     1421 2022-05-10 13:03:50.000000 py5jupyter-0.1.2a1/src/version.ts
--rw-rw-r--   0 jim       (1000) jim       (1000)     5754 2022-05-15 10:15:16.000000 py5jupyter-0.1.2a1/src/widget.ts
--rw-rw-r--   0 jim       (1000) jim       (1000)      553 2022-05-07 11:17:35.000000 py5jupyter-0.1.2a1/tsconfig.json
--rw-rw-r--   0 jim       (1000) jim       (1000)     2126 2022-05-07 11:17:35.000000 py5jupyter-0.1.2a1/webpack.config.js
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/.coveragerc
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/.eslintignore
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/.eslintrc.js
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/.npmignore
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/.prettierignore
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/.prettierrc
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/Makefile
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/babel.config.js
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/codecov.yml
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/install.json
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/jest.config.js
+-rw-r--r--   0        0        0   933834 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/package-lock.json
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/package.json
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/py5jupyter.json
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/pytest.ini
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/readthedocs.yml
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/setup.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/tsconfig.eslint.json
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/tsconfig.json
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/webpack.config.js
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/docs/Makefile
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/docs/environment.yml
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/docs/make.bat
+-rw-r--r--   0        0        0     6297 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/docs/source/conf.py
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/docs/source/develop-install.rst
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/docs/source/index.rst
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/docs/source/installing.rst
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/docs/source/introduction.rst
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/docs/source/_static/helper.js
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/docs/source/examples/index.rst
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/docs/source/examples/introduction.nblink
+-rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/examples/Camera3D Example.ipynb
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/examples/PeasyCam Example.ipynb
+-rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/examples/Test.ipynb
+-rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/py5jupyter/__init__.py
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/py5jupyter/_version.py
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/py5jupyter/kernels/__init__.py
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/py5jupyter/kernels/py5/__init__.py
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/py5jupyter/kernels/py5/__main__.py
+-rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/py5jupyter/kernels/py5/install.py
+-rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/py5jupyter/kernels/py5/kernel.py
+-rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/py5jupyter/kernels/py5/resources/logo-32x32.png
+-rw-r--r--   0        0        0     6982 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/py5jupyter/kernels/py5/resources/logo-64x64.png
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/py5jupyter/kernels/py5bot/__init__.py
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/py5jupyter/kernels/py5bot/__main__.py
+-rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/py5jupyter/kernels/py5bot/install.py
+-rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/py5jupyter/kernels/py5bot/kernel.py
+-rw-r--r--   0        0        0     4942 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/py5jupyter/kernels/py5bot/py5bot.py
+-rw-r--r--   0        0        0     2541 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/py5jupyter/kernels/py5bot/resources/logo-32x32.png
+-rw-r--r--   0        0        0     6819 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/py5jupyter/kernels/py5bot/resources/logo-64x64.png
+-rw-r--r--   0        0        0    20991 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/py5jupyter/labextension/build_log.json
+-rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/py5jupyter/labextension/package.json
+-rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/py5jupyter/labextension/static/lib_index_js.b65cf7c58127bf49a498.js
+-rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/py5jupyter/labextension/static/lib_index_js.b65cf7c58127bf49a498.js.map
+-rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/py5jupyter/labextension/static/lib_plugin_js.586e3941dfcc287e7351.js
+-rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/py5jupyter/labextension/static/lib_plugin_js.586e3941dfcc287e7351.js.map
+-rw-r--r--   0        0        0    14343 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/py5jupyter/labextension/static/lib_widget_js.fc065f743fb92e735a68.js
+-rw-r--r--   0        0        0    13214 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/py5jupyter/labextension/static/lib_widget_js.fc065f743fb92e735a68.js.map
+-rw-r--r--   0        0        0    26338 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/py5jupyter/labextension/static/remoteEntry.102c2185a6a3be91ce3c.js
+-rw-r--r--   0        0        0    25133 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/py5jupyter/labextension/static/remoteEntry.102c2185a6a3be91ce3c.js.map
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/py5jupyter/labextension/static/style.js
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/py5jupyter/nbextension/extension.js
+-rw-r--r--   0        0        0     7989 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/py5jupyter/nbextension/index.js
+-rw-r--r--   0        0        0    17185 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/py5jupyter/nbextension/index.js.map
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/py5jupyter/tests/__init__.py
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/py5jupyter/tests/conftest.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/py5jupyter/tests/test_example.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/py5jupyter/tests/test_nbextension_path.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/py5jupyter/widgets/__init__.py
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/py5jupyter/widgets/_frontend.py
+-rw-r--r--   0        0        0     5351 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/py5jupyter/widgets/sketchportal.py
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/src/extension.ts
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/src/index.ts
+-rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/src/plugin.ts
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/src/utils.ts
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/src/version.ts
+-rw-r--r--   0        0        0     5759 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/src/widget.ts
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/src/__tests__/index.spec.ts
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/src/__tests__/utils.ts
+-rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/.gitignore
+-rw-r--r--   0        0        0    24436 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/LICENSE
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/README.md
+-rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/pyproject.toml
+-rw-r--r--   0        0        0    32046 2020-02-02 00:00:00.000000 py5jupyter-0.2.0a0/PKG-INFO
```

### Comparing `py5jupyter-0.1.2a1/LICENSE` & `py5jupyter-0.2.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `py5jupyter-0.1.2a1/README.md` & `py5jupyter-0.2.0a0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # py5jupyter (& py5)
 
-![py5 logo](https://py5.ixora.io/_static/logo.png)
+![py5 logo](https://py5coding.org/_static/logo.png)
 
 [![py5jupyter monthly downloads](https://pepy.tech/badge/py5jupyter/month)](https://pepy.tech/project/py5jupyter)
 
 [![py5jupyter weekly downloads](https://pepy.tech/badge/py5jupyter/week)](https://pepy.tech/project/py5jupyter)
 
 py5 is a new version of [**Processing**][processing] for Python 3.8+. It makes the Java [**Processing**][processing] jars available to the CPython interpreter using [**JPype**][jpype]. It can do just about everything [**Processing**][processing] can do, except with Python instead of Java code.
 
-The goal of py5 is to create a new version of Processing that is integrated into the Python ecosystem. Built into the library are thoughtful choices about how to best get py5 to work with other popular Python libraries such as [numpy](https://www.numpy.org/) or [Pillow](https://python-pillow.org/).
+The goal of py5 is to create a new version of Processing that is integrated into the Python ecosystem. Built into the library are thoughtful choices about how to best get py5 to work with other popular Python libraries and tools such as [Jupyter][jupyter], [numpy][numpy], and [Pillow][pillow].
 
 The py5jupyter library provides Jupyter-related functionality for py5. This includes the Jupyter kernels and Jupyter widgets.
 
 For more in-depth information about py5, see the [py5generator][py5_generator_repo] github repo.
 
 ## Installation
 
@@ -30,13 +30,18 @@
 ```
 
 ## Get In Touch
 
 Have a comment or question? We'd love to hear from you! The best ways to reach out are:
 
 * github [discussions](https://github.com/py5coding/py5generator/discussions) and [issues](https://github.com/py5coding/py5generator/issues)
+* Mastodon <a rel="me" href="https://fosstodon.org/@py5coding">fosstodon.org/@py5coding</a>
 * twitter [@py5coding](https://twitter.com/py5coding)
 * [processing foundation discourse](https://discourse.processing.org/)
 
 [py5_generator_repo]: https://github.com/py5coding/py5generator
 [processing]: https://github.com/processing/processing4
 [jpype]: https://github.com/jpype-project/jpype
+
+[jupyter]: https://jupyter.org/
+[numpy]: https://numpy.org/
+[pillow]: https://python-pillow.org/
```

### Comparing `py5jupyter-0.1.2a1/docs/Makefile` & `py5jupyter-0.2.0a0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `py5jupyter-0.1.2a1/docs/make.bat` & `py5jupyter-0.2.0a0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `py5jupyter-0.1.2a1/docs/source/_static/embed-bundle.js` & `py5jupyter-0.2.0a0/py5jupyter/nbextension/index.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,28 @@
-define("jupyter-py5", ["@jupyter-widgets/base"], (e => (() => {
+define(["@jupyter-widgets/base"], (e => (() => {
     "use strict";
     var t = {
+            112: function(e, t, n) {
+                var i = this && this.__createBinding || (Object.create ? function(e, t, n, i) {
+                        void 0 === i && (i = n), Object.defineProperty(e, i, {
+                            enumerable: !0,
+                            get: function() {
+                                return t[n]
+                            }
+                        })
+                    } : function(e, t, n, i) {
+                        void 0 === i && (i = n), e[i] = t[n]
+                    }),
+                    s = this && this.__exportStar || function(e, t) {
+                        for (var n in e) "default" === n || Object.prototype.hasOwnProperty.call(t, n) || i(t, e, n)
+                    };
+                Object.defineProperty(t, "__esModule", {
+                    value: !0
+                }), window.__webpack_public_path__ = document.querySelector("body").getAttribute("data-base-url") + "nbextensions/py5jupyter", s(n(607), t)
+            },
             607: function(e, t, n) {
                 var i = this && this.__createBinding || (Object.create ? function(e, t, n, i) {
                         void 0 === i && (i = n), Object.defineProperty(e, i, {
                             enumerable: !0,
                             get: function() {
                                 return t[n]
                             }
@@ -211,10 +229,10 @@
     return function e(i) {
         var s = n[i];
         if (void 0 !== s) return s.exports;
         var o = n[i] = {
             exports: {}
         };
         return t[i].call(o.exports, o, o.exports, e), o.exports
-    }(607)
+    }(112)
 })()));
-//# sourceMappingURL=embed-bundle.js.map
+//# sourceMappingURL=index.js.map
```

### Comparing `py5jupyter-0.1.2a1/docs/source/_static/embed-bundle.js.map` & `py5jupyter-0.2.0a0/py5jupyter/nbextension/index.js.map`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7838064713064713%*

 * *Differences: {"'file'": "'index.js'",*

 * * "'mappings'": "'6cAyBCA,OAAeC,wBACdC,SAASC,cAAc,QAASC,aAAa,iBAC7C,0BAEF,W,gZCVA,YACA,W,4ZCGA,yBAAoCC,G,yCAChC,IAAIC,EAEJ,MAAMC,EAAO,IAAIC,KAAK,CAACH,GAAS,CAAEI,KAAM,eACxCH,EAAMI,IAAIC,gBAAgBJ,GAE1B,MAAMK,EAAM,IAAIC,MAChB,OAAO,IAAIC,SAAQC,IACfH,EAAII,OAAS,KACTD,EAAQH,EAAI,EAEhBA,EAAIK,IAAMX,CAAG,GAErB,G,wGCbA,MAAMY,EAAO,EAAQ,KAQR,EAAAC,eAAiBD,EAAKE,QAKtB,EAAAC,YAAcH,EAAKI,I,2bCjBhC,eAKA,SAEA,SAMA,MAAaC,UAA6B,EAAAC,eACxCC,WACE,OAAO,OAAP,wBACKC,MAAMD,YAAU,CACnBE,YAAaJ,EAAqBK,WAClCC,cA […]*

```diff
@@ -1,11 +1,16 @@
 {
-    "file": "embed-bundle.js",
-    "mappings": "2dAmBA,YACA,a,0ZCGA,yBAAoCA,G,yCAChC,IAAIC,EAEJ,MAAMC,EAAO,IAAIC,KAAK,CAACH,GAAS,CAAEI,KAAM,eACxCH,EAAMI,IAAIC,gBAAgBJ,GAE1B,MAAMK,EAAM,IAAIC,MAChB,OAAO,IAAIC,SAAQC,IACfH,EAAII,OAAS,KACTD,EAAQH,IAEZA,EAAIK,IAAMX,U,qGCXlB,MAAMY,EAAO,EAAQ,KAQR,EAAAC,eAAiBD,EAAKE,QAKtB,EAAAC,YAAcH,EAAKI,M,ybCjBhC,eAKA,SAEA,SAMA,MAAaC,UAA6B,EAAAC,eACxCC,WACE,OAAO,OAAP,wBACKC,MAAMD,YAAU,CACnBE,YAAaJ,EAAqBK,WAClCC,cAAeN,EAAqBO,aACpCC,sBAAuBR,EAAqBS,qBAC5CC,WAAYV,EAAqBW,UACjCC,aAAcZ,EAAqBa,YACnCC,qBAAsBd,EAAqBe,oBAC3CC,MAAO,GACPC,OAAQ,GACRC,MAAO,IAAIC,SAAS,IAAIC,YAAY,OAZ1C,yBAgBS,EAAAC,YAAc,OAAH,wBACb,EAAApB,eAAeoB,aAAW,CAC7BH,MAAO,CACLI,UAAYJ,GACH,IAAIC,SAASD,EAAMpC,OAAOyC,MAAM,OAKtC,EAAAlB,WAAa,uBACb,EAAAE,aAAe,EAAAT,YACf,EAAAW,qBAAuB,EAAAb,eACvB,EAAAe,UAAY,sBACZ,EAAAE,YAAc,EAAAf,YACd,EAAAiB,oBAAsB,EAAAnB,eAG/B,MAAa4B,UAA4B,EAAAC,cAIvCC,SACEC,KAAKC,QAAUC,SAASC,cAAc,UACtCH,KAAKC,QAAQZ,MAAQW,KAAKI,MAAMC,IAAI,SACpCL,KAAKC,QAAQX,OAASU,KAAKI,MAAMC,IAAI,UACrCL,KAAKC,QAAQK,SAAW,EAExB,MAAMC,EAAMP,KAAKC,QAAQO,WAAW,MACpC,GAAY,OAARD,EACF,KAAM,+BAENP,KAAKS,KAAOF,EAGdP,KAAKU,gBACLV,KAAKW,GAAGC,YAAYZ,KAAKC,SAEzBD,KAAKC,QAAQY,iBAAiB,UAAW,CACvCC,YAAad,KAAKe,WAAWC,KAAKhB,KAAM,cAE1CA,KAAKC,QAAQY,iBAAiB,WAAY,CACxCC,YAAad,KAAKe,WAAWC,KAAKhB,KAAM,eAE1CA,KAAKC,QAAQY,iBAAiB,QAAS,CACrCC,YAAad,KAAKe,WAAWC,KAAKhB,KAAM,YAE1CA,KAAKC,QAAQY,iBAAiB,aAAc,CAC1CC,YAAad,KAAKiB,aAAaD,KAAKhB,KAAM,iBAE5CA,KAAKC,QAAQY,iBAAiB,YAAa,CACzCC,YAAad,KAAKkB,YAAYF,KAAKhB,QAErCA,KAAKC,QAAQY,iBAAiB,YAAa,CACzCC,YAAad,KAAKiB,aAAaD,KAAKhB,KAAM,gBAE5CA,KAAKC,QAAQY,iBAAiB,UAAW,CACvCC,YAAad,KAAKiB,aAAaD,KAAKhB,KAAM,cAE5CA,KAAKC,QAAQY,iBAAiB,aAAc,CAC1CC,YAAad,KAAKiB,aAAaD,KAAKhB,KAAM,iBAE5CA,KAAKC,QAAQY,iBAAiB,QAAS,CACrCC,YAAad,KAAKiB,aAAaD,KAAKhB,KAAM,iBAE5CA,KAAKC,QAAQY,iBAAiB,QAAS,CACrCC,YAAad,KAAKmB,aAAaH,KAAKhB,QAItCA,KAAKI,MAAMgB,GAAG,eAAgBpB,KAAKU,cAAeV,MAGtCU,gB,yCACZ,MAAMhD,QAAY,EAAA2D,cAAcrB,KAAKI,MAAMC,IAAI,UAC/CL,KAAKS,KAAKa,UAAU5D,EAAK,EAAG,MAKtBqD,WAAWQ,EAAoBC,GACrCxB,KAAKI,MAAMqB,KAAK,OAAD,QAAGD,MAAOD,EAAYG,IAAKF,EAAME,IAAKC,OAAQH,EAAMG,QAAW3B,KAAK4B,aAAaJ,IAAU,IAGpGP,aAAaM,EAAoBC,GACvCxB,KAAKI,MAAMqB,KAAK,OAAD,sBAAGD,MAAOD,EAAYM,QAASL,EAAMK,SAAY7B,KAAK4B,aAAaJ,IAAWxB,KAAK8B,eAAeN,IAAU,IAGrHN,YAAYM,GAElBxB,KAAKC,QAAQ8B,QAEb/B,KAAKI,MAAMqB,KAAK,OAAD,sBAAGD,MAAO,aAAcK,QAASL,EAAMK,SAAY7B,KAAK4B,aAAaJ,IAAWxB,KAAK8B,eAAeN,IAAU,IAKvHL,aAAaK,GACnBxB,KAAKI,MAAMqB,KAAK,OAAD,sBAAGD,MAAO,cAAeK,QAASL,EAAMK,QAASG,MAAyB,GAAhBR,EAAMS,OAAeT,EAAMS,OAAST,EAAMU,QAAYlC,KAAK4B,aAAaJ,IAAWxB,KAAK8B,eAAeN,IAAU,IAGlLM,eAAeN,GAEvB,MAAMW,EAAOnC,KAAKC,QAAQmC,wBAK1B,MAAO,CAAEC,EAHErC,KAAKC,QAAQZ,OAASmC,EAAMc,QAAUH,EAAKI,MAASJ,EAAK9C,MAGxDmD,EAFDxC,KAAKC,QAAQX,QAAUkC,EAAMiB,QAAUN,EAAKO,KAAQP,EAAK7C,QAK5DsC,aAAaJ,GACrB,MAAO,CAAEmB,IAAyB,GAAlBnB,EAAMoB,SAAmC,GAAjBpB,EAAMqB,QAAkC,GAAjBrB,EAAMsB,QAAiC,GAAhBtB,EAAMuB,SA9FhG,yB,QCjEAC,EAAOC,QAAUC,G,i3ECCbC,EAA2B,G,OAG/B,SAASC,EAAoBC,GAE5B,IAAIC,EAAeH,EAAyBE,GAC5C,QAAqBE,IAAjBD,EACH,OAAOA,EAAaL,QAGrB,IAAID,EAASG,EAAyBE,GAAY,CAGjDJ,QAAS,IAOV,OAHAO,EAAoBH,GAAUI,KAAKT,EAAOC,QAASD,EAAQA,EAAOC,QAASG,GAGpEJ,EAAOC,QClBWG,CAAoB,M",
+    "file": "index.js",
+    "mappings": "6cAyBCA,OAAeC,wBACdC,SAASC,cAAc,QAASC,aAAa,iBAC7C,0BAEF,W,gZCVA,YACA,W,4ZCGA,yBAAoCC,G,yCAChC,IAAIC,EAEJ,MAAMC,EAAO,IAAIC,KAAK,CAACH,GAAS,CAAEI,KAAM,eACxCH,EAAMI,IAAIC,gBAAgBJ,GAE1B,MAAMK,EAAM,IAAIC,MAChB,OAAO,IAAIC,SAAQC,IACfH,EAAII,OAAS,KACTD,EAAQH,EAAI,EAEhBA,EAAIK,IAAMX,CAAG,GAErB,G,wGCbA,MAAMY,EAAO,EAAQ,KAQR,EAAAC,eAAiBD,EAAKE,QAKtB,EAAAC,YAAcH,EAAKI,I,2bCjBhC,eAKA,SAEA,SAMA,MAAaC,UAA6B,EAAAC,eACxCC,WACE,OAAO,OAAP,wBACKC,MAAMD,YAAU,CACnBE,YAAaJ,EAAqBK,WAClCC,cAAeN,EAAqBO,aACpCC,sBAAuBR,EAAqBS,qBAC5CC,WAAYV,EAAqBW,UACjCC,aAAcZ,EAAqBa,YACnCC,qBAAsBd,EAAqBe,oBAC3CC,MAAO,GACPC,OAAQ,GACRC,MAAO,IAAIC,SAAS,IAAIC,YAAY,KAExC,EAdF,yBAgBS,EAAAC,YAAc,OAAH,wBACb,EAAApB,eAAeoB,aAAW,CAC7BH,MAAO,CACLI,UAAYJ,GACH,IAAIC,SAASD,EAAMpC,OAAOyC,MAAM,OAKtC,EAAAlB,WAAa,uBACb,EAAAE,aAAe,EAAAT,YACf,EAAAW,qBAAuB,EAAAb,eACvB,EAAAe,UAAY,sBACZ,EAAAE,YAAc,EAAAf,YACd,EAAAiB,oBAAsB,EAAAnB,eAG/B,MAAa4B,UAA4B,EAAAC,cAIvCC,SACEC,KAAKC,QAAUjD,SAASkD,cAAc,UACtCF,KAAKC,QAAQZ,MAAQW,KAAKG,MAAMC,IAAI,SACpCJ,KAAKC,QAAQX,OAASU,KAAKG,MAAMC,IAAI,UACrCJ,KAAKC,QAAQI,SAAW,EAExB,MAAMC,EAAMN,KAAKC,QAAQM,WAAW,MACpC,GAAY,OAARD,EACF,KAAM,+BAENN,KAAKQ,KAAOF,EAGdN,KAAKS,gBACLT,KAAKU,GAAGC,YAAYX,KAAKC,SAEzBD,KAAKC,QAAQW,iBAAiB,UAAW,CACvCC,YAAab,KAAKc,WAAWC,KAAKf,KAAM,cAE1CA,KAAKC,QAAQW,iBAAiB,WAAY,CACxCC,YAAab,KAAKc,WAAWC,KAAKf,KAAM,eAE1CA,KAAKC,QAAQW,iBAAiB,QAAS,CACrCC,YAAab,KAAKc,WAAWC,KAAKf,KAAM,YAE1CA,KAAKC,QAAQW,iBAAiB,aAAc,CAC1CC,YAAab,KAAKgB,aAAaD,KAAKf,KAAM,iBAE5CA,KAAKC,QAAQW,iBAAiB,YAAa,CACzCC,YAAab,KAAKiB,YAAYF,KAAKf,QAErCA,KAAKC,QAAQW,iBAAiB,YAAa,CACzCC,YAAab,KAAKgB,aAAaD,KAAKf,KAAM,gBAE5CA,KAAKC,QAAQW,iBAAiB,UAAW,CACvCC,YAAab,KAAKgB,aAAaD,KAAKf,KAAM,cAE5CA,KAAKC,QAAQW,iBAAiB,aAAc,CAC1CC,YAAab,KAAKgB,aAAaD,KAAKf,KAAM,iBAE5CA,KAAKC,QAAQW,iBAAiB,QAAS,CACrCC,YAAab,KAAKgB,aAAaD,KAAKf,KAAM,iBAE5CA,KAAKC,QAAQW,iBAAiB,QAAS,CACrCC,YAAab,KAAKkB,aAAaH,KAAKf,QAItCA,KAAKG,MAAMgB,GAAG,eAAgBnB,KAAKS,cAAeT,KACpD,CAEcS,gB,yCACZ,MAAM/C,QAAY,EAAA0D,cAAcpB,KAAKG,MAAMC,IAAI,UAC/CJ,KAAKQ,KAAKa,UAAU3D,EAAK,EAAG,EAC9B,G,CAIQoD,WAAWQ,EAAoBC,GACrCvB,KAAKG,MAAMqB,KAAK,OAAD,QAAGD,MAAOD,EAAYG,IAAKF,EAAME,IAAKC,OAAQH,EAAMG,QAAW1B,KAAK2B,aAAaJ,IAAU,CAAC,EAC7G,CAEQP,aAAaM,EAAoBC,GACvCvB,KAAKG,MAAMqB,KAAK,OAAD,sBAAGD,MAAOD,EAAYM,QAASL,EAAMK,SAAY5B,KAAK2B,aAAaJ,IAAWvB,KAAK6B,eAAeN,IAAU,CAAC,EAC9H,CAEQN,YAAYM,GAElBvB,KAAKC,QAAQ6B,QAEb9B,KAAKG,MAAMqB,KAAK,OAAD,sBAAGD,MAAO,aAAcK,QAASL,EAAMK,SAAY5B,KAAK2B,aAAaJ,IAAWvB,KAAK6B,eAAeN,IAAU,CAAC,EAChI,CAIQL,aAAaK,GACnBvB,KAAKG,MAAMqB,KAAK,OAAD,sBAAGD,MAAO,cAAeK,QAASL,EAAMK,QAASG,MAAyB,GAAhBR,EAAMS,OAAeT,EAAMS,OAAST,EAAMU,QAAYjC,KAAK2B,aAAaJ,IAAWvB,KAAK6B,eAAeN,IAAU,CAAC,EAC7L,CAEUM,eAAeN,GAEvB,MAAMW,EAAOlC,KAAKC,QAAQkC,wBAK1B,MAAO,CAAEC,EAHEpC,KAAKC,QAAQZ,OAASkC,EAAMc,QAAUH,EAAKI,MAASJ,EAAK7C,MAGxDkD,EAFDvC,KAAKC,QAAQX,QAAUiC,EAAMiB,QAAUN,EAAKO,KAAQP,EAAK5C,OAGtE,CAEUqC,aAAaJ,GACrB,MAAO,CAAEmB,IAAyB,GAAlBnB,EAAMoB,SAAmC,GAAjBpB,EAAMqB,QAAkC,GAAjBrB,EAAMsB,QAAiC,GAAhBtB,EAAMuB,OAC9F,EA/FF,uB,UCjEAC,EAAOC,QAAUC,C,m3ECCbC,EAA2B,CAAC,E,OAGhC,SAASC,EAAoBC,GAE5B,IAAIC,EAAeH,EAAyBE,GAC5C,QAAqBE,IAAjBD,EACH,OAAOA,EAAaL,QAGrB,IAAID,EAASG,EAAyBE,GAAY,CAGjDJ,QAAS,CAAC,GAOX,OAHAO,EAAoBH,GAAUI,KAAKT,EAAOC,QAASD,EAAQA,EAAOC,QAASG,GAGpEJ,EAAOC,OACf,CCnB0BG,CAAoB,I",
     "names": [
+        "window",
+        "__webpack_public_path__",
+        "document",
+        "querySelector",
+        "getAttribute",
         "buffer",
         "url",
         "blob",
         "Blob",
         "type",
         "URL",
         "createObjectURL",
@@ -45,15 +50,14 @@
         "serialize",
         "slice",
         "Py5SketchPortalView",
         "DOMWidgetView",
         "render",
         "this",
         "_canvas",
-        "document",
         "createElement",
         "model",
         "get",
         "tabIndex",
         "ctx",
         "getContext",
         "_ctx",
@@ -104,26 +108,28 @@
         "cachedModule",
         "undefined",
         "__webpack_modules__",
         "call"
     ],
     "sourceRoot": "",
     "sources": [
+        "webpack://jupyter-py5/./src/extension.ts",
         "webpack://jupyter-py5/./src/index.ts",
         "webpack://jupyter-py5/./src/utils.ts",
         "webpack://jupyter-py5/./src/version.ts",
         "webpack://jupyter-py5/./src/widget.ts",
         "webpack://jupyter-py5/external amd \"@jupyter-widgets/base\"",
         "webpack://jupyter-py5/webpack/bootstrap",
         "webpack://jupyter-py5/webpack/startup"
     ],
     "sourcesContent": [
-        "// *****************************************************************************\n//\n//   Part of the py5jupyter (& py5) library\n//   Copyright (C) 2022 Jim Schmitz\n//\n//   This library is free software: you can redistribute it and/or modify it\n//   under the terms of the GNU Lesser General Public License as published by\n//   the Free Software Foundation, either version 2.1 of the License, or (at\n//   your option) any later version.\n//\n//   This library is distributed in the hope that it will be useful, but\n//   WITHOUT ANY WARRANTY; without even the implied warranty of\n//   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser\n//   General Public License for more details.\n//\n//   You should have received a copy of the GNU Lesser General Public License\n//   along with this library. If not, see <https://www.gnu.org/licenses/>.\n//\n// *****************************************************************************\nexport * from './version';\nexport * from './widget';\n",
-        "// *****************************************************************************\n//\n//   Part of the py5jupyter (& py5) library\n//   Copyright (C) 2022 Jim Schmitz\n//\n//   This library is free software: you can redistribute it and/or modify it\n//   under the terms of the GNU Lesser General Public License as published by\n//   the Free Software Foundation, either version 2.1 of the License, or (at\n//   your option) any later version.\n//\n//   This library is distributed in the hope that it will be useful, but\n//   WITHOUT ANY WARRANTY; without even the implied warranty of\n//   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser\n//   General Public License for more details.\n//\n//   You should have received a copy of the GNU Lesser General Public License\n//   along with this library. If not, see <https://www.gnu.org/licenses/>.\n//\n// *****************************************************************************\n\n// The below function came from the wonderful Python library ipycanvas\n// https://github.com/martinRenou/ipycanvas\n\nexport async function bufferToImage(buffer: any): Promise<HTMLImageElement> {\n    let url: string;\n\n    const blob = new Blob([buffer], { type: 'image/jpeg' });\n    url = URL.createObjectURL(blob);\n\n    const img = new Image();\n    return new Promise(resolve => {\n        img.onload = () => {\n            resolve(img);\n        };\n        img.src = url;\n    });\n}\n",
-        "// *****************************************************************************\n//\n//   Part of the py5jupyter (& py5) library\n//   Copyright (C) 2022 Jim Schmitz\n//\n//   This library is free software: you can redistribute it and/or modify it\n//   under the terms of the GNU Lesser General Public License as published by\n//   the Free Software Foundation, either version 2.1 of the License, or (at\n//   your option) any later version.\n//\n//   This library is distributed in the hope that it will be useful, but\n//   WITHOUT ANY WARRANTY; without even the implied warranty of\n//   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser\n//   General Public License for more details.\n//\n//   You should have received a copy of the GNU Lesser General Public License\n//   along with this library. If not, see <https://www.gnu.org/licenses/>.\n//\n// *****************************************************************************\n\n// eslint-disable-next-line @typescript-eslint/ban-ts-comment\n// @ts-ignore\n// eslint-disable-next-line @typescript-eslint/no-var-requires\nconst data = require('../package.json');\n\n/**\n * The _model_module_version/_view_module_version this package implements.\n *\n * The html widget manager assumes that this is the same as the npm package\n * version number.\n */\nexport const MODULE_VERSION = data.version;\n\n/*\n * The current package name.\n */\nexport const MODULE_NAME = data.name;\n",
-        "// *****************************************************************************\n//\n//   Part of the py5jupyter (& py5) library\n//   Copyright (C) 2022 Jim Schmitz\n//\n//   This library is free software: you can redistribute it and/or modify it\n//   under the terms of the GNU Lesser General Public License as published by\n//   the Free Software Foundation, either version 2.1 of the License, or (at\n//   your option) any later version.\n//\n//   This library is distributed in the hope that it will be useful, but\n//   WITHOUT ANY WARRANTY; without even the implied warranty of\n//   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser\n//   General Public License for more details.\n//\n//   You should have received a copy of the GNU Lesser General Public License\n//   along with this library. If not, see <https://www.gnu.org/licenses/>.\n//\n// *****************************************************************************\nimport {\n  DOMWidgetModel,\n  DOMWidgetView,\n} from '@jupyter-widgets/base';\n\nimport { MODULE_NAME, MODULE_VERSION } from './version';\n\nimport {\n  bufferToImage\n} from './utils';\n\n// https://ipywidgets.readthedocs.io/en/latest/examples/Widget%20Low%20Level.html\n\nexport class Py5SketchPortalModel extends DOMWidgetModel {\n  defaults() {\n    return {\n      ...super.defaults(),\n      _model_name: Py5SketchPortalModel.model_name,\n      _model_module: Py5SketchPortalModel.model_module,\n      _model_module_version: Py5SketchPortalModel.model_module_version,\n      _view_name: Py5SketchPortalModel.view_name,\n      _view_module: Py5SketchPortalModel.view_module,\n      _view_module_version: Py5SketchPortalModel.view_module_version,\n      width: '',\n      height: '',\n      value: new DataView(new ArrayBuffer(0)),\n    };\n  }\n\n  static serializers = {\n    ...DOMWidgetModel.serializers,\n    value: {\n      serialize: (value: any): DataView => {\n        return new DataView(value.buffer.slice(0));\n      },\n    },\n  };\n\n  static model_name = 'Py5SketchPortalModel';\n  static model_module = MODULE_NAME;\n  static model_module_version = MODULE_VERSION;\n  static view_name = 'Py5SketchPortalView';\n  static view_module = MODULE_NAME;\n  static view_module_version = MODULE_VERSION;\n}\n\nexport class Py5SketchPortalView extends DOMWidgetView {\n  private _canvas: HTMLCanvasElement;\n  private _ctx: CanvasRenderingContext2D;\n\n  render() {\n    this._canvas = document.createElement('canvas');\n    this._canvas.width = this.model.get('width');\n    this._canvas.height = this.model.get('height');\n    this._canvas.tabIndex = 0;\n\n    const ctx = this._canvas.getContext('2d');\n    if (ctx === null) {\n      throw 'Could not create 2d context.';\n    } else {\n      this._ctx = ctx;\n    }\n\n    this._updateImgSrc();\n    this.el.appendChild(this._canvas);\n\n    this._canvas.addEventListener('keydown', {\n      handleEvent: this.onKeyEvent.bind(this, 'key_down')\n    });\n    this._canvas.addEventListener('keypress', {\n      handleEvent: this.onKeyEvent.bind(this, 'key_press')\n    });\n    this._canvas.addEventListener('keyup', {\n      handleEvent: this.onKeyEvent.bind(this, 'key_up')\n    });\n    this._canvas.addEventListener('mouseenter', {\n      handleEvent: this.onMouseEvent.bind(this, 'mouse_enter')\n    });\n    this._canvas.addEventListener('mousedown', {\n      handleEvent: this.onMouseDown.bind(this)\n    });\n    this._canvas.addEventListener('mousemove', {\n      handleEvent: this.onMouseEvent.bind(this, 'mouse_move')\n    });\n    this._canvas.addEventListener('mouseup', {\n      handleEvent: this.onMouseEvent.bind(this, 'mouse_up')\n    });\n    this._canvas.addEventListener('mouseleave', {\n      handleEvent: this.onMouseEvent.bind(this, 'mouse_leave')\n    });\n    this._canvas.addEventListener('click', {\n      handleEvent: this.onMouseEvent.bind(this, 'mouse_click')\n    });\n    this._canvas.addEventListener('wheel', {\n      handleEvent: this.onMouseWheel.bind(this)\n    });\n\n    // Python -> JavaScript update\n    this.model.on('change:value', this._updateImgSrc, this);\n  }\n\n  private async _updateImgSrc() {\n    const img = await bufferToImage(this.model.get('value'));\n    this._ctx.drawImage(img, 0, 0);\n  }\n\n  // https://developer.mozilla.org/en-US/docs/Web/API/KeyboardEvent\n\n  private onKeyEvent(event_name: string, event: KeyboardEvent) {\n    this.model.send({ event: event_name, key: event.key, repeat: event.repeat, ...this.getModifiers(event) }, {});\n  }\n\n  private onMouseEvent(event_name: string, event: MouseEvent) {\n    this.model.send({ event: event_name, buttons: event.buttons, ...this.getModifiers(event), ...this.getCoordinates(event) }, {});\n  }\n\n  private onMouseDown(event: MouseEvent) {\n    // Bring focus to the img element, so keyboard events can be triggered\n    this._canvas.focus();\n\n    this.model.send({ event: 'mouse_down', buttons: event.buttons, ...this.getModifiers(event), ...this.getCoordinates(event) }, {});\n  }\n\n  // https://developer.mozilla.org/en-US/docs/Web/API/GlobalEventHandlers\n\n  private onMouseWheel(event: WheelEvent) {\n    this.model.send({ event: 'mouse_wheel', buttons: event.buttons, wheel: ((event.deltaY != 0) ? event.deltaY : event.deltaX), ...this.getModifiers(event), ...this.getCoordinates(event) }, {});\n  }\n\n  protected getCoordinates(event: MouseEvent | Touch) {\n    // https://developer.mozilla.org/en-US/docs/Web/API/MouseEvent\n    const rect = this._canvas.getBoundingClientRect();\n\n    const x = (this._canvas.width * (event.clientX - rect.left)) / rect.width;\n    const y = (this._canvas.height * (event.clientY - rect.top)) / rect.height;\n\n    return { x, y };\n  }\n\n  protected getModifiers(event: MouseEvent | KeyboardEvent) {\n    return { mod: (+event.shiftKey) * 1 + (+event.ctrlKey) * 2 + (+event.metaKey) * 4 + (+event.altKey) * 8 };\n  }\n\n}\n",
+        "// *****************************************************************************\n//\n//   Part of the py5jupyter (& py5) library\n//   Copyright (C) 2022-2023 Jim Schmitz\n//\n//   This library is free software: you can redistribute it and/or modify it\n//   under the terms of the GNU Lesser General Public License as published by\n//   the Free Software Foundation, either version 2.1 of the License, or (at\n//   your option) any later version.\n//\n//   This library is distributed in the hope that it will be useful, but\n//   WITHOUT ANY WARRANTY; without even the implied warranty of\n//   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser\n//   General Public License for more details.\n//\n//   You should have received a copy of the GNU Lesser General Public License\n//   along with this library. If not, see <https://www.gnu.org/licenses/>.\n//\n// *****************************************************************************\n// Entry point for the notebook bundle containing custom model definitions.\n\n// Some static assets may be required by the custom widget javascript. The base\n// url for the notebook is not known at build time and is therefore computed\n// dynamically.\n// eslint-disable-next-line @typescript-eslint/no-non-null-assertion\n(window as any).__webpack_public_path__ =\n  document.querySelector('body')!.getAttribute('data-base-url') +\n  'nbextensions/py5jupyter';\n\nexport * from './index';\n",
+        "// *****************************************************************************\n//\n//   Part of the py5jupyter (& py5) library\n//   Copyright (C) 2022-2023 Jim Schmitz\n//\n//   This library is free software: you can redistribute it and/or modify it\n//   under the terms of the GNU Lesser General Public License as published by\n//   the Free Software Foundation, either version 2.1 of the License, or (at\n//   your option) any later version.\n//\n//   This library is distributed in the hope that it will be useful, but\n//   WITHOUT ANY WARRANTY; without even the implied warranty of\n//   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser\n//   General Public License for more details.\n//\n//   You should have received a copy of the GNU Lesser General Public License\n//   along with this library. If not, see <https://www.gnu.org/licenses/>.\n//\n// *****************************************************************************\nexport * from './version';\nexport * from './widget';\n",
+        "// *****************************************************************************\n//\n//   Part of the py5jupyter (& py5) library\n//   Copyright (C) 2022-2023 Jim Schmitz\n//\n//   This library is free software: you can redistribute it and/or modify it\n//   under the terms of the GNU Lesser General Public License as published by\n//   the Free Software Foundation, either version 2.1 of the License, or (at\n//   your option) any later version.\n//\n//   This library is distributed in the hope that it will be useful, but\n//   WITHOUT ANY WARRANTY; without even the implied warranty of\n//   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser\n//   General Public License for more details.\n//\n//   You should have received a copy of the GNU Lesser General Public License\n//   along with this library. If not, see <https://www.gnu.org/licenses/>.\n//\n// *****************************************************************************\n\n// The below function came from the wonderful Python library ipycanvas\n// https://github.com/martinRenou/ipycanvas\n\nexport async function bufferToImage(buffer: any): Promise<HTMLImageElement> {\n    let url: string;\n\n    const blob = new Blob([buffer], { type: 'image/jpeg' });\n    url = URL.createObjectURL(blob);\n\n    const img = new Image();\n    return new Promise(resolve => {\n        img.onload = () => {\n            resolve(img);\n        };\n        img.src = url;\n    });\n}\n",
+        "// *****************************************************************************\n//\n//   Part of the py5jupyter (& py5) library\n//   Copyright (C) 2022-2023 Jim Schmitz\n//\n//   This library is free software: you can redistribute it and/or modify it\n//   under the terms of the GNU Lesser General Public License as published by\n//   the Free Software Foundation, either version 2.1 of the License, or (at\n//   your option) any later version.\n//\n//   This library is distributed in the hope that it will be useful, but\n//   WITHOUT ANY WARRANTY; without even the implied warranty of\n//   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser\n//   General Public License for more details.\n//\n//   You should have received a copy of the GNU Lesser General Public License\n//   along with this library. If not, see <https://www.gnu.org/licenses/>.\n//\n// *****************************************************************************\n\n// eslint-disable-next-line @typescript-eslint/ban-ts-comment\n// @ts-ignore\n// eslint-disable-next-line @typescript-eslint/no-var-requires\nconst data = require('../package.json');\n\n/**\n * The _model_module_version/_view_module_version this package implements.\n *\n * The html widget manager assumes that this is the same as the npm package\n * version number.\n */\nexport const MODULE_VERSION = data.version;\n\n/*\n * The current package name.\n */\nexport const MODULE_NAME = data.name;\n",
+        "// *****************************************************************************\n//\n//   Part of the py5jupyter (& py5) library\n//   Copyright (C) 2022-2023 Jim Schmitz\n//\n//   This library is free software: you can redistribute it and/or modify it\n//   under the terms of the GNU Lesser General Public License as published by\n//   the Free Software Foundation, either version 2.1 of the License, or (at\n//   your option) any later version.\n//\n//   This library is distributed in the hope that it will be useful, but\n//   WITHOUT ANY WARRANTY; without even the implied warranty of\n//   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser\n//   General Public License for more details.\n//\n//   You should have received a copy of the GNU Lesser General Public License\n//   along with this library. If not, see <https://www.gnu.org/licenses/>.\n//\n// *****************************************************************************\nimport {\n  DOMWidgetModel,\n  DOMWidgetView,\n} from '@jupyter-widgets/base';\n\nimport { MODULE_NAME, MODULE_VERSION } from './version';\n\nimport {\n  bufferToImage\n} from './utils';\n\n// https://ipywidgets.readthedocs.io/en/latest/examples/Widget%20Low%20Level.html\n\nexport class Py5SketchPortalModel extends DOMWidgetModel {\n  defaults() {\n    return {\n      ...super.defaults(),\n      _model_name: Py5SketchPortalModel.model_name,\n      _model_module: Py5SketchPortalModel.model_module,\n      _model_module_version: Py5SketchPortalModel.model_module_version,\n      _view_name: Py5SketchPortalModel.view_name,\n      _view_module: Py5SketchPortalModel.view_module,\n      _view_module_version: Py5SketchPortalModel.view_module_version,\n      width: '',\n      height: '',\n      value: new DataView(new ArrayBuffer(0)),\n    };\n  }\n\n  static serializers = {\n    ...DOMWidgetModel.serializers,\n    value: {\n      serialize: (value: any): DataView => {\n        return new DataView(value.buffer.slice(0));\n      },\n    },\n  };\n\n  static model_name = 'Py5SketchPortalModel';\n  static model_module = MODULE_NAME;\n  static model_module_version = MODULE_VERSION;\n  static view_name = 'Py5SketchPortalView';\n  static view_module = MODULE_NAME;\n  static view_module_version = MODULE_VERSION;\n}\n\nexport class Py5SketchPortalView extends DOMWidgetView {\n  private _canvas: HTMLCanvasElement;\n  private _ctx: CanvasRenderingContext2D;\n\n  render() {\n    this._canvas = document.createElement('canvas');\n    this._canvas.width = this.model.get('width');\n    this._canvas.height = this.model.get('height');\n    this._canvas.tabIndex = 0;\n\n    const ctx = this._canvas.getContext('2d');\n    if (ctx === null) {\n      throw 'Could not create 2d context.';\n    } else {\n      this._ctx = ctx;\n    }\n\n    this._updateImgSrc();\n    this.el.appendChild(this._canvas);\n\n    this._canvas.addEventListener('keydown', {\n      handleEvent: this.onKeyEvent.bind(this, 'key_down')\n    });\n    this._canvas.addEventListener('keypress', {\n      handleEvent: this.onKeyEvent.bind(this, 'key_press')\n    });\n    this._canvas.addEventListener('keyup', {\n      handleEvent: this.onKeyEvent.bind(this, 'key_up')\n    });\n    this._canvas.addEventListener('mouseenter', {\n      handleEvent: this.onMouseEvent.bind(this, 'mouse_enter')\n    });\n    this._canvas.addEventListener('mousedown', {\n      handleEvent: this.onMouseDown.bind(this)\n    });\n    this._canvas.addEventListener('mousemove', {\n      handleEvent: this.onMouseEvent.bind(this, 'mouse_move')\n    });\n    this._canvas.addEventListener('mouseup', {\n      handleEvent: this.onMouseEvent.bind(this, 'mouse_up')\n    });\n    this._canvas.addEventListener('mouseleave', {\n      handleEvent: this.onMouseEvent.bind(this, 'mouse_leave')\n    });\n    this._canvas.addEventListener('click', {\n      handleEvent: this.onMouseEvent.bind(this, 'mouse_click')\n    });\n    this._canvas.addEventListener('wheel', {\n      handleEvent: this.onMouseWheel.bind(this)\n    });\n\n    // Python -> JavaScript update\n    this.model.on('change:value', this._updateImgSrc, this);\n  }\n\n  private async _updateImgSrc() {\n    const img = await bufferToImage(this.model.get('value'));\n    this._ctx.drawImage(img, 0, 0);\n  }\n\n  // https://developer.mozilla.org/en-US/docs/Web/API/KeyboardEvent\n\n  private onKeyEvent(event_name: string, event: KeyboardEvent) {\n    this.model.send({ event: event_name, key: event.key, repeat: event.repeat, ...this.getModifiers(event) }, {});\n  }\n\n  private onMouseEvent(event_name: string, event: MouseEvent) {\n    this.model.send({ event: event_name, buttons: event.buttons, ...this.getModifiers(event), ...this.getCoordinates(event) }, {});\n  }\n\n  private onMouseDown(event: MouseEvent) {\n    // Bring focus to the img element, so keyboard events can be triggered\n    this._canvas.focus();\n\n    this.model.send({ event: 'mouse_down', buttons: event.buttons, ...this.getModifiers(event), ...this.getCoordinates(event) }, {});\n  }\n\n  // https://developer.mozilla.org/en-US/docs/Web/API/GlobalEventHandlers\n\n  private onMouseWheel(event: WheelEvent) {\n    this.model.send({ event: 'mouse_wheel', buttons: event.buttons, wheel: ((event.deltaY != 0) ? event.deltaY : event.deltaX), ...this.getModifiers(event), ...this.getCoordinates(event) }, {});\n  }\n\n  protected getCoordinates(event: MouseEvent | Touch) {\n    // https://developer.mozilla.org/en-US/docs/Web/API/MouseEvent\n    const rect = this._canvas.getBoundingClientRect();\n\n    const x = (this._canvas.width * (event.clientX - rect.left)) / rect.width;\n    const y = (this._canvas.height * (event.clientY - rect.top)) / rect.height;\n\n    return { x, y };\n  }\n\n  protected getModifiers(event: MouseEvent | KeyboardEvent) {\n    return { mod: (+event.shiftKey) * 1 + (+event.ctrlKey) * 2 + (+event.metaKey) * 4 + (+event.altKey) * 8 };\n  }\n\n}\n",
         "module.exports = __WEBPACK_EXTERNAL_MODULE__146__;",
         "// The module cache\nvar __webpack_module_cache__ = {};\n\n// The require function\nfunction __webpack_require__(moduleId) {\n\t// Check if module is in cache\n\tvar cachedModule = __webpack_module_cache__[moduleId];\n\tif (cachedModule !== undefined) {\n\t\treturn cachedModule.exports;\n\t}\n\t// Create a new module (and put it into the cache)\n\tvar module = __webpack_module_cache__[moduleId] = {\n\t\t// no module.id needed\n\t\t// no module.loaded needed\n\t\texports: {}\n\t};\n\n\t// Execute the module function\n\t__webpack_modules__[moduleId].call(module.exports, module, module.exports, __webpack_require__);\n\n\t// Return the exports of the module\n\treturn module.exports;\n}\n\n",
-        "// startup\n// Load entry module and return exports\n// This entry module is referenced by other modules so it can't be inlined\nvar __webpack_exports__ = __webpack_require__(607);\n"
+        "// startup\n// Load entry module and return exports\n// This entry module is referenced by other modules so it can't be inlined\nvar __webpack_exports__ = __webpack_require__(112);\n"
     ],
     "version": 3
 }
```

### Comparing `py5jupyter-0.1.2a1/docs/source/conf.py` & `py5jupyter-0.2.0a0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `py5jupyter-0.1.2a1/docs/source/develop-install.rst` & `py5jupyter-0.2.0a0/docs/source/develop-install.rst`

 * *Files identical despite different names*

### Comparing `py5jupyter-0.1.2a1/docs/source/index.rst` & `py5jupyter-0.2.0a0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `py5jupyter-0.1.2a1/docs/source/installing.rst` & `py5jupyter-0.2.0a0/docs/source/installing.rst`

 * *Files identical despite different names*

### Comparing `py5jupyter-0.1.2a1/examples/.ipynb_checkpoints/Camera3D Test-checkpoint.ipynb` & `py5jupyter-0.2.0a0/examples/Camera3D Example.ipynb`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9678819444444444%*

 * *Differences: {"'cells'": "{0: {'source': ['import py5_tools\\n', 'import py5\\n', '\\n', 'from camera3D import "*

 * *            "Camera3D']}, delete: [9, 2, 0]}"}*

```diff
@@ -1,41 +1,19 @@
 {
     "cells": [
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "dabc71e6",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "import time\n",
-                "\n",
-                "import jpype.imports\n",
-                "\n",
-                "import py5_tools\n",
-                "py5_tools.add_jars('/home/jim/Projects/ITP/pythonprocessing/py5projects/jars')"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
             "id": "206aa45c",
             "metadata": {},
             "outputs": [],
             "source": [
-                "import py5"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "e04fc7e0",
-            "metadata": {},
-            "outputs": [],
-            "source": [
+                "import py5_tools\n",
+                "import py5\n",
+                "\n",
                 "from camera3D import Camera3D"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "3170777f",
@@ -118,26 +96,14 @@
             "source": [
                 "py5.run_sketch()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "bacad47d",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "time.sleep(3)\n",
-                "\n",
-                "py5_tools.screenshot(hook_post_draw=True)"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
             "id": "83c2e817",
             "metadata": {},
             "outputs": [],
             "source": [
                 "py5_tools.sketch_portal(hook_post_draw=True)"
             ]
         },
```

### Comparing `py5jupyter-0.1.2a1/examples/.ipynb_checkpoints/Test-checkpoint.ipynb` & `py5jupyter-0.2.0a0/examples/Test.ipynb`

 * *Files identical despite different names*

### Comparing `py5jupyter-0.1.2a1/package.json` & `py5jupyter-0.2.0a0/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'version'": "'0.2.0'"}*

```diff
@@ -86,9 +86,9 @@
         "test": "jest",
         "watch": "npm-run-all -p watch:*",
         "watch:labextension": "jupyter labextension watch .",
         "watch:lib": "tsc -w",
         "watch:nbextension": "webpack --watch --mode=development"
     },
     "types": "./lib/index.d.ts",
-    "version": "0.1.0"
+    "version": "0.2.0"
 }
```

### Comparing `py5jupyter-0.1.2a1/py5jupyter/__init__.py` & `py5jupyter-0.2.0a0/py5jupyter/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # *****************************************************************************
 #
 #   Part of the py5jupyter (& py5) library
-#   Copyright (C) 2022 Jim Schmitz
+#   Copyright (C) 2022-2023 Jim Schmitz
 #
 #   This library is free software: you can redistribute it and/or modify it
 #   under the terms of the GNU Lesser General Public License as published by
 #   the Free Software Foundation, either version 2.1 of the License, or (at
 #   your option) any later version.
 #
 #   This library is distributed in the hope that it will be useful, but
```

### Comparing `py5jupyter-0.1.2a1/py5jupyter/_version.py` & `py5jupyter-0.2.0a0/py5jupyter/kernels/py5/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # *****************************************************************************
 #
 #   Part of the py5jupyter (& py5) library
-#   Copyright (C) 2022 Jim Schmitz
+#   Copyright (C) 2022-2023 Jim Schmitz
 #
 #   This library is free software: you can redistribute it and/or modify it
 #   under the terms of the GNU Lesser General Public License as published by
 #   the Free Software Foundation, either version 2.1 of the License, or (at
 #   your option) any later version.
 #
 #   This library is distributed in the hope that it will be useful, but
@@ -13,9 +13,10 @@
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser
 #   General Public License for more details.
 #
 #   You should have received a copy of the GNU Lesser General Public License
 #   along with this library. If not, see <https://www.gnu.org/licenses/>.
 #
 # *****************************************************************************
-version_info = (0, 1, 2, 'a1')
-__version__ = ".".join(map(str, version_info))
+from .kernel import Py5App
+
+Py5App.launch_instance()
```

### Comparing `py5jupyter-0.1.2a1/py5jupyter/kernels/__init__.py` & `py5jupyter-0.2.0a0/py5jupyter/kernels/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # *****************************************************************************
 #
 #   Part of the py5jupyter (& py5) library
-#   Copyright (C) 2022 Jim Schmitz
+#   Copyright (C) 2022-2023 Jim Schmitz
 #
 #   This library is free software: you can redistribute it and/or modify it
 #   under the terms of the GNU Lesser General Public License as published by
 #   the Free Software Foundation, either version 2.1 of the License, or (at
 #   your option) any later version.
 #
 #   This library is distributed in the hope that it will be useful, but
```

### Comparing `py5jupyter-0.1.2a1/py5jupyter/kernels/py5/__init__.py` & `py5jupyter-0.2.0a0/py5jupyter/kernels/py5/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # *****************************************************************************
 #
 #   Part of the py5jupyter (& py5) library
-#   Copyright (C) 2022 Jim Schmitz
+#   Copyright (C) 2022-2023 Jim Schmitz
 #
 #   This library is free software: you can redistribute it and/or modify it
 #   under the terms of the GNU Lesser General Public License as published by
 #   the Free Software Foundation, either version 2.1 of the License, or (at
 #   your option) any later version.
 #
 #   This library is distributed in the hope that it will be useful, but
```

### Comparing `py5jupyter-0.1.2a1/py5jupyter/kernels/py5/__main__.py` & `py5jupyter-0.2.0a0/py5jupyter/widgets/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # *****************************************************************************
 #
 #   Part of the py5jupyter (& py5) library
-#   Copyright (C) 2022 Jim Schmitz
+#   Copyright (C) 2022-2023 Jim Schmitz
 #
 #   This library is free software: you can redistribute it and/or modify it
 #   under the terms of the GNU Lesser General Public License as published by
 #   the Free Software Foundation, either version 2.1 of the License, or (at
 #   your option) any later version.
 #
 #   This library is distributed in the hope that it will be useful, but
@@ -13,10 +13,8 @@
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser
 #   General Public License for more details.
 #
 #   You should have received a copy of the GNU Lesser General Public License
 #   along with this library. If not, see <https://www.gnu.org/licenses/>.
 #
 # *****************************************************************************
-from .kernel import Py5App
-
-Py5App.launch_instance()
+from .sketchportal import Py5SketchPortal
```

### Comparing `py5jupyter-0.1.2a1/py5jupyter/kernels/py5/install.py` & `py5jupyter-0.2.0a0/py5jupyter/kernels/py5/install.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # *****************************************************************************
 #
 #   Part of the py5jupyter (& py5) library
-#   Copyright (C) 2022 Jim Schmitz
+#   Copyright (C) 2022-2023 Jim Schmitz
 #
 #   This library is free software: you can redistribute it and/or modify it
 #   under the terms of the GNU Lesser General Public License as published by
 #   the Free Software Foundation, either version 2.1 of the License, or (at
 #   your option) any later version.
 #
 #   This library is distributed in the hope that it will be useful, but
```

### Comparing `py5jupyter-0.1.2a1/py5jupyter/kernels/py5/kernel.py` & `py5jupyter-0.2.0a0/py5jupyter/kernels/py5/kernel.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # *****************************************************************************
 #
 #   Part of the py5jupyter (& py5) library
-#   Copyright (C) 2022 Jim Schmitz
+#   Copyright (C) 2022-2023 Jim Schmitz
 #
 #   This library is free software: you can redistribute it and/or modify it
 #   under the terms of the GNU Lesser General Public License as published by
 #   the Free Software Foundation, either version 2.1 of the License, or (at
 #   your option) any later version.
 #
 #   This library is distributed in the hope that it will be useful, but
@@ -23,24 +23,24 @@
 from ipykernel.zmqshell import ZMQInteractiveShell
 from IPython.core.interactiveshell import InteractiveShellABC
 from ipykernel.kernelapp import IPKernelApp
 
 from traitlets import Type, Instance, Unicode, List
 
 from py5_tools.parsing import TransformDynamicVariablesToCalls, Py5CodeValidation
-
+from py5_tools import __version__ as __py5_version__
 
 _PY5_HELP_LINKS = [
     {
-        'text': 'py5 Reference',
-        'url': 'http://py5.ixora.io/reference/'
+        'text': 'py5 Documentation',
+        'url': 'http://py5coding.org/'
     },
     {
-        'text': 'py5 Tutorials',
-        'url': 'http://py5.ixora.io/tutorials/'
+        'text': 'py5 Function Reference',
+        'url': 'http://py5coding.org/reference/sketch.html'
     },
 ]
 
 _MACOSX_PRE_STARTUP = """
 get_ipython().run_line_magic('gui', 'osx')
 """
 
@@ -54,30 +54,30 @@
 _KERNEL_STARTUP = (_MACOSX_PRE_STARTUP if sys.platform == 'darwin' else "") + _DEFAULT_STARTUP
 
 
 class Py5Shell(ZMQInteractiveShell):
 
     ast_transformers = List([TransformDynamicVariablesToCalls(), Py5CodeValidation()]).tag(config=True)
 
-    banner2 = Unicode("Activating py5 imported mode").tag(config=True)
+    banner2 = Unicode("py5 " + __py5_version__ + " | py5 kernel 0.1.3a0 | A Python Jupyter kernel plus py5 in imported mode").tag(config=True)
 
 
 InteractiveShellABC.register(Py5Shell)
 
 
 class Py5Kernel(IPythonKernel):
     shell = Instance('IPython.core.interactiveshell.InteractiveShellABC',
                      allow_none=True)
     shell_class = Type(Py5Shell)
 
     help_links = List([*IPythonKernel.help_links.default(),
                        *_PY5_HELP_LINKS]).tag(config=True)
 
     implementation = 'py5'
-    implementation_version = '0.7.3.dev0'
+    implementation_version = '0.1.3a0'
 
 
 class Py5App(IPKernelApp):
     name = 'py5-kernel'
 
     kernel_class = Type('py5jupyter.kernels.py5.Py5Kernel',
                         klass='ipykernel.kernelbase.Kernel').tag(config=True)
```

### Comparing `py5jupyter-0.1.2a1/py5jupyter/kernels/py5bot/__init__.py` & `py5jupyter-0.2.0a0/py5jupyter/kernels/py5bot/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # *****************************************************************************
 #
 #   Part of the py5jupyter (& py5) library
-#   Copyright (C) 2022 Jim Schmitz
+#   Copyright (C) 2022-2023 Jim Schmitz
 #
 #   This library is free software: you can redistribute it and/or modify it
 #   under the terms of the GNU Lesser General Public License as published by
 #   the Free Software Foundation, either version 2.1 of the License, or (at
 #   your option) any later version.
 #
 #   This library is distributed in the hope that it will be useful, but
```

### Comparing `py5jupyter-0.1.2a1/py5jupyter/kernels/py5bot/__main__.py` & `py5jupyter-0.2.0a0/py5jupyter/kernels/py5bot/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # *****************************************************************************
 #
 #   Part of the py5jupyter (& py5) library
-#   Copyright (C) 2022 Jim Schmitz
+#   Copyright (C) 2022-2023 Jim Schmitz
 #
 #   This library is free software: you can redistribute it and/or modify it
 #   under the terms of the GNU Lesser General Public License as published by
 #   the Free Software Foundation, either version 2.1 of the License, or (at
 #   your option) any later version.
 #
 #   This library is distributed in the hope that it will be useful, but
```

### Comparing `py5jupyter-0.1.2a1/py5jupyter/kernels/py5bot/install.py` & `py5jupyter-0.2.0a0/py5jupyter/kernels/py5bot/install.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # *****************************************************************************
 #
 #   Part of the py5jupyter (& py5) library
-#   Copyright (C) 2022 Jim Schmitz
+#   Copyright (C) 2022-2023 Jim Schmitz
 #
 #   This library is free software: you can redistribute it and/or modify it
 #   under the terms of the GNU Lesser General Public License as published by
 #   the Free Software Foundation, either version 2.1 of the License, or (at
 #   your option) any later version.
 #
 #   This library is distributed in the hope that it will be useful, but
```

### Comparing `py5jupyter-0.1.2a1/py5jupyter/kernels/py5bot/kernel.py` & `py5jupyter-0.2.0a0/py5jupyter/kernels/py5bot/kernel.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # *****************************************************************************
 #
 #   Part of the py5jupyter (& py5) library
-#   Copyright (C) 2022 Jim Schmitz
+#   Copyright (C) 2022-2023 Jim Schmitz
 #
 #   This library is free software: you can redistribute it and/or modify it
 #   under the terms of the GNU Lesser General Public License as published by
 #   the Free Software Foundation, either version 2.1 of the License, or (at
 #   your option) any later version.
 #
 #   This library is distributed in the hope that it will be useful, but
@@ -15,43 +15,57 @@
 #
 #   You should have received a copy of the GNU Lesser General Public License
 #   along with this library. If not, see <https://www.gnu.org/licenses/>.
 #
 # *****************************************************************************
 import sys
 
+from ipykernel.ipkernel import IPythonKernel
 from ipykernel.zmqshell import ZMQInteractiveShell
 from IPython.core.interactiveshell import InteractiveShellABC
 from ipykernel.kernelapp import IPKernelApp
 
 from traitlets import Type, Instance, Unicode, List
 
-from ..py5.kernel import Py5Kernel
 from py5_tools import split_setup
+from py5_tools.parsing import TransformDynamicVariablesToCalls, Py5CodeValidation, check_for_problems
+from py5_tools import __version__ as __py5_version__
+
 from . import py5bot
-from py5_tools.parsing import TransformDynamicVariablesToCalls, Py5CodeValidation
+
+
+_PY5_HELP_LINKS = [
+    {
+        'text': 'py5 Documentation',
+        'url': 'http://py5coding.org/'
+    },
+    {
+        'text': 'py5 Function Reference',
+        'url': 'http://py5coding.org/reference/sketch.html'
+    },
+]
 
 
 class Py5BotShell(ZMQInteractiveShell):
 
     # needed to make sure code using the %%python bypass gets transformed
     ast_transformers = List([TransformDynamicVariablesToCalls(), Py5CodeValidation()]).tag(config=True)
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._py5bot_mgr = py5bot.Py5BotManager()
 
-    banner2 = Unicode("Activating py5bot").tag(config=True)
+    banner2 = Unicode("py5 " + __py5_version__ + " | py5bot kernel 0.1.3a0 | A static drawing environment for py5").tag(config=True)
 
     def run_cell(self, raw_cell, *args, **kwargs):
         # check for special code that should bypass py5bot processing
         if raw_cell.strip().startswith('%%python\n'):
             return super(Py5BotShell, self).run_cell(raw_cell.replace('%%python\n', ''), *args, **kwargs)
 
-        success, result = py5bot.check_for_problems(raw_cell, "<py5bot>")
+        success, result = check_for_problems(raw_cell, "<py5bot>", tool='py5bot')
         if success:
             py5bot_globals, py5bot_settings, py5bot_setup = result
             if split_setup.count_noncomment_lines(py5bot_settings) == 0:
                 py5bot_settings = 'size(100, 100, HIDDEN)'
             self._py5bot_mgr.write_code(py5bot_globals, py5bot_settings, py5bot_setup)
 
             return super(Py5BotShell, self).run_cell(self._py5bot_mgr.run_code, *args, **kwargs)
@@ -59,21 +73,24 @@
             print(result, file=sys.stderr)
 
             return super(Py5BotShell, self).run_cell('None', *args, **kwargs)
 
 InteractiveShellABC.register(Py5BotShell)
 
 
-class Py5BotKernel(Py5Kernel):
+class Py5BotKernel(IPythonKernel):
     shell = Instance('IPython.core.interactiveshell.InteractiveShellABC',
                      allow_none=True)
     shell_class = Type(Py5BotShell)
 
+    help_links = List([*IPythonKernel.help_links.default(),
+                       *_PY5_HELP_LINKS]).tag(config=True)
+
     implementation = 'py5bot'
-    implementation_version = '0.7.3.dev0'
+    implementation_version = '0.1.3a0'
 
 
 class Py5BotApp(IPKernelApp):
     name = 'py5bot-kernel'
 
     kernel_class = Type('py5jupyter.kernels.py5bot.Py5BotKernel',
                         klass='ipykernel.kernelbase.Kernel').tag(config=True)
```

### Comparing `py5jupyter-0.1.2a1/py5jupyter/labextension/build_log.json` & `py5jupyter-0.2.0a0/py5jupyter/labextension/build_log.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9971359427609426%*

 * *Differences: {'0': "{'resolve': {'fallback': {'crypto': False}}, 'plugins': {1: {'_options': {'shared': "*

 * *      "{'@jupyterlab/application': {'requiredVersion': '^3.5.1'}, "*

 * *      "'@jupyterlab/application-extension': {'requiredVersion': '^3.5.1'}, "*

 * *      "'@jupyterlab/apputils-extension': {'requiredVersion': '^3.5.1'}, "*

 * *      "'@jupyterlab/cell-toolbar-extension': {'requiredVersion': '^3.5.1'}, "*

 * *      "'@jupyterlab/celltags-extension': {'requiredVersion': '^3.5.1'}, "*

 * *      "'@jupyterlab/codemirror-extension': {'req […]*

```diff
@@ -115,418 +115,418 @@
                     "shared": {
                         "@jupyter-widgets/base": {
                             "import": false,
                             "singleton": true
                         },
                         "@jupyterlab/application": {
                             "import": false,
-                            "requiredVersion": "^3.4.0",
+                            "requiredVersion": "^3.5.1",
                             "singleton": true
                         },
                         "@jupyterlab/application-extension": {
                             "import": false,
-                            "requiredVersion": "^3.4.0"
+                            "requiredVersion": "^3.5.1"
                         },
                         "@jupyterlab/apputils": {
                             "import": false,
-                            "requiredVersion": "^3.4.0",
+                            "requiredVersion": "^3.5.1",
                             "singleton": true
                         },
                         "@jupyterlab/apputils-extension": {
                             "import": false,
-                            "requiredVersion": "^3.4.0"
+                            "requiredVersion": "^3.5.1"
                         },
                         "@jupyterlab/attachments": {
                             "import": false,
-                            "requiredVersion": "^3.4.0"
+                            "requiredVersion": "^3.5.1"
                         },
                         "@jupyterlab/cell-toolbar": {
                             "import": false,
-                            "requiredVersion": "^3.4.0",
+                            "requiredVersion": "^3.5.1",
                             "singleton": true
                         },
                         "@jupyterlab/cell-toolbar-extension": {
                             "import": false,
-                            "requiredVersion": "^3.4.0"
+                            "requiredVersion": "^3.5.1"
                         },
                         "@jupyterlab/cells": {
                             "import": false,
-                            "requiredVersion": "^3.4.0"
+                            "requiredVersion": "^3.5.1"
                         },
                         "@jupyterlab/celltags": {
                             "import": false,
-                            "requiredVersion": "^3.4.0"
+                            "requiredVersion": "^3.5.1"
                         },
                         "@jupyterlab/celltags-extension": {
                             "import": false,
-                            "requiredVersion": "^3.4.0"
+                            "requiredVersion": "^3.5.1"
                         },
                         "@jupyterlab/codeeditor": {
                             "import": false,
-                            "requiredVersion": "^3.4.0",
+                            "requiredVersion": "^3.5.1",
                             "singleton": true
                         },
                         "@jupyterlab/codemirror": {
                             "import": false,
-                            "requiredVersion": "^3.4.0",
+                            "requiredVersion": "^3.5.1",
                             "singleton": true
                         },
                         "@jupyterlab/codemirror-extension": {
                             "import": false,
-                            "requiredVersion": "^3.4.0"
+                            "requiredVersion": "^3.5.1"
                         },
                         "@jupyterlab/completer": {
                             "import": false,
-                            "requiredVersion": "^3.4.0",
+                            "requiredVersion": "^3.5.1",
                             "singleton": true
                         },
                         "@jupyterlab/completer-extension": {
                             "import": false,
-                            "requiredVersion": "^3.4.0"
+                            "requiredVersion": "^3.5.1"
                         },
                         "@jupyterlab/console": {
                             "import": false,
-                            "requiredVersion": "^3.4.0",
+                            "requiredVersion": "^3.5.1",
                             "singleton": true
                         },
                         "@jupyterlab/console-extension": {
                             "import": false,
-                            "requiredVersion": "^3.4.0"
+                            "requiredVersion": "^3.5.1"
                         },
                         "@jupyterlab/coreutils": {
                             "import": false,
-                            "requiredVersion": "^5.4.0",
+                            "requiredVersion": "^5.5.1",
                             "singleton": true
                         },
                         "@jupyterlab/csvviewer": {
                             "import": false,
-                            "requiredVersion": "^3.4.0"
+                            "requiredVersion": "^3.5.1"
                         },
                         "@jupyterlab/csvviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^3.4.0"
+                            "requiredVersion": "^3.5.1"
                         },
                         "@jupyterlab/debugger": {
                             "import": false,
-                            "requiredVersion": "^3.4.0",
+                            "requiredVersion": "^3.5.1",
                             "singleton": true
                         },
                         "@jupyterlab/debugger-extension": {
                             "import": false,
-                            "requiredVersion": "^3.4.0"
+                            "requiredVersion": "^3.5.1"
                         },
                         "@jupyterlab/docmanager": {
                             "import": false,
-                            "requiredVersion": "^3.4.0",
+                            "requiredVersion": "^3.5.1",
                             "singleton": true
                         },
                         "@jupyterlab/docmanager-extension": {
                             "import": false,
-                            "requiredVersion": "^3.4.0"
+                            "requiredVersion": "^3.5.1"
                         },
                         "@jupyterlab/docprovider": {
                             "import": false,
-                            "requiredVersion": "^3.4.0",
+                            "requiredVersion": "^3.5.1",
                             "singleton": true
                         },
                         "@jupyterlab/docprovider-extension": {
                             "import": false,
-                            "requiredVersion": "^3.4.0"
+                            "requiredVersion": "^3.5.1"
                         },
                         "@jupyterlab/docregistry": {
                             "import": false,
-                            "requiredVersion": "^3.4.0"
+                            "requiredVersion": "^3.5.1"
                         },
                         "@jupyterlab/documentsearch": {
                             "import": false,
-                            "requiredVersion": "^3.4.0",
+                            "requiredVersion": "^3.5.1",
                             "singleton": true
                         },
                         "@jupyterlab/documentsearch-extension": {
                             "import": false,
-                            "requiredVersion": "^3.4.0"
+                            "requiredVersion": "^3.5.1"
                         },
                         "@jupyterlab/extensionmanager": {
                             "import": false,
-                            "requiredVersion": "^3.4.0",
+                            "requiredVersion": "^3.5.1",
                             "singleton": true
                         },
                         "@jupyterlab/extensionmanager-extension": {
                             "import": false,
-                            "requiredVersion": "^3.4.0"
+                            "requiredVersion": "^3.5.1"
                         },
                         "@jupyterlab/filebrowser": {
                             "import": false,
-                            "requiredVersion": "^3.4.0",
+                            "requiredVersion": "^3.5.1",
                             "singleton": true
                         },
                         "@jupyterlab/filebrowser-extension": {
                             "import": false,
-                            "requiredVersion": "^3.4.0"
+                            "requiredVersion": "^3.5.1"
                         },
                         "@jupyterlab/fileeditor": {
                             "import": false,
-                            "requiredVersion": "^3.4.0",
+                            "requiredVersion": "^3.5.1",
                             "singleton": true
                         },
                         "@jupyterlab/fileeditor-extension": {
                             "import": false,
-                            "requiredVersion": "^3.4.0"
+                            "requiredVersion": "^3.5.1"
                         },
                         "@jupyterlab/help-extension": {
                             "import": false,
-                            "requiredVersion": "^3.4.0"
+                            "requiredVersion": "^3.5.1"
                         },
                         "@jupyterlab/htmlviewer": {
                             "import": false,
-                            "requiredVersion": "^3.4.0"
+                            "requiredVersion": "^3.5.1"
                         },
                         "@jupyterlab/htmlviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^3.4.0"
+                            "requiredVersion": "^3.5.1"
                         },
                         "@jupyterlab/hub-extension": {
                             "import": false,
-                            "requiredVersion": "^3.4.0"
+                            "requiredVersion": "^3.5.1"
                         },
                         "@jupyterlab/imageviewer": {
                             "import": false,
-                            "requiredVersion": "^3.4.0",
+                            "requiredVersion": "^3.5.1",
                             "singleton": true
                         },
                         "@jupyterlab/imageviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^3.4.0"
+                            "requiredVersion": "^3.5.1"
                         },
                         "@jupyterlab/inspector": {
                             "import": false,
-                            "requiredVersion": "^3.4.0",
+                            "requiredVersion": "^3.5.1",
                             "singleton": true
                         },
                         "@jupyterlab/inspector-extension": {
                             "import": false,
-                            "requiredVersion": "^3.4.0"
+                            "requiredVersion": "^3.5.1"
                         },
                         "@jupyterlab/javascript-extension": {
                             "import": false,
-                            "requiredVersion": "^3.4.0"
+                            "requiredVersion": "^3.5.1"
                         },
                         "@jupyterlab/json-extension": {
                             "import": false,
-                            "requiredVersion": "^3.4.0"
+                            "requiredVersion": "^3.5.1"
                         },
                         "@jupyterlab/launcher": {
                             "import": false,
-                            "requiredVersion": "^3.4.0",
+                            "requiredVersion": "^3.5.1",
                             "singleton": true
                         },
                         "@jupyterlab/launcher-extension": {
                             "import": false,
-                            "requiredVersion": "^3.4.0"
+                            "requiredVersion": "^3.5.1"
                         },
                         "@jupyterlab/logconsole": {
                             "import": false,
-                            "requiredVersion": "^3.4.0",
+                            "requiredVersion": "^3.5.1",
                             "singleton": true
                         },
                         "@jupyterlab/logconsole-extension": {
                             "import": false,
-                            "requiredVersion": "^3.4.0"
+                            "requiredVersion": "^3.5.1"
                         },
                         "@jupyterlab/mainmenu": {
                             "import": false,
-                            "requiredVersion": "^3.4.0",
+                            "requiredVersion": "^3.5.1",
                             "singleton": true
                         },
                         "@jupyterlab/mainmenu-extension": {
                             "import": false,
-                            "requiredVersion": "^3.4.0"
+                            "requiredVersion": "^3.5.1"
                         },
                         "@jupyterlab/markdownviewer": {
                             "import": false,
-                            "requiredVersion": "^3.4.0",
+                            "requiredVersion": "^3.5.1",
                             "singleton": true
                         },
                         "@jupyterlab/markdownviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^3.4.0"
+                            "requiredVersion": "^3.5.1"
                         },
                         "@jupyterlab/mathjax2": {
                             "import": false,
-                            "requiredVersion": "^3.4.0"
+                            "requiredVersion": "^3.5.1"
                         },
                         "@jupyterlab/mathjax2-extension": {
                             "import": false,
-                            "requiredVersion": "^3.4.0"
+                            "requiredVersion": "^3.5.1"
                         },
                         "@jupyterlab/metapackage": {
                             "import": false,
-                            "requiredVersion": "^3.4.0"
+                            "requiredVersion": "^3.5.1"
                         },
                         "@jupyterlab/nbconvert-css": {
                             "import": false,
-                            "requiredVersion": "^3.4.0"
+                            "requiredVersion": "^3.5.1"
                         },
                         "@jupyterlab/nbformat": {
                             "import": false,
-                            "requiredVersion": "^3.4.0"
+                            "requiredVersion": "^3.5.1"
                         },
                         "@jupyterlab/notebook": {
                             "import": false,
-                            "requiredVersion": "^3.4.0",
+                            "requiredVersion": "^3.5.1",
                             "singleton": true
                         },
                         "@jupyterlab/notebook-extension": {
                             "import": false,
-                            "requiredVersion": "^3.4.0"
+                            "requiredVersion": "^3.5.1"
                         },
                         "@jupyterlab/observables": {
                             "import": false,
-                            "requiredVersion": "^4.4.0"
+                            "requiredVersion": "^4.5.1"
                         },
                         "@jupyterlab/outputarea": {
                             "import": false,
-                            "requiredVersion": "^3.4.0"
+                            "requiredVersion": "^3.5.1"
                         },
                         "@jupyterlab/pdf-extension": {
                             "import": false,
-                            "requiredVersion": "^3.4.0"
+                            "requiredVersion": "^3.5.1"
                         },
                         "@jupyterlab/property-inspector": {
                             "import": false,
-                            "requiredVersion": "^3.4.0"
+                            "requiredVersion": "^3.5.1"
                         },
                         "@jupyterlab/rendermime": {
                             "import": false,
-                            "requiredVersion": "^3.4.0",
+                            "requiredVersion": "^3.5.1",
                             "singleton": true
                         },
                         "@jupyterlab/rendermime-extension": {
                             "import": false,
-                            "requiredVersion": "^3.4.0"
+                            "requiredVersion": "^3.5.1"
                         },
                         "@jupyterlab/rendermime-interfaces": {
                             "import": false,
-                            "requiredVersion": "^3.4.0",
+                            "requiredVersion": "^3.5.1",
                             "singleton": true
                         },
                         "@jupyterlab/running": {
                             "import": false,
-                            "requiredVersion": "^3.4.0"
+                            "requiredVersion": "^3.5.1"
                         },
                         "@jupyterlab/running-extension": {
                             "import": false,
-                            "requiredVersion": "^3.4.0"
+                            "requiredVersion": "^3.5.1"
                         },
                         "@jupyterlab/services": {
                             "import": false,
-                            "requiredVersion": "^6.4.0",
+                            "requiredVersion": "^6.5.1",
                             "singleton": true
                         },
                         "@jupyterlab/settingeditor": {
                             "import": false,
-                            "requiredVersion": "^3.4.0",
+                            "requiredVersion": "^3.5.1",
                             "singleton": true
                         },
                         "@jupyterlab/settingeditor-extension": {
                             "import": false,
-                            "requiredVersion": "^3.4.0"
+                            "requiredVersion": "^3.5.1"
                         },
                         "@jupyterlab/settingregistry": {
                             "import": false,
-                            "requiredVersion": "^3.4.0",
+                            "requiredVersion": "^3.5.1",
                             "singleton": true
                         },
                         "@jupyterlab/shared-models": {
                             "import": false,
-                            "requiredVersion": "^3.4.0",
+                            "requiredVersion": "^3.5.1",
                             "singleton": true
                         },
                         "@jupyterlab/shortcuts-extension": {
                             "import": false,
-                            "requiredVersion": "^3.4.0"
+                            "requiredVersion": "^3.5.1"
                         },
                         "@jupyterlab/statedb": {
                             "import": false,
-                            "requiredVersion": "^3.4.0",
+                            "requiredVersion": "^3.5.1",
                             "singleton": true
                         },
                         "@jupyterlab/statusbar": {
                             "import": false,
-                            "requiredVersion": "^3.4.0",
+                            "requiredVersion": "^3.5.1",
                             "singleton": true
                         },
                         "@jupyterlab/statusbar-extension": {
                             "import": false,
-                            "requiredVersion": "^3.4.0"
+                            "requiredVersion": "^3.5.1"
                         },
                         "@jupyterlab/terminal": {
                             "import": false,
-                            "requiredVersion": "^3.4.0",
+                            "requiredVersion": "^3.5.1",
                             "singleton": true
                         },
                         "@jupyterlab/terminal-extension": {
                             "import": false,
-                            "requiredVersion": "^3.4.0"
+                            "requiredVersion": "^3.5.1"
                         },
                         "@jupyterlab/theme-dark-extension": {
                             "import": false,
-                            "requiredVersion": "^3.4.0"
+                            "requiredVersion": "^3.5.1"
                         },
                         "@jupyterlab/theme-light-extension": {
                             "import": false,
-                            "requiredVersion": "^3.4.0"
+                            "requiredVersion": "^3.5.1"
                         },
                         "@jupyterlab/toc": {
                             "import": false,
-                            "requiredVersion": "^5.4.0",
+                            "requiredVersion": "^5.5.1",
                             "singleton": true
                         },
                         "@jupyterlab/toc-extension": {
                             "import": false,
-                            "requiredVersion": "^5.4.0"
+                            "requiredVersion": "^5.5.1"
                         },
                         "@jupyterlab/tooltip": {
                             "import": false,
-                            "requiredVersion": "^3.4.0",
+                            "requiredVersion": "^3.5.1",
                             "singleton": true
                         },
                         "@jupyterlab/tooltip-extension": {
                             "import": false,
-                            "requiredVersion": "^3.4.0"
+                            "requiredVersion": "^3.5.1"
                         },
                         "@jupyterlab/translation": {
                             "import": false,
-                            "requiredVersion": "^3.4.0",
+                            "requiredVersion": "^3.5.1",
                             "singleton": true
                         },
                         "@jupyterlab/translation-extension": {
                             "import": false,
-                            "requiredVersion": "^3.4.0"
+                            "requiredVersion": "^3.5.1"
                         },
                         "@jupyterlab/ui-components": {
                             "import": false,
-                            "requiredVersion": "^3.4.0",
+                            "requiredVersion": "^3.5.1",
                             "singleton": true
                         },
                         "@jupyterlab/ui-components-extension": {
                             "import": false,
-                            "requiredVersion": "^3.4.0"
+                            "requiredVersion": "^3.5.1"
                         },
                         "@jupyterlab/vdom": {
                             "import": false,
-                            "requiredVersion": "^3.4.0"
+                            "requiredVersion": "^3.5.1"
                         },
                         "@jupyterlab/vdom-extension": {
                             "import": false,
-                            "requiredVersion": "^3.4.0"
+                            "requiredVersion": "^3.5.1"
                         },
                         "@jupyterlab/vega5-extension": {
                             "import": false,
-                            "requiredVersion": "^3.4.0"
+                            "requiredVersion": "^3.5.1"
                         },
                         "@lumino/algorithm": {
                             "import": false,
                             "requiredVersion": "^1.9.0",
                             "singleton": true
                         },
                         "@lumino/application": {
@@ -577,15 +577,15 @@
                         "@lumino/virtualdom": {
                             "import": false,
                             "requiredVersion": "^1.14.0",
                             "singleton": true
                         },
                         "@lumino/widgets": {
                             "import": false,
-                            "requiredVersion": "^1.30.0",
+                            "requiredVersion": "^1.33.0",
                             "singleton": true
                         },
                         "jupyter-py5": {
                             "import": "/home/jim/Projects/ITP/pythonprocessing/py5jupyter/lib/index.js",
                             "singleton": true,
                             "version": "0.1.0"
                         },
@@ -624,14 +624,15 @@
                 "@phosphor/signaling": "/home/jim/Projects/ITP/pythonprocessing/py5jupyter/node_modules/@lumino/signaling/dist/index.js",
                 "@phosphor/virtualdom$": "/home/jim/Projects/ITP/pythonprocessing/py5jupyter/node_modules/@lumino/virtualdom/dist/index.js",
                 "@phosphor/widgets$": "/home/jim/Projects/ITP/pythonprocessing/py5jupyter/node_modules/@lumino/widgets/dist/index.js",
                 "@phosphor/widgets/style": "/home/jim/Projects/ITP/pythonprocessing/py5jupyter/node_modules/@lumino/widgets/style"
             },
             "fallback": {
                 "buffer": false,
+                "crypto": false,
                 "path": "/home/jim/Projects/ITP/pythonprocessing/py5jupyter/node_modules/path-browserify/index.js",
                 "process": "/home/jim/Projects/ITP/pythonprocessing/py5jupyter/node_modules/process/browser.js",
                 "url": false
             }
         },
         "watchOptions": {
             "aggregateTimeout": 1000,
```

### Comparing `py5jupyter-0.1.2a1/py5jupyter/labextension/package.json` & `py5jupyter-0.2.0a0/py5jupyter/labextension/package.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9990234375%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.102c2185a6a3be91ce3c.js'}}"}*

```diff
@@ -45,15 +45,15 @@
         "dist/*.js",
         "css/*.css"
     ],
     "homepage": "https://github.com/py5coding/py5jupyter",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.042026d6e03651ecc3fd.js"
+            "load": "static/remoteEntry.102c2185a6a3be91ce3c.js"
         },
         "extension": "lib/plugin",
         "outputDir": "py5jupyter/labextension/",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
```

### Comparing `py5jupyter-0.1.2a1/py5jupyter/labextension/static/lib_index_js.488a66c2de85320bc65a.js` & `py5jupyter-0.2.0a0/py5jupyter/labextension/static/lib_index_js.b65cf7c58127bf49a498.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -29,15 +29,15 @@
                 };
                 Object.defineProperty(exports, "__esModule", ({
                     value: true
                 }));
                 // *****************************************************************************
                 //
                 //   Part of the py5jupyter (& py5) library
-                //   Copyright (C) 2022 Jim Schmitz
+                //   Copyright (C) 2022-2023 Jim Schmitz
                 //
                 //   This library is free software: you can redistribute it and/or modify it
                 //   under the terms of the GNU Lesser General Public License as published by
                 //   the Free Software Foundation, either version 2.1 of the License, or (at
                 //   your option) any later version.
                 //
                 //   This library is distributed in the hope that it will be useful, but
@@ -54,8 +54,8 @@
                 //# sourceMappingURL=index.js.map
 
                 /***/
             })
 
     }
 ]);
-//# sourceMappingURL=lib_index_js.488a66c2de85320bc65a.js.map
+//# sourceMappingURL=lib_index_js.b65cf7c58127bf49a498.js.map
```

### Comparing `py5jupyter-0.1.2a1/py5jupyter/labextension/static/lib_index_js.488a66c2de85320bc65a.js.map` & `py5jupyter-0.2.0a0/py5jupyter/labextension/static/lib_index_js.b65cf7c58127bf49a498.js.map`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8571428571428571%*

 * *Differences: {"'file'": "'lib_index_js.b65cf7c58127bf49a498.js'",*

 * * "'sourcesContent'": '[\'"use strict";\\nvar __createBinding = (this && this.__createBinding) || '*

 * *                     '(Object.create ? (function(o, m, k, k2) {\\n    if (k2 === undefined) k2 = '*

 * *                     'k;\\n    Object.defineProperty(o, k2, { enumerable: true, get: function() { '*

 * *                     'return m[k]; } });\\n}) : (function(o, m, k, k2) {\\n    if (k2 === '*

 * *                     'undefined) k2 = k;\\n    o[k2] = m[k];\\n}));\\ […]*

```diff
@@ -1,13 +1,13 @@
 {
-    "file": "lib_index_js.488a66c2de85320bc65a.js",
+    "file": "lib_index_js.b65cf7c58127bf49a498.js",
     "mappings": ";;;;;;;;;AAAa;AACb;AACA;AACA,mCAAmC,oCAAoC,gBAAgB;AACvF,CAAC;AACD;AACA;AACA,CAAC;AACD;AACA;AACA;AACA,8CAA6C,EAAE,aAAa,EAAC;AAC7D;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,2BAA2B;AAC3B;AACA;AACA;AACA;AACA;AACA;AACA;AACA,aAAa,mBAAO,CAAC,mCAAW;AAChC,aAAa,mBAAO,CAAC,iCAAU;AAC/B",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://jupyter-py5/./lib/index.js"
     ],
     "sourcesContent": [
-        "\"use strict\";\nvar __createBinding = (this && this.__createBinding) || (Object.create ? (function(o, m, k, k2) {\n    if (k2 === undefined) k2 = k;\n    Object.defineProperty(o, k2, { enumerable: true, get: function() { return m[k]; } });\n}) : (function(o, m, k, k2) {\n    if (k2 === undefined) k2 = k;\n    o[k2] = m[k];\n}));\nvar __exportStar = (this && this.__exportStar) || function(m, exports) {\n    for (var p in m) if (p !== \"default\" && !Object.prototype.hasOwnProperty.call(exports, p)) __createBinding(exports, m, p);\n};\nObject.defineProperty(exports, \"__esModule\", { value: true });\n// *****************************************************************************\n//\n//   Part of the py5jupyter (& py5) library\n//   Copyright (C) 2022 Jim Schmitz\n//\n//   This library is free software: you can redistribute it and/or modify it\n//   under the terms of the GNU Lesser General Public License as published by\n//   the Free Software Foundation, either version 2.1 of the License, or (at\n//   your option) any later version.\n//\n//   This library is distributed in the hope that it will be useful, but\n//   WITHOUT ANY WARRANTY; without even the implied warranty of\n//   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser\n//   General Public License for more details.\n//\n//   You should have received a copy of the GNU Lesser General Public License\n//   along with this library. If not, see <https://www.gnu.org/licenses/>.\n//\n// *****************************************************************************\n__exportStar(require(\"./version\"), exports);\n__exportStar(require(\"./widget\"), exports);\n//# sourceMappingURL=index.js.map"
+        "\"use strict\";\nvar __createBinding = (this && this.__createBinding) || (Object.create ? (function(o, m, k, k2) {\n    if (k2 === undefined) k2 = k;\n    Object.defineProperty(o, k2, { enumerable: true, get: function() { return m[k]; } });\n}) : (function(o, m, k, k2) {\n    if (k2 === undefined) k2 = k;\n    o[k2] = m[k];\n}));\nvar __exportStar = (this && this.__exportStar) || function(m, exports) {\n    for (var p in m) if (p !== \"default\" && !Object.prototype.hasOwnProperty.call(exports, p)) __createBinding(exports, m, p);\n};\nObject.defineProperty(exports, \"__esModule\", { value: true });\n// *****************************************************************************\n//\n//   Part of the py5jupyter (& py5) library\n//   Copyright (C) 2022-2023 Jim Schmitz\n//\n//   This library is free software: you can redistribute it and/or modify it\n//   under the terms of the GNU Lesser General Public License as published by\n//   the Free Software Foundation, either version 2.1 of the License, or (at\n//   your option) any later version.\n//\n//   This library is distributed in the hope that it will be useful, but\n//   WITHOUT ANY WARRANTY; without even the implied warranty of\n//   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser\n//   General Public License for more details.\n//\n//   You should have received a copy of the GNU Lesser General Public License\n//   along with this library. If not, see <https://www.gnu.org/licenses/>.\n//\n// *****************************************************************************\n__exportStar(require(\"./version\"), exports);\n__exportStar(require(\"./widget\"), exports);\n//# sourceMappingURL=index.js.map"
     ],
     "version": 3
 }
```

### Comparing `py5jupyter-0.1.2a1/py5jupyter/labextension/static/lib_plugin_js.586e3941dfcc287e7351.js` & `py5jupyter-0.2.0a0/py5jupyter/labextension/static/lib_plugin_js.586e3941dfcc287e7351.js`

 * *Files identical despite different names*

### Comparing `py5jupyter-0.1.2a1/py5jupyter/labextension/static/lib_plugin_js.586e3941dfcc287e7351.js.map` & `py5jupyter-0.2.0a0/py5jupyter/labextension/static/lib_plugin_js.586e3941dfcc287e7351.js.map`

 * *Files identical despite different names*

### Comparing `py5jupyter-0.1.2a1/py5jupyter/labextension/static/lib_widget_js.d141153e6400998a12a2.js` & `py5jupyter-0.2.0a0/py5jupyter/labextension/static/lib_widget_js.fc065f743fb92e735a68.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -10,15 +10,15 @@
             /***/
             (function(__unused_webpack_module, exports) {
 
 
                 // *****************************************************************************
                 //
                 //   Part of the py5jupyter (& py5) library
-                //   Copyright (C) 2022 Jim Schmitz
+                //   Copyright (C) 2022-2023 Jim Schmitz
                 //
                 //   This library is free software: you can redistribute it and/or modify it
                 //   under the terms of the GNU Lesser General Public License as published by
                 //   the Free Software Foundation, either version 2.1 of the License, or (at
                 //   your option) any later version.
                 //
                 //   This library is distributed in the hope that it will be useful, but
@@ -95,15 +95,15 @@
             /***/
             ((__unused_webpack_module, exports, __webpack_require__) => {
 
 
                 // *****************************************************************************
                 //
                 //   Part of the py5jupyter (& py5) library
-                //   Copyright (C) 2022 Jim Schmitz
+                //   Copyright (C) 2022-2023 Jim Schmitz
                 //
                 //   This library is free software: you can redistribute it and/or modify it
                 //   under the terms of the GNU Lesser General Public License as published by
                 //   the Free Software Foundation, either version 2.1 of the License, or (at
                 //   your option) any later version.
                 //
                 //   This library is distributed in the hope that it will be useful, but
@@ -180,15 +180,15 @@
                 Object.defineProperty(exports, "__esModule", ({
                     value: true
                 }));
                 exports.Py5SketchPortalView = exports.Py5SketchPortalModel = void 0;
                 // *****************************************************************************
                 //
                 //   Part of the py5jupyter (& py5) library
-                //   Copyright (C) 2022 Jim Schmitz
+                //   Copyright (C) 2022-2023 Jim Schmitz
                 //
                 //   This library is free software: you can redistribute it and/or modify it
                 //   under the terms of the GNU Lesser General Public License as published by
                 //   the Free Software Foundation, either version 2.1 of the License, or (at
                 //   your option) any later version.
                 //
                 //   This library is distributed in the hope that it will be useful, but
@@ -349,8 +349,8 @@
                 module.exports = JSON.parse('{"name":"jupyter-py5","version":"0.1.0","description":"py5 Jupyter tools","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/py5coding/py5jupyter","bugs":{"url":"https://github.com/py5coding/py5jupyter/issues"},"license":"BSD-3-Clause","author":{"name":"Jim Schmitz","email":"jim@ixora.io"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/py5coding/py5jupyter"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf py5jupyter/labextension","clean:nbextension":"rimraf py5jupyter/nbextension/static/index.js","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"yarn run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2.0.0 || ^3.0.0 || ^4.0.0"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyterlab/builder":"^3.0.0","@phosphor/application":"^1.6.0","@phosphor/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"py5jupyter/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}');
 
                 /***/
             })
 
     }
 ]);
-//# sourceMappingURL=lib_widget_js.d141153e6400998a12a2.js.map
+//# sourceMappingURL=lib_widget_js.fc065f743fb92e735a68.js.map
```

### Comparing `py5jupyter-0.1.2a1/py5jupyter/labextension/static/lib_widget_js.d141153e6400998a12a2.js.map` & `py5jupyter-0.2.0a0/py5jupyter/labextension/static/lib_widget_js.fc065f743fb92e735a68.js.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8571428571428571%*

 * *Differences: {"'file'": "'lib_widget_js.fc065f743fb92e735a68.js'",*

 * * "'sourcesContent'": '[\'"use strict";\\n// '*

 * *                     '*****************************************************************************\\n//\\n//   '*

 * *                     'Part of the py5jupyter (& py5) library\\n//   Copyright (C) 2022-2023 Jim '*

 * *                     'Schmitz\\n//\\n//   This library is free software: you can redistribute it '*

 * *                     'and/or modify it\\n//   under the terms of the GNU Lesser General Public '*

 * *     […]*

```diff
@@ -1,17 +1,17 @@
 {
-    "file": "lib_widget_js.d141153e6400998a12a2.js",
+    "file": "lib_widget_js.fc065f743fb92e735a68.js",
     "mappings": ";;;;;;;;;AAAa;AACb;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,2BAA2B;AAC3B;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,4BAA4B,+DAA+D,iBAAiB;AAC5G;AACA,oCAAoC,MAAM,+BAA+B,YAAY;AACrF,mCAAmC,MAAM,mCAAmC,YAAY;AACxF,gCAAgC;AAChC;AACA,KAAK;AACL;AACA,8CAA6C,EAAE,aAAa,EAAC;AAC7D,qBAAqB;AACrB;AACA;AACA;AACA;AACA;AACA,0CAA0C,oBAAoB;AAC9D;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT,KAAK;AACL;AACA,qBAAqB;AACrB;;;;;;;;;;AChDa;AACb;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,2BAA2B;AAC3B;AACA;AACA;AACA;AACA;AACA;AACA;AACA,8CAA6C,EAAE,aAAa,EAAC;AAC7D,mBAAmB,GAAG,sBAAsB;AAC5C;AACA;AACA;AACA,aAAa,mBAAO,CAAC,uCAAiB;AACtC;AACA;AACA;AACA;AACA;AACA;AACA,sBAAsB;AACtB;AACA;AACA;AACA,mBAAmB;AACnB;;;;;;;;;;ACrCa;AACb;AACA,4BAA4B,+DAA+D,iBAAiB;AAC5G;AACA,oCAAoC,MAAM,+BAA+B,YAAY;AACrF,mCAAmC,MAAM,mCAAmC,YAAY;AACxF,gCAAgC;AAChC;AACA,KAAK;AACL;AACA,8CAA6C,EAAE,aAAa,EAAC;AAC7D,2BAA2B,GAAG,4BAA4B;AAC1D;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,2BAA2B;AAC3B;AACA;AACA;AACA;AACA;AACA;AACA;AACA,eAAe,mBAAO,CAAC,oFAAuB;AAC9C,kBAAkB,mBAAO,CAAC,mCAAW;AACrC,gBAAgB,mBAAO,CAAC,+BAAS;AACjC;AACA;AACA;AACA,6CAA6C,uBAAuB,8XAA8X;AAClc;AACA;AACA,4BAA4B;AAC5B,iEAAiE,wCAAwC;AACzG;AACA;AACA,SAAS;AACT,OAAO;AACP;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA,SAAS;AACT;AACA;AACA,SAAS;AACT;AACA;AACA,SAAS;AACT;AACA;AACA,SAAS;AACT;AACA;AACA,SAAS;AACT;AACA;AACA,SAAS;AACT;AACA;AACA,SAAS;AACT;AACA;AACA,SAAS;AACT;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA,wCAAwC,yDAAyD,+BAA+B;AAChI;AACA;AACA,sDAAsD,2CAA2C,4DAA4D;AAC7J;AACA;AACA;AACA;AACA,sDAAsD,6CAA6C,4DAA4D;AAC/J;AACA;AACA;AACA,sDAAsD,0GAA0G,4DAA4D;AAC5N;AACA;AACA;AACA;AACA;AACA;AACA,iBAAiB;AACjB;AACA;AACA,iBAAiB;AACjB;AACA;AACA,2BAA2B;AAC3B",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://jupyter-py5/./lib/utils.js",
         "webpack://jupyter-py5/./lib/version.js",
         "webpack://jupyter-py5/./lib/widget.js"
     ],
     "sourcesContent": [
-        "\"use strict\";\n// *****************************************************************************\n//\n//   Part of the py5jupyter (& py5) library\n//   Copyright (C) 2022 Jim Schmitz\n//\n//   This library is free software: you can redistribute it and/or modify it\n//   under the terms of the GNU Lesser General Public License as published by\n//   the Free Software Foundation, either version 2.1 of the License, or (at\n//   your option) any later version.\n//\n//   This library is distributed in the hope that it will be useful, but\n//   WITHOUT ANY WARRANTY; without even the implied warranty of\n//   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser\n//   General Public License for more details.\n//\n//   You should have received a copy of the GNU Lesser General Public License\n//   along with this library. If not, see <https://www.gnu.org/licenses/>.\n//\n// *****************************************************************************\nvar __awaiter = (this && this.__awaiter) || function (thisArg, _arguments, P, generator) {\n    function adopt(value) { return value instanceof P ? value : new P(function (resolve) { resolve(value); }); }\n    return new (P || (P = Promise))(function (resolve, reject) {\n        function fulfilled(value) { try { step(generator.next(value)); } catch (e) { reject(e); } }\n        function rejected(value) { try { step(generator[\"throw\"](value)); } catch (e) { reject(e); } }\n        function step(result) { result.done ? resolve(result.value) : adopt(result.value).then(fulfilled, rejected); }\n        step((generator = generator.apply(thisArg, _arguments || [])).next());\n    });\n};\nObject.defineProperty(exports, \"__esModule\", { value: true });\nexports.bufferToImage = void 0;\n// The below function came from the wonderful Python library ipycanvas\n// https://github.com/martinRenou/ipycanvas\nfunction bufferToImage(buffer) {\n    return __awaiter(this, void 0, void 0, function* () {\n        let url;\n        const blob = new Blob([buffer], { type: 'image/jpeg' });\n        url = URL.createObjectURL(blob);\n        const img = new Image();\n        return new Promise(resolve => {\n            img.onload = () => {\n                resolve(img);\n            };\n            img.src = url;\n        });\n    });\n}\nexports.bufferToImage = bufferToImage;\n//# sourceMappingURL=utils.js.map",
-        "\"use strict\";\n// *****************************************************************************\n//\n//   Part of the py5jupyter (& py5) library\n//   Copyright (C) 2022 Jim Schmitz\n//\n//   This library is free software: you can redistribute it and/or modify it\n//   under the terms of the GNU Lesser General Public License as published by\n//   the Free Software Foundation, either version 2.1 of the License, or (at\n//   your option) any later version.\n//\n//   This library is distributed in the hope that it will be useful, but\n//   WITHOUT ANY WARRANTY; without even the implied warranty of\n//   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser\n//   General Public License for more details.\n//\n//   You should have received a copy of the GNU Lesser General Public License\n//   along with this library. If not, see <https://www.gnu.org/licenses/>.\n//\n// *****************************************************************************\nObject.defineProperty(exports, \"__esModule\", { value: true });\nexports.MODULE_NAME = exports.MODULE_VERSION = void 0;\n// eslint-disable-next-line @typescript-eslint/ban-ts-comment\n// @ts-ignore\n// eslint-disable-next-line @typescript-eslint/no-var-requires\nconst data = require('../package.json');\n/**\n * The _model_module_version/_view_module_version this package implements.\n *\n * The html widget manager assumes that this is the same as the npm package\n * version number.\n */\nexports.MODULE_VERSION = data.version;\n/*\n * The current package name.\n */\nexports.MODULE_NAME = data.name;\n//# sourceMappingURL=version.js.map",
-        "\"use strict\";\nvar __awaiter = (this && this.__awaiter) || function (thisArg, _arguments, P, generator) {\n    function adopt(value) { return value instanceof P ? value : new P(function (resolve) { resolve(value); }); }\n    return new (P || (P = Promise))(function (resolve, reject) {\n        function fulfilled(value) { try { step(generator.next(value)); } catch (e) { reject(e); } }\n        function rejected(value) { try { step(generator[\"throw\"](value)); } catch (e) { reject(e); } }\n        function step(result) { result.done ? resolve(result.value) : adopt(result.value).then(fulfilled, rejected); }\n        step((generator = generator.apply(thisArg, _arguments || [])).next());\n    });\n};\nObject.defineProperty(exports, \"__esModule\", { value: true });\nexports.Py5SketchPortalView = exports.Py5SketchPortalModel = void 0;\n// *****************************************************************************\n//\n//   Part of the py5jupyter (& py5) library\n//   Copyright (C) 2022 Jim Schmitz\n//\n//   This library is free software: you can redistribute it and/or modify it\n//   under the terms of the GNU Lesser General Public License as published by\n//   the Free Software Foundation, either version 2.1 of the License, or (at\n//   your option) any later version.\n//\n//   This library is distributed in the hope that it will be useful, but\n//   WITHOUT ANY WARRANTY; without even the implied warranty of\n//   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser\n//   General Public License for more details.\n//\n//   You should have received a copy of the GNU Lesser General Public License\n//   along with this library. If not, see <https://www.gnu.org/licenses/>.\n//\n// *****************************************************************************\nconst base_1 = require(\"@jupyter-widgets/base\");\nconst version_1 = require(\"./version\");\nconst utils_1 = require(\"./utils\");\n// https://ipywidgets.readthedocs.io/en/latest/examples/Widget%20Low%20Level.html\nclass Py5SketchPortalModel extends base_1.DOMWidgetModel {\n    defaults() {\n        return Object.assign(Object.assign({}, super.defaults()), { _model_name: Py5SketchPortalModel.model_name, _model_module: Py5SketchPortalModel.model_module, _model_module_version: Py5SketchPortalModel.model_module_version, _view_name: Py5SketchPortalModel.view_name, _view_module: Py5SketchPortalModel.view_module, _view_module_version: Py5SketchPortalModel.view_module_version, width: '', height: '', value: new DataView(new ArrayBuffer(0)) });\n    }\n}\nexports.Py5SketchPortalModel = Py5SketchPortalModel;\nPy5SketchPortalModel.serializers = Object.assign(Object.assign({}, base_1.DOMWidgetModel.serializers), { value: {\n        serialize: (value) => {\n            return new DataView(value.buffer.slice(0));\n        },\n    } });\nPy5SketchPortalModel.model_name = 'Py5SketchPortalModel';\nPy5SketchPortalModel.model_module = version_1.MODULE_NAME;\nPy5SketchPortalModel.model_module_version = version_1.MODULE_VERSION;\nPy5SketchPortalModel.view_name = 'Py5SketchPortalView';\nPy5SketchPortalModel.view_module = version_1.MODULE_NAME;\nPy5SketchPortalModel.view_module_version = version_1.MODULE_VERSION;\nclass Py5SketchPortalView extends base_1.DOMWidgetView {\n    render() {\n        this._canvas = document.createElement('canvas');\n        this._canvas.width = this.model.get('width');\n        this._canvas.height = this.model.get('height');\n        this._canvas.tabIndex = 0;\n        const ctx = this._canvas.getContext('2d');\n        if (ctx === null) {\n            throw 'Could not create 2d context.';\n        }\n        else {\n            this._ctx = ctx;\n        }\n        this._updateImgSrc();\n        this.el.appendChild(this._canvas);\n        this._canvas.addEventListener('keydown', {\n            handleEvent: this.onKeyEvent.bind(this, 'key_down')\n        });\n        this._canvas.addEventListener('keypress', {\n            handleEvent: this.onKeyEvent.bind(this, 'key_press')\n        });\n        this._canvas.addEventListener('keyup', {\n            handleEvent: this.onKeyEvent.bind(this, 'key_up')\n        });\n        this._canvas.addEventListener('mouseenter', {\n            handleEvent: this.onMouseEvent.bind(this, 'mouse_enter')\n        });\n        this._canvas.addEventListener('mousedown', {\n            handleEvent: this.onMouseDown.bind(this)\n        });\n        this._canvas.addEventListener('mousemove', {\n            handleEvent: this.onMouseEvent.bind(this, 'mouse_move')\n        });\n        this._canvas.addEventListener('mouseup', {\n            handleEvent: this.onMouseEvent.bind(this, 'mouse_up')\n        });\n        this._canvas.addEventListener('mouseleave', {\n            handleEvent: this.onMouseEvent.bind(this, 'mouse_leave')\n        });\n        this._canvas.addEventListener('click', {\n            handleEvent: this.onMouseEvent.bind(this, 'mouse_click')\n        });\n        this._canvas.addEventListener('wheel', {\n            handleEvent: this.onMouseWheel.bind(this)\n        });\n        // Python -> JavaScript update\n        this.model.on('change:value', this._updateImgSrc, this);\n    }\n    _updateImgSrc() {\n        return __awaiter(this, void 0, void 0, function* () {\n            const img = yield utils_1.bufferToImage(this.model.get('value'));\n            this._ctx.drawImage(img, 0, 0);\n        });\n    }\n    // https://developer.mozilla.org/en-US/docs/Web/API/KeyboardEvent\n    onKeyEvent(event_name, event) {\n        this.model.send(Object.assign({ event: event_name, key: event.key, repeat: event.repeat }, this.getModifiers(event)), {});\n    }\n    onMouseEvent(event_name, event) {\n        this.model.send(Object.assign(Object.assign({ event: event_name, buttons: event.buttons }, this.getModifiers(event)), this.getCoordinates(event)), {});\n    }\n    onMouseDown(event) {\n        // Bring focus to the img element, so keyboard events can be triggered\n        this._canvas.focus();\n        this.model.send(Object.assign(Object.assign({ event: 'mouse_down', buttons: event.buttons }, this.getModifiers(event)), this.getCoordinates(event)), {});\n    }\n    // https://developer.mozilla.org/en-US/docs/Web/API/GlobalEventHandlers\n    onMouseWheel(event) {\n        this.model.send(Object.assign(Object.assign({ event: 'mouse_wheel', buttons: event.buttons, wheel: ((event.deltaY != 0) ? event.deltaY : event.deltaX) }, this.getModifiers(event)), this.getCoordinates(event)), {});\n    }\n    getCoordinates(event) {\n        // https://developer.mozilla.org/en-US/docs/Web/API/MouseEvent\n        const rect = this._canvas.getBoundingClientRect();\n        const x = (this._canvas.width * (event.clientX - rect.left)) / rect.width;\n        const y = (this._canvas.height * (event.clientY - rect.top)) / rect.height;\n        return { x, y };\n    }\n    getModifiers(event) {\n        return { mod: (+event.shiftKey) * 1 + (+event.ctrlKey) * 2 + (+event.metaKey) * 4 + (+event.altKey) * 8 };\n    }\n}\nexports.Py5SketchPortalView = Py5SketchPortalView;\n//# sourceMappingURL=widget.js.map"
+        "\"use strict\";\n// *****************************************************************************\n//\n//   Part of the py5jupyter (& py5) library\n//   Copyright (C) 2022-2023 Jim Schmitz\n//\n//   This library is free software: you can redistribute it and/or modify it\n//   under the terms of the GNU Lesser General Public License as published by\n//   the Free Software Foundation, either version 2.1 of the License, or (at\n//   your option) any later version.\n//\n//   This library is distributed in the hope that it will be useful, but\n//   WITHOUT ANY WARRANTY; without even the implied warranty of\n//   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser\n//   General Public License for more details.\n//\n//   You should have received a copy of the GNU Lesser General Public License\n//   along with this library. If not, see <https://www.gnu.org/licenses/>.\n//\n// *****************************************************************************\nvar __awaiter = (this && this.__awaiter) || function (thisArg, _arguments, P, generator) {\n    function adopt(value) { return value instanceof P ? value : new P(function (resolve) { resolve(value); }); }\n    return new (P || (P = Promise))(function (resolve, reject) {\n        function fulfilled(value) { try { step(generator.next(value)); } catch (e) { reject(e); } }\n        function rejected(value) { try { step(generator[\"throw\"](value)); } catch (e) { reject(e); } }\n        function step(result) { result.done ? resolve(result.value) : adopt(result.value).then(fulfilled, rejected); }\n        step((generator = generator.apply(thisArg, _arguments || [])).next());\n    });\n};\nObject.defineProperty(exports, \"__esModule\", { value: true });\nexports.bufferToImage = void 0;\n// The below function came from the wonderful Python library ipycanvas\n// https://github.com/martinRenou/ipycanvas\nfunction bufferToImage(buffer) {\n    return __awaiter(this, void 0, void 0, function* () {\n        let url;\n        const blob = new Blob([buffer], { type: 'image/jpeg' });\n        url = URL.createObjectURL(blob);\n        const img = new Image();\n        return new Promise(resolve => {\n            img.onload = () => {\n                resolve(img);\n            };\n            img.src = url;\n        });\n    });\n}\nexports.bufferToImage = bufferToImage;\n//# sourceMappingURL=utils.js.map",
+        "\"use strict\";\n// *****************************************************************************\n//\n//   Part of the py5jupyter (& py5) library\n//   Copyright (C) 2022-2023 Jim Schmitz\n//\n//   This library is free software: you can redistribute it and/or modify it\n//   under the terms of the GNU Lesser General Public License as published by\n//   the Free Software Foundation, either version 2.1 of the License, or (at\n//   your option) any later version.\n//\n//   This library is distributed in the hope that it will be useful, but\n//   WITHOUT ANY WARRANTY; without even the implied warranty of\n//   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser\n//   General Public License for more details.\n//\n//   You should have received a copy of the GNU Lesser General Public License\n//   along with this library. If not, see <https://www.gnu.org/licenses/>.\n//\n// *****************************************************************************\nObject.defineProperty(exports, \"__esModule\", { value: true });\nexports.MODULE_NAME = exports.MODULE_VERSION = void 0;\n// eslint-disable-next-line @typescript-eslint/ban-ts-comment\n// @ts-ignore\n// eslint-disable-next-line @typescript-eslint/no-var-requires\nconst data = require('../package.json');\n/**\n * The _model_module_version/_view_module_version this package implements.\n *\n * The html widget manager assumes that this is the same as the npm package\n * version number.\n */\nexports.MODULE_VERSION = data.version;\n/*\n * The current package name.\n */\nexports.MODULE_NAME = data.name;\n//# sourceMappingURL=version.js.map",
+        "\"use strict\";\nvar __awaiter = (this && this.__awaiter) || function (thisArg, _arguments, P, generator) {\n    function adopt(value) { return value instanceof P ? value : new P(function (resolve) { resolve(value); }); }\n    return new (P || (P = Promise))(function (resolve, reject) {\n        function fulfilled(value) { try { step(generator.next(value)); } catch (e) { reject(e); } }\n        function rejected(value) { try { step(generator[\"throw\"](value)); } catch (e) { reject(e); } }\n        function step(result) { result.done ? resolve(result.value) : adopt(result.value).then(fulfilled, rejected); }\n        step((generator = generator.apply(thisArg, _arguments || [])).next());\n    });\n};\nObject.defineProperty(exports, \"__esModule\", { value: true });\nexports.Py5SketchPortalView = exports.Py5SketchPortalModel = void 0;\n// *****************************************************************************\n//\n//   Part of the py5jupyter (& py5) library\n//   Copyright (C) 2022-2023 Jim Schmitz\n//\n//   This library is free software: you can redistribute it and/or modify it\n//   under the terms of the GNU Lesser General Public License as published by\n//   the Free Software Foundation, either version 2.1 of the License, or (at\n//   your option) any later version.\n//\n//   This library is distributed in the hope that it will be useful, but\n//   WITHOUT ANY WARRANTY; without even the implied warranty of\n//   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser\n//   General Public License for more details.\n//\n//   You should have received a copy of the GNU Lesser General Public License\n//   along with this library. If not, see <https://www.gnu.org/licenses/>.\n//\n// *****************************************************************************\nconst base_1 = require(\"@jupyter-widgets/base\");\nconst version_1 = require(\"./version\");\nconst utils_1 = require(\"./utils\");\n// https://ipywidgets.readthedocs.io/en/latest/examples/Widget%20Low%20Level.html\nclass Py5SketchPortalModel extends base_1.DOMWidgetModel {\n    defaults() {\n        return Object.assign(Object.assign({}, super.defaults()), { _model_name: Py5SketchPortalModel.model_name, _model_module: Py5SketchPortalModel.model_module, _model_module_version: Py5SketchPortalModel.model_module_version, _view_name: Py5SketchPortalModel.view_name, _view_module: Py5SketchPortalModel.view_module, _view_module_version: Py5SketchPortalModel.view_module_version, width: '', height: '', value: new DataView(new ArrayBuffer(0)) });\n    }\n}\nexports.Py5SketchPortalModel = Py5SketchPortalModel;\nPy5SketchPortalModel.serializers = Object.assign(Object.assign({}, base_1.DOMWidgetModel.serializers), { value: {\n        serialize: (value) => {\n            return new DataView(value.buffer.slice(0));\n        },\n    } });\nPy5SketchPortalModel.model_name = 'Py5SketchPortalModel';\nPy5SketchPortalModel.model_module = version_1.MODULE_NAME;\nPy5SketchPortalModel.model_module_version = version_1.MODULE_VERSION;\nPy5SketchPortalModel.view_name = 'Py5SketchPortalView';\nPy5SketchPortalModel.view_module = version_1.MODULE_NAME;\nPy5SketchPortalModel.view_module_version = version_1.MODULE_VERSION;\nclass Py5SketchPortalView extends base_1.DOMWidgetView {\n    render() {\n        this._canvas = document.createElement('canvas');\n        this._canvas.width = this.model.get('width');\n        this._canvas.height = this.model.get('height');\n        this._canvas.tabIndex = 0;\n        const ctx = this._canvas.getContext('2d');\n        if (ctx === null) {\n            throw 'Could not create 2d context.';\n        }\n        else {\n            this._ctx = ctx;\n        }\n        this._updateImgSrc();\n        this.el.appendChild(this._canvas);\n        this._canvas.addEventListener('keydown', {\n            handleEvent: this.onKeyEvent.bind(this, 'key_down')\n        });\n        this._canvas.addEventListener('keypress', {\n            handleEvent: this.onKeyEvent.bind(this, 'key_press')\n        });\n        this._canvas.addEventListener('keyup', {\n            handleEvent: this.onKeyEvent.bind(this, 'key_up')\n        });\n        this._canvas.addEventListener('mouseenter', {\n            handleEvent: this.onMouseEvent.bind(this, 'mouse_enter')\n        });\n        this._canvas.addEventListener('mousedown', {\n            handleEvent: this.onMouseDown.bind(this)\n        });\n        this._canvas.addEventListener('mousemove', {\n            handleEvent: this.onMouseEvent.bind(this, 'mouse_move')\n        });\n        this._canvas.addEventListener('mouseup', {\n            handleEvent: this.onMouseEvent.bind(this, 'mouse_up')\n        });\n        this._canvas.addEventListener('mouseleave', {\n            handleEvent: this.onMouseEvent.bind(this, 'mouse_leave')\n        });\n        this._canvas.addEventListener('click', {\n            handleEvent: this.onMouseEvent.bind(this, 'mouse_click')\n        });\n        this._canvas.addEventListener('wheel', {\n            handleEvent: this.onMouseWheel.bind(this)\n        });\n        // Python -> JavaScript update\n        this.model.on('change:value', this._updateImgSrc, this);\n    }\n    _updateImgSrc() {\n        return __awaiter(this, void 0, void 0, function* () {\n            const img = yield utils_1.bufferToImage(this.model.get('value'));\n            this._ctx.drawImage(img, 0, 0);\n        });\n    }\n    // https://developer.mozilla.org/en-US/docs/Web/API/KeyboardEvent\n    onKeyEvent(event_name, event) {\n        this.model.send(Object.assign({ event: event_name, key: event.key, repeat: event.repeat }, this.getModifiers(event)), {});\n    }\n    onMouseEvent(event_name, event) {\n        this.model.send(Object.assign(Object.assign({ event: event_name, buttons: event.buttons }, this.getModifiers(event)), this.getCoordinates(event)), {});\n    }\n    onMouseDown(event) {\n        // Bring focus to the img element, so keyboard events can be triggered\n        this._canvas.focus();\n        this.model.send(Object.assign(Object.assign({ event: 'mouse_down', buttons: event.buttons }, this.getModifiers(event)), this.getCoordinates(event)), {});\n    }\n    // https://developer.mozilla.org/en-US/docs/Web/API/GlobalEventHandlers\n    onMouseWheel(event) {\n        this.model.send(Object.assign(Object.assign({ event: 'mouse_wheel', buttons: event.buttons, wheel: ((event.deltaY != 0) ? event.deltaY : event.deltaX) }, this.getModifiers(event)), this.getCoordinates(event)), {});\n    }\n    getCoordinates(event) {\n        // https://developer.mozilla.org/en-US/docs/Web/API/MouseEvent\n        const rect = this._canvas.getBoundingClientRect();\n        const x = (this._canvas.width * (event.clientX - rect.left)) / rect.width;\n        const y = (this._canvas.height * (event.clientY - rect.top)) / rect.height;\n        return { x, y };\n    }\n    getModifiers(event) {\n        return { mod: (+event.shiftKey) * 1 + (+event.ctrlKey) * 2 + (+event.metaKey) * 4 + (+event.altKey) * 8 };\n    }\n}\nexports.Py5SketchPortalView = Py5SketchPortalView;\n//# sourceMappingURL=widget.js.map"
     ],
     "version": 3
 }
```

### Comparing `py5jupyter-0.1.2a1/py5jupyter/labextension/static/remoteEntry.042026d6e03651ecc3fd.js` & `py5jupyter-0.2.0a0/py5jupyter/labextension/static/remoteEntry.102c2185a6a3be91ce3c.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -154,16 +154,16 @@
     (() => {
         /******/ // This function allow to reference async chunks
         /******/
         __webpack_require__.u = (chunkId) => {
             /******/ // return url for filenames based on template
             /******/
             return "" + chunkId + "." + {
-                "lib_widget_js": "d141153e6400998a12a2",
-                "lib_index_js": "488a66c2de85320bc65a",
+                "lib_widget_js": "fc065f743fb92e735a68",
+                "lib_index_js": "b65cf7c58127bf49a498",
                 "lib_plugin_js": "586e3941dfcc287e7351"
             } [chunkId] + ".js";
             /******/
         };
         /******/
     })();
     /******/
@@ -1001,8 +1001,8 @@
     /******/
     var __webpack_exports__ = __webpack_require__("webpack/container/entry/jupyter-py5");
     /******/
     (_JUPYTERLAB = typeof _JUPYTERLAB === "undefined" ? {} : _JUPYTERLAB)["jupyter-py5"] = __webpack_exports__;
     /******/
     /******/
 })();
-//# sourceMappingURL=remoteEntry.042026d6e03651ecc3fd.js.map
+//# sourceMappingURL=remoteEntry.102c2185a6a3be91ce3c.js.map
```

### Comparing `py5jupyter-0.1.2a1/py5jupyter/labextension/static/remoteEntry.042026d6e03651ecc3fd.js.map` & `py5jupyter-0.2.0a0/py5jupyter/labextension/static/remoteEntry.102c2185a6a3be91ce3c.js.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9196428571428571%*

 * *Differences: {"'file'": "'remoteEntry.102c2185a6a3be91ce3c.js'",*

 * * "'sourcesContent'": "{insert: [(4, '// This function allow to reference async "*

 * *                     'chunks\\n__webpack_require__.u = (chunkId) => {\\n\\t// return url for '*

 * *                     'filenames based on template\\n\\treturn "" + chunkId + "." + '*

 * *                     '{"lib_widget_js":"fc065f743fb92e735a68","lib_index_js":"b65cf7c58127bf49a498","lib_plugin_js":"586e3941dfcc287e7351"}[chunkId] '*

 * *                     '+ ".js";\\n};\')], delete: […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "file": "remoteEntry.042026d6e03651ecc3fd.js",
+    "file": "remoteEntry.102c2185a6a3be91ce3c.js",
     "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCjCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,oHAAoH;WAClJ;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCzCA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC3CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WCfA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB,GAAG;WACH;WACA;;;;;WCvKA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL,eAAe;WACf;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;UErFA;UACA;UACA;UACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://jupyter-py5/webpack/container-entry",
         "webpack://jupyter-py5/webpack/bootstrap",
         "webpack://jupyter-py5/webpack/runtime/define property getters",
@@ -21,15 +21,15 @@
         "webpack://jupyter-py5/webpack/after-startup"
     ],
     "sourcesContent": [
         "var moduleMap = {\n\t\"./index\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"lib_widget_js\"), __webpack_require__.e(\"lib_index_js\")]).then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./extension\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"lib_widget_js\"), __webpack_require__.e(\"lib_plugin_js\")]).then(() => (() => ((__webpack_require__(/*! ./lib/plugin */ \"./lib/plugin.js\")))));\n\t}\n};\nvar get = (module, getScope) => {\n\t__webpack_require__.R = getScope;\n\tgetScope = (\n\t\t__webpack_require__.o(moduleMap, module)\n\t\t\t? moduleMap[module]()\n\t\t\t: Promise.resolve().then(() => {\n\t\t\t\tthrow new Error('Module \"' + module + '\" does not exist in container.');\n\t\t\t})\n\t);\n\t__webpack_require__.R = undefined;\n\treturn getScope;\n};\nvar init = (shareScope, initScope) => {\n\tif (!__webpack_require__.S) return;\n\tvar name = \"default\"\n\tvar oldScope = __webpack_require__.S[name];\n\tif(oldScope && oldScope !== shareScope) throw new Error(\"Container initialization failed as it has already been initialized with a different share scope\");\n\t__webpack_require__.S[name] = shareScope;\n\treturn __webpack_require__.I(name, initScope);\n};\n\n// This exports getters to disallow modifications\n__webpack_require__.d(exports, {\n\tget: () => (get),\n\tinit: () => (init)\n});",
         "// The module cache\nvar __webpack_module_cache__ = {};\n\n// The require function\nfunction __webpack_require__(moduleId) {\n\t// Check if module is in cache\n\tvar cachedModule = __webpack_module_cache__[moduleId];\n\tif (cachedModule !== undefined) {\n\t\treturn cachedModule.exports;\n\t}\n\t// Create a new module (and put it into the cache)\n\tvar module = __webpack_module_cache__[moduleId] = {\n\t\t// no module.id needed\n\t\t// no module.loaded needed\n\t\texports: {}\n\t};\n\n\t// Execute the module function\n\t__webpack_modules__[moduleId].call(module.exports, module, module.exports, __webpack_require__);\n\n\t// Return the exports of the module\n\treturn module.exports;\n}\n\n// expose the modules object (__webpack_modules__)\n__webpack_require__.m = __webpack_modules__;\n\n// expose the module cache\n__webpack_require__.c = __webpack_module_cache__;\n\n",
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
-        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"lib_widget_js\":\"d141153e6400998a12a2\",\"lib_index_js\":\"488a66c2de85320bc65a\",\"lib_plugin_js\":\"586e3941dfcc287e7351\"}[chunkId] + \".js\";\n};",
+        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"lib_widget_js\":\"fc065f743fb92e735a68\",\"lib_index_js\":\"b65cf7c58127bf49a498\",\"lib_plugin_js\":\"586e3941dfcc287e7351\"}[chunkId] + \".js\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "var inProgress = {};\nvar dataWebpackPrefix = \"jupyter-py5:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t}\n\t;\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
         "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => (typeof console !== \"undefined\" && console.warn && console.warn(msg));\n\tvar uniqueName = \"jupyter-py5\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"jupyter-py5\", \"0.1.0\", () => (Promise.all([__webpack_require__.e(\"lib_widget_js\"), __webpack_require__.e(\"lib_index_js\")]).then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
         "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) scriptUrl = scripts[scripts.length - 1].src\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
         "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) typeof console !== \"undefined\" && console.warn && console.warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\ttypeof console !== \"undefined\" && console.warn && console.warn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyter-widgets/base\": () => (loadSingletonVersionCheck(\"default\", \"@jupyter-widgets/base\", [,[1,4,0,0],[1,3,0,0],[1,2,0,0],[1,1,1,10],1,1,1]))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_widget_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyter-widgets/base\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
         "// no baseURI\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t\"jupyter-py5\": 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(true) { // all chunks have JS\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t} else installedChunks[chunkId] = 0;\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunkjupyter_py5\"] = self[\"webpackChunkjupyter_py5\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
```

### Comparing `py5jupyter-0.1.2a1/py5jupyter/tests/conftest.py` & `py5jupyter-0.2.0a0/py5jupyter/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `py5jupyter-0.1.2a1/py5jupyter/widgets/__init__.py` & `py5jupyter-0.2.0a0/src/version.ts`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,37 @@
-# *****************************************************************************
-#
-#   Part of the py5jupyter (& py5) library
-#   Copyright (C) 2022 Jim Schmitz
-#
-#   This library is free software: you can redistribute it and/or modify it
-#   under the terms of the GNU Lesser General Public License as published by
-#   the Free Software Foundation, either version 2.1 of the License, or (at
-#   your option) any later version.
-#
-#   This library is distributed in the hope that it will be useful, but
-#   WITHOUT ANY WARRANTY; without even the implied warranty of
-#   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser
-#   General Public License for more details.
-#
-#   You should have received a copy of the GNU Lesser General Public License
-#   along with this library. If not, see <https://www.gnu.org/licenses/>.
-#
-# *****************************************************************************
-from .sketchportal import Py5SketchPortal
+// *****************************************************************************
+//
+//   Part of the py5jupyter (& py5) library
+//   Copyright (C) 2022-2023 Jim Schmitz
+//
+//   This library is free software: you can redistribute it and/or modify it
+//   under the terms of the GNU Lesser General Public License as published by
+//   the Free Software Foundation, either version 2.1 of the License, or (at
+//   your option) any later version.
+//
+//   This library is distributed in the hope that it will be useful, but
+//   WITHOUT ANY WARRANTY; without even the implied warranty of
+//   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser
+//   General Public License for more details.
+//
+//   You should have received a copy of the GNU Lesser General Public License
+//   along with this library. If not, see <https://www.gnu.org/licenses/>.
+//
+// *****************************************************************************
+
+// eslint-disable-next-line @typescript-eslint/ban-ts-comment
+// @ts-ignore
+// eslint-disable-next-line @typescript-eslint/no-var-requires
+const data = require('../package.json');
+
+/**
+ * The _model_module_version/_view_module_version this package implements.
+ *
+ * The html widget manager assumes that this is the same as the npm package
+ * version number.
+ */
+export const MODULE_VERSION = data.version;
+
+/*
+ * The current package name.
+ */
+export const MODULE_NAME = data.name;
```

### Comparing `py5jupyter-0.1.2a1/py5jupyter/widgets/_frontend.py` & `py5jupyter-0.2.0a0/py5jupyter/widgets/_frontend.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # *****************************************************************************
 #
 #   Part of the py5jupyter (& py5) library
-#   Copyright (C) 2022 Jim Schmitz
+#   Copyright (C) 2022-2023 Jim Schmitz
 #
 #   This library is free software: you can redistribute it and/or modify it
 #   under the terms of the GNU Lesser General Public License as published by
 #   the Free Software Foundation, either version 2.1 of the License, or (at
 #   your option) any later version.
 #
 #   This library is distributed in the hope that it will be useful, but
@@ -14,8 +14,8 @@
 #   General Public License for more details.
 #
 #   You should have received a copy of the GNU Lesser General Public License
 #   along with this library. If not, see <https://www.gnu.org/licenses/>.
 #
 # *****************************************************************************
 module_name = "jupyter-py5"
-module_version = "^0.1.0"
+module_version = "^0.2.0"
```

### Comparing `py5jupyter-0.1.2a1/py5jupyter/widgets/sketchportal.py` & `py5jupyter-0.2.0a0/py5jupyter/widgets/sketchportal.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # *****************************************************************************
 #
 #   Part of the py5jupyter (& py5) library
-#   Copyright (C) 2022 Jim Schmitz
+#   Copyright (C) 2022-2023 Jim Schmitz
 #
 #   This library is free software: you can redistribute it and/or modify it
 #   under the terms of the GNU Lesser General Public License as published by
 #   the Free Sotware Foundation, either version 2.1 of the License, or (at
 #   your option) any later version.
 #
 #   This library is distributed in the hope that it will be useful, but
```

### Comparing `py5jupyter-0.1.2a1/src/__tests__/index.spec.ts` & `py5jupyter-0.2.0a0/src/__tests__/index.spec.ts`

 * *Files identical despite different names*

### Comparing `py5jupyter-0.1.2a1/src/__tests__/utils.ts` & `py5jupyter-0.2.0a0/src/__tests__/utils.ts`

 * *Files identical despite different names*

### Comparing `py5jupyter-0.1.2a1/src/extension.ts` & `py5jupyter-0.2.0a0/src/extension.ts`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 // *****************************************************************************
 //
 //   Part of the py5jupyter (& py5) library
-//   Copyright (C) 2022 Jim Schmitz
+//   Copyright (C) 2022-2023 Jim Schmitz
 //
 //   This library is free software: you can redistribute it and/or modify it
 //   under the terms of the GNU Lesser General Public License as published by
 //   the Free Software Foundation, either version 2.1 of the License, or (at
 //   your option) any later version.
 //
 //   This library is distributed in the hope that it will be useful, but
```

### Comparing `py5jupyter-0.1.2a1/src/index.ts` & `py5jupyter-0.2.0a0/src/index.ts`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 // *****************************************************************************
 //
 //   Part of the py5jupyter (& py5) library
-//   Copyright (C) 2022 Jim Schmitz
+//   Copyright (C) 2022-2023 Jim Schmitz
 //
 //   This library is free software: you can redistribute it and/or modify it
 //   under the terms of the GNU Lesser General Public License as published by
 //   the Free Software Foundation, either version 2.1 of the License, or (at
 //   your option) any later version.
 //
 //   This library is distributed in the hope that it will be useful, but
```

### Comparing `py5jupyter-0.1.2a1/src/plugin.ts` & `py5jupyter-0.2.0a0/src/plugin.ts`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 // *****************************************************************************
 //
 //   Part of the py5jupyter (& py5) library
-//   Copyright (C) 2022 Jim Schmitz
+//   Copyright (C) 2022-2023 Jim Schmitz
 //
 //   This library is free software: you can redistribute it and/or modify it
 //   under the terms of the GNU Lesser General Public License as published by
 //   the Free Software Foundation, either version 2.1 of the License, or (at
 //   your option) any later version.
 //
 //   This library is distributed in the hope that it will be useful, but
```

### Comparing `py5jupyter-0.1.2a1/src/utils.ts` & `py5jupyter-0.2.0a0/src/utils.ts`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 // *****************************************************************************
 //
 //   Part of the py5jupyter (& py5) library
-//   Copyright (C) 2022 Jim Schmitz
+//   Copyright (C) 2022-2023 Jim Schmitz
 //
 //   This library is free software: you can redistribute it and/or modify it
 //   under the terms of the GNU Lesser General Public License as published by
 //   the Free Software Foundation, either version 2.1 of the License, or (at
 //   your option) any later version.
 //
 //   This library is distributed in the hope that it will be useful, but
```

### Comparing `py5jupyter-0.1.2a1/src/widget.ts` & `py5jupyter-0.2.0a0/src/widget.ts`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 // *****************************************************************************
 //
 //   Part of the py5jupyter (& py5) library
-//   Copyright (C) 2022 Jim Schmitz
+//   Copyright (C) 2022-2023 Jim Schmitz
 //
 //   This library is free software: you can redistribute it and/or modify it
 //   under the terms of the GNU Lesser General Public License as published by
 //   the Free Software Foundation, either version 2.1 of the License, or (at
 //   your option) any later version.
 //
 //   This library is distributed in the hope that it will be useful, but
```

### Comparing `py5jupyter-0.1.2a1/tsconfig.json` & `py5jupyter-0.2.0a0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `py5jupyter-0.1.2a1/webpack.config.js` & `py5jupyter-0.2.0a0/webpack.config.js`

 * *Files identical despite different names*

