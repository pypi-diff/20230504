# Comparing `tmp/yaecs-3.2.3.tar.gz` & `tmp/yaecs-3.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaecs-3.2.3.tar", last modified: Wed May  3 12:04:15 2023, max compression
+gzip compressed data, was "yaecs-3.2.4.tar", last modified: Thu May  4 11:44:51 2023, max compression
```

## Comparing `yaecs-3.2.3.tar` & `yaecs-3.2.4.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:04:15.800347 yaecs-3.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-03 12:03:52.000000 yaecs-3.2.3/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:04:15.792347 yaecs-3.2.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:04:15.796347 yaecs-3.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-03 12:03:52.000000 yaecs-3.2.3/.github/workflows/pipy_deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-05-03 12:03:52.000000 yaecs-3.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    20869 2023-05-03 12:03:52.000000 yaecs-3.2.3/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-05-03 12:03:52.000000 yaecs-3.2.3/COPYING.LESSER.md
--rw-r--r--   0 runner    (1001) docker     (123)    34915 2023-05-03 12:03:52.000000 yaecs-3.2.3/COPYING.md
--rw-r--r--   0 runner    (1001) docker     (123)    78683 2023-05-03 12:03:52.000000 yaecs-3.2.3/DOCUMENTATION_WIP.md
--rw-r--r--   0 runner    (1001) docker     (123)    34915 2023-05-03 12:03:52.000000 yaecs-3.2.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-03 12:03:52.000000 yaecs-3.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-05-03 12:04:15.800347 yaecs-3.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-05-03 12:03:52.000000 yaecs-3.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-03 12:03:52.000000 yaecs-3.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-03 12:03:52.000000 yaecs-3.2.3/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:04:15.796347 yaecs-3.2.3/resources/
--rw-r--r--   0 runner    (1001) docker     (123)   175062 2023-05-03 12:03:52.000000 yaecs-3.2.3/resources/yaecs_constructor_overview.png
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 12:04:15.800347 yaecs-3.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-03 12:03:52.000000 yaecs-3.2.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-05-03 12:03:52.000000 yaecs-3.2.3/short-readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:04:15.792347 yaecs-3.2.3/unittests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:04:15.796347 yaecs-3.2.3/unittests/config/
--rw-r--r--   0 runner    (1001) docker     (123)    10329 2023-05-03 12:03:52.000000 yaecs-3.2.3/unittests/config/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    36401 2023-05-03 12:03:52.000000 yaecs-3.2.3/unittests/config/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-05-03 12:03:52.000000 yaecs-3.2.3/unittests/config/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:04:15.796347 yaecs-3.2.3/usage_example/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-03 12:03:52.000000 yaecs-3.2.3/usage_example/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-03 12:03:52.000000 yaecs-3.2.3/usage_example/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:04:15.796347 yaecs-3.2.3/usage_example/configs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:04:15.796347 yaecs-3.2.3/usage_example/configs/default/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-03 12:03:52.000000 yaecs-3.2.3/usage_example/configs/default/data_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-03 12:03:52.000000 yaecs-3.2.3/usage_example/configs/default/main_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-03 12:03:52.000000 yaecs-3.2.3/usage_example/configs/default/model_config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:04:15.796347 yaecs-3.2.3/usage_example/configs/experiment/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-03 12:03:52.000000 yaecs-3.2.3/usage_example/configs/experiment/dummy_test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-03 12:03:52.000000 yaecs-3.2.3/usage_example/configs/experiment/grid_search.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-03 12:03:52.000000 yaecs-3.2.3/usage_example/configs/experiment/random_search.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-03 12:03:52.000000 yaecs-3.2.3/usage_example/configs/project_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10563 2023-05-03 12:03:52.000000 yaecs-3.2.3/usage_example/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:04:15.796347 yaecs-3.2.3/usage_example/project_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-03 12:03:52.000000 yaecs-3.2.3/usage_example/project_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:04:15.796347 yaecs-3.2.3/yaecs/
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-05-03 12:03:52.000000 yaecs-3.2.3/yaecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-03 12:04:15.000000 yaecs-3.2.3/yaecs/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:04:15.800347 yaecs-3.2.3/yaecs/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 12:03:52.000000 yaecs-3.2.3/yaecs/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24515 2023-05-03 12:03:52.000000 yaecs-3.2.3/yaecs/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    47630 2023-05-03 12:03:52.000000 yaecs-3.2.3/yaecs/config/config_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17249 2023-05-03 12:03:52.000000 yaecs-3.2.3/yaecs/config/config_convenience.py
--rw-r--r--   0 runner    (1001) docker     (123)    13615 2023-05-03 12:03:52.000000 yaecs-3.2.3/yaecs/config/config_getters.py
--rw-r--r--   0 runner    (1001) docker     (123)    14876 2023-05-03 12:03:52.000000 yaecs-3.2.3/yaecs/config/config_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    10859 2023-05-03 12:03:52.000000 yaecs-3.2.3/yaecs/config/config_processing_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-05-03 12:03:52.000000 yaecs-3.2.3/yaecs/config/config_setters.py
--rw-r--r--   0 runner    (1001) docker     (123)    24448 2023-05-03 12:03:52.000000 yaecs-3.2.3/yaecs/config_history.py
--rw-r--r--   0 runner    (1001) docker     (123)    33455 2023-05-03 12:03:52.000000 yaecs-3.2.3/yaecs/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-05-03 12:03:52.000000 yaecs-3.2.3/yaecs/pytorch_lightning_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10315 2023-05-03 12:03:52.000000 yaecs-3.2.3/yaecs/user_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    35179 2023-05-03 12:03:52.000000 yaecs-3.2.3/yaecs/yaecs_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:04:15.796347 yaecs-3.2.3/yaecs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-05-03 12:04:15.000000 yaecs-3.2.3/yaecs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-03 12:04:15.000000 yaecs-3.2.3/yaecs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 12:04:15.000000 yaecs-3.2.3/yaecs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-03 12:04:15.000000 yaecs-3.2.3/yaecs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-03 12:04:15.000000 yaecs-3.2.3/yaecs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:44:51.226376 yaecs-3.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-04 11:44:33.000000 yaecs-3.2.4/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:44:51.218376 yaecs-3.2.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:44:51.222376 yaecs-3.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-04 11:44:33.000000 yaecs-3.2.4/.github/workflows/pipy_deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-05-04 11:44:33.000000 yaecs-3.2.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    20869 2023-05-04 11:44:33.000000 yaecs-3.2.4/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-05-04 11:44:33.000000 yaecs-3.2.4/COPYING.LESSER.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34915 2023-05-04 11:44:33.000000 yaecs-3.2.4/COPYING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    78683 2023-05-04 11:44:33.000000 yaecs-3.2.4/DOCUMENTATION_WIP.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34915 2023-05-04 11:44:33.000000 yaecs-3.2.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-04 11:44:33.000000 yaecs-3.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-05-04 11:44:51.226376 yaecs-3.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-05-04 11:44:33.000000 yaecs-3.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-04 11:44:33.000000 yaecs-3.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-04 11:44:33.000000 yaecs-3.2.4/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:44:51.222376 yaecs-3.2.4/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)   175062 2023-05-04 11:44:33.000000 yaecs-3.2.4/resources/yaecs_constructor_overview.png
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 11:44:51.226376 yaecs-3.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-04 11:44:33.000000 yaecs-3.2.4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-05-04 11:44:33.000000 yaecs-3.2.4/short-readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:44:51.218376 yaecs-3.2.4/unittests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:44:51.222376 yaecs-3.2.4/unittests/config/
+-rw-r--r--   0 runner    (1001) docker     (123)    10329 2023-05-04 11:44:33.000000 yaecs-3.2.4/unittests/config/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36401 2023-05-04 11:44:33.000000 yaecs-3.2.4/unittests/config/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-05-04 11:44:33.000000 yaecs-3.2.4/unittests/config/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:44:51.222376 yaecs-3.2.4/usage_example/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-04 11:44:33.000000 yaecs-3.2.4/usage_example/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-04 11:44:33.000000 yaecs-3.2.4/usage_example/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:44:51.222376 yaecs-3.2.4/usage_example/configs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:44:51.222376 yaecs-3.2.4/usage_example/configs/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-04 11:44:33.000000 yaecs-3.2.4/usage_example/configs/default/data_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-04 11:44:33.000000 yaecs-3.2.4/usage_example/configs/default/main_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-04 11:44:33.000000 yaecs-3.2.4/usage_example/configs/default/model_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:44:51.222376 yaecs-3.2.4/usage_example/configs/experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-04 11:44:33.000000 yaecs-3.2.4/usage_example/configs/experiment/dummy_test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-04 11:44:33.000000 yaecs-3.2.4/usage_example/configs/experiment/grid_search.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-04 11:44:33.000000 yaecs-3.2.4/usage_example/configs/experiment/random_search.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-04 11:44:33.000000 yaecs-3.2.4/usage_example/configs/project_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10563 2023-05-04 11:44:33.000000 yaecs-3.2.4/usage_example/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:44:51.222376 yaecs-3.2.4/usage_example/project_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-04 11:44:33.000000 yaecs-3.2.4/usage_example/project_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:44:51.226376 yaecs-3.2.4/yaecs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-05-04 11:44:33.000000 yaecs-3.2.4/yaecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-04 11:44:51.000000 yaecs-3.2.4/yaecs/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:44:51.226376 yaecs-3.2.4/yaecs/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:44:33.000000 yaecs-3.2.4/yaecs/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24515 2023-05-04 11:44:33.000000 yaecs-3.2.4/yaecs/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47611 2023-05-04 11:44:33.000000 yaecs-3.2.4/yaecs/config/config_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17271 2023-05-04 11:44:33.000000 yaecs-3.2.4/yaecs/config/config_convenience.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13615 2023-05-04 11:44:33.000000 yaecs-3.2.4/yaecs/config/config_getters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14876 2023-05-04 11:44:33.000000 yaecs-3.2.4/yaecs/config/config_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10918 2023-05-04 11:44:33.000000 yaecs-3.2.4/yaecs/config/config_processing_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-05-04 11:44:33.000000 yaecs-3.2.4/yaecs/config/config_setters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24448 2023-05-04 11:44:33.000000 yaecs-3.2.4/yaecs/config_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33455 2023-05-04 11:44:33.000000 yaecs-3.2.4/yaecs/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-05-04 11:44:33.000000 yaecs-3.2.4/yaecs/pytorch_lightning_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10315 2023-05-04 11:44:33.000000 yaecs-3.2.4/yaecs/user_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35179 2023-05-04 11:44:33.000000 yaecs-3.2.4/yaecs/yaecs_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:44:51.226376 yaecs-3.2.4/yaecs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-05-04 11:44:51.000000 yaecs-3.2.4/yaecs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-04 11:44:51.000000 yaecs-3.2.4/yaecs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 11:44:51.000000 yaecs-3.2.4/yaecs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-04 11:44:51.000000 yaecs-3.2.4/yaecs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-04 11:44:51.000000 yaecs-3.2.4/yaecs.egg-info/top_level.txt
```

### Comparing `yaecs-3.2.3/.github/workflows/pipy_deployment.yaml` & `yaecs-3.2.4/.github/workflows/pipy_deployment.yaml`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.3/.gitignore` & `yaecs-3.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.3/.pylintrc` & `yaecs-3.2.4/.pylintrc`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.3/COPYING.LESSER.md` & `yaecs-3.2.4/COPYING.LESSER.md`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.3/COPYING.md` & `yaecs-3.2.4/COPYING.md`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.3/DOCUMENTATION_WIP.md` & `yaecs-3.2.4/DOCUMENTATION_WIP.md`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.3/LICENSE.md` & `yaecs-3.2.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.3/PKG-INFO` & `yaecs-3.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaecs
-Version: 3.2.3
+Version: 3.2.4
 Summary: A Config System designed for experimental purposes
 Author: Reactive Reality AG
 Project-URL: Source, https://gitlab.com/reactivereality/public/yaecs
 Keywords: template,machine,learning
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `yaecs-3.2.3/README.md` & `yaecs-3.2.4/README.md`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.3/pyproject.toml` & `yaecs-3.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.3/resources/yaecs_constructor_overview.png` & `yaecs-3.2.4/resources/yaecs_constructor_overview.png`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.3/setup.py` & `yaecs-3.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.3/short-readme.md` & `yaecs-3.2.4/short-readme.md`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.3/unittests/config/conftest.py` & `yaecs-3.2.4/unittests/config/conftest.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.3/unittests/config/test_config.py` & `yaecs-3.2.4/unittests/config/test_config.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.3/unittests/config/utils.py` & `yaecs-3.2.4/unittests/config/utils.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.3/usage_example/configs/project_config.py` & `yaecs-3.2.4/usage_example/configs/project_config.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.3/usage_example/main.py` & `yaecs-3.2.4/usage_example/main.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.3/usage_example/project_utils/utils.py` & `yaecs-3.2.4/usage_example/project_utils/utils.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.3/yaecs/__init__.py` & `yaecs-3.2.4/yaecs/__init__.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.3/yaecs/config/config.py` & `yaecs-3.2.4/yaecs/config/config.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.3/yaecs/config/config_base.py` & `yaecs-3.2.4/yaecs/config/config_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -371,15 +371,16 @@
                 if not any(state.startswith("setup") for state in self._state):
                     raise RuntimeError("Type-hinting is only allowed in the default config.")
                 name = yaml_loader.constructed_objects[list(yaml_loader.constructed_objects.keys())[-1]]
                 name = self._get_full_path(name)
                 type_hint = tag[6:]
                 if type_hint in self._assigned_as_yaml_tags:
                     _, processor_type, new_type_hint = self._assigned_as_yaml_tags[type_hint]
-                    self.add_processing_function_all(name, f"_tagged_method_{type_hint}", processor_type)
+                    if self.get_variation_name() is None:
+                        self.add_processing_function_all(name, f"_tagged_method_{type_hint}", processor_type)
                     type_hint = new_type_hint
                 self._main_config.add_type_hint(name, parse_type(type_hint))
                 if isinstance(node, yaml.ScalarNode):
                     if node.value == "":
                         def _can_be_str(parsed_type):
                             if parsed_type is str:
                                 return True
@@ -788,27 +789,27 @@
     def _process_parameter(self, name: str, parameter: Any, processing_type: str, order: Optional[Real] = None) -> Any:
         """ This method checks if a processing function has been defined for given name, then returns the processed
         value when that is the case. """
         if processing_type not in ["pre", "post"]:
             raise ValueError(f"Unknown processing_type : '{processing_type}'. Valid types are 'pre' or 'post'.")
         total_name = self._get_full_path(name)
         main = self.get_main_config()
+        processors = [proc for key, proc in getattr(self, f"_{processing_type}_processing_functions").items()
+                      if compare_string_pattern(total_name, key)]
+        processors = [(proc if isinstance(proc, Callable)
+                       else self._assigned_as_yaml_tags[proc[len("_tagged_method_"):]][0]) for proc in processors]
+        processors = sorted([p for p in processors if order is None or get_order(p) == order], key=get_order)
         if processing_type == "pre":
             main.remove_value_before_postprocessing(total_name)
         if main.get_master_switch(processing_type):
             old_value = None
             if processing_type == "pre":
                 self.check_type(main.get_type_hint(total_name))(parameter)
             else:
                 old_value = copy.deepcopy(parameter)
-            processors = [proc for key, proc in getattr(self, f"_{processing_type}_processing_functions").items()
-                          if compare_string_pattern(total_name, key)]
-            processors = [(proc if isinstance(proc, Callable)
-                           else self._assigned_as_yaml_tags[proc[len("_tagged_method_"):]][0]) for proc in processors]
-            processors = sorted([p for p in processors if order is None or get_order(p) == order], key=get_order)
             was_processed = bool(processors)
             for processor in processors:
                 try:
                     parameter = processor(parameter)
                 except Exception:
                     YAECS_LOGGER.error(f"ERROR while {processing_type}-processing param '{total_name}' :")
                     raise
@@ -817,12 +818,12 @@
                                    "pre-processing functions that change the type of a "
                                    "param to a non-native YAML type are forbidden because "
                                    "they cannot be saved. Please use a parameter "
                                    "post-processing instead.")
             if processing_type == "post" and was_processed:
                 main.save_value_before_postprocessing(self._get_full_path(name), old_value)
         elif processing_type == "pre":
-            for key, item in self._pre_processing_functions.items():
-                if compare_string_pattern(total_name, key) and item.__name__.startswith("yaecs_config_hook__"):
-                    for hook_name in item.__name__.split("__")[1].split(","):
+            for processor in processors:
+                if processor.__name__.startswith("yaecs_config_hook__"):
+                    for hook_name in processor.__name__.split("__")[1].split(","):
                         self.add_currently_processed_param_as_hook(hook_name)
         return parameter
```

### Comparing `yaecs-3.2.3/yaecs/config/config_convenience.py` & `yaecs-3.2.4/yaecs/config/config_convenience.py`

 * *Files 0% similar despite different names*

```diff
@@ -221,15 +221,15 @@
         strings.
         :param patterns: string, a list of strings or several strings
         :return: all params matching at least one of the input string
         """
         patterns = (patterns[0] if len(patterns) == 1 and isinstance(patterns[0], list) else patterns)
         if patterns is None or (len(patterns) == 1 and patterns[0] is None):
             return None
-        new_names = [n for n in patterns if "*" not in n and n in self.get_parameter_names(True)]
+        new_names = [n.strip(" ") for n in patterns if "*" not in n and n.strip(" ") in self.get_parameter_names(True)]
         for name in [n for n in patterns if "*" in n]:
             new_names = new_names + [p for p in self.get_parameter_names(True) if compare_string_pattern(p, name)]
         return new_names
 
     def save(self, filename: str = None, save_header: bool = True, save_hierarchy: str = True) -> None:
         """
         Saves the current config at the provided location. The saving format allows for a perfect recovery of the config
```

### Comparing `yaecs-3.2.3/yaecs/config/config_getters.py` & `yaecs-3.2.4/yaecs/config/config_getters.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.3/yaecs/config/config_hooks.py` & `yaecs-3.2.4/yaecs/config/config_hooks.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.3/yaecs/config/config_processing_functions.py` & `yaecs-3.2.4/yaecs/config/config_processing_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """ This file defines a library of convenient processing functions. """
 
 from functools import partial
 import logging
 import os
 from typing import Any, Callable, List, Optional, TYPE_CHECKING
 
-from ..yaecs_utils import assign_order, assign_yaml_tag, Priority, set_function_attribute
+from ..yaecs_utils import assign_order, assign_yaml_tag, compare_string_pattern, Priority, set_function_attribute
 
 if TYPE_CHECKING:
     from numbers import Number
     from .config import Configuration
 
 YAECS_LOGGER = logging.getLogger(__name__)
 
@@ -84,19 +84,19 @@
                             f"the copied param. Current default value '{path_to_copy}' is not a string.")
         main = self.get_main_config()
         param_name = self.get_processed_param_name(full_path=True)
         copy_fn = partial(_copy, main=main)
         set_function_attribute(copy_fn, "__name__", "_copy")
         set_function_attribute(copy_fn, "order", Priority.OFTEN_LAST)
 
-        current_processing = object.__getattribute__(main, "_post_processing_functions")
-        if not any((param_name in main.match_params(k) and v.__name__ == "_copy")
+        current_processing = object.__getattribute__(main, "_added_post_processing")()
+        if not any((compare_string_pattern(param_name, k) and v.__name__ == "_copy")
                    for k, v in current_processing.items()):
             main.add_processing_function_all(param_name, copy_fn, "post")
-        else:
+        elif self.get_variation_name() is None:
             YAECS_LOGGER.warning(f"WARNING : Parameter '{param_name}' was already declared as a copy of param "
                                  f"'{path_to_copy}'. Processing function will not be added again.")
 
         return self.protected_param(path_to_copy)
 
     def check_number_in_range(self, minimum: 'Number' = -float('inf'), maximum: 'Number' = float('inf')) -> Callable:
         """
```

### Comparing `yaecs-3.2.3/yaecs/config/config_setters.py` & `yaecs-3.2.4/yaecs/config/config_setters.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.3/yaecs/config_history.py` & `yaecs-3.2.4/yaecs/config_history.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.3/yaecs/experiment.py` & `yaecs-3.2.4/yaecs/experiment.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.3/yaecs/pytorch_lightning_utils.py` & `yaecs-3.2.4/yaecs/pytorch_lightning_utils.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.3/yaecs/user_utils.py` & `yaecs-3.2.4/yaecs/user_utils.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.3/yaecs/yaecs_utils.py` & `yaecs-3.2.4/yaecs/yaecs_utils.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.3/yaecs.egg-info/PKG-INFO` & `yaecs-3.2.4/yaecs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaecs
-Version: 3.2.3
+Version: 3.2.4
 Summary: A Config System designed for experimental purposes
 Author: Reactive Reality AG
 Project-URL: Source, https://gitlab.com/reactivereality/public/yaecs
 Keywords: template,machine,learning
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `yaecs-3.2.3/yaecs.egg-info/SOURCES.txt` & `yaecs-3.2.4/yaecs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

