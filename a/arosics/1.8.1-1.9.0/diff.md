# Comparing `tmp/arosics-1.8.1.tar.gz` & `tmp/arosics-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arosics-1.8.1.tar", last modified: Fri Mar 10 18:59:06 2023, max compression
+gzip compressed data, was "arosics-1.9.0.tar", last modified: Thu May  4 17:04:02 2023, max compression
```

## Comparing `arosics-1.8.1.tar` & `arosics-1.9.0.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 18:59:06.188099 arosics-1.8.1/
--rw-rw-rw-   0 root         (0) root         (0)      578 2023-03-10 18:58:44.000000 arosics-1.8.1/.coveragerc
--rw-rw-rw-   0 root         (0) root         (0)      292 2023-03-10 18:58:44.000000 arosics-1.8.1/.editorconfig
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 18:59:06.172100 arosics-1.8.1/.github/
--rw-rw-rw-   0 root         (0) root         (0)      318 2023-03-10 18:58:44.000000 arosics-1.8.1/.github/ISSUE_TEMPLATE.md
--rw-rw-rw-   0 root         (0) root         (0)      863 2023-03-10 18:58:44.000000 arosics-1.8.1/.github/create_release_from_gitlab_ci.sh
--rw-rw-rw-   0 root         (0) root         (0)      847 2023-03-10 18:58:44.000000 arosics-1.8.1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     3229 2023-03-10 18:58:44.000000 arosics-1.8.1/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     2716 2023-03-10 18:58:44.000000 arosics-1.8.1/.zenodo.json
--rw-rw-rw-   0 root         (0) root         (0)      173 2023-03-10 18:58:44.000000 arosics-1.8.1/AUTHORS.rst
--rw-rw-rw-   0 root         (0) root         (0)     1882 2023-03-10 18:58:44.000000 arosics-1.8.1/CITATION
--rw-rw-rw-   0 root         (0) root         (0)     3798 2023-03-10 18:58:44.000000 arosics-1.8.1/CONTRIBUTING.rst
--rw-rw-rw-   0 root         (0) root         (0)    24322 2023-03-10 18:58:44.000000 arosics-1.8.1/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)    10140 2023-03-10 18:58:44.000000 arosics-1.8.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      262 2023-03-10 18:58:44.000000 arosics-1.8.1/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     4118 2023-03-10 18:58:44.000000 arosics-1.8.1/Makefile
--rw-r--r--   0 root         (0) root         (0)     7979 2023-03-10 18:59:06.188099 arosics-1.8.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6434 2023-03-10 18:58:44.000000 arosics-1.8.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 18:59:06.176100 arosics-1.8.1/arosics/
--rwxrwxrwx   0 root         (0) root         (0)    86052 2023-03-10 18:58:44.000000 arosics-1.8.1/arosics/CoReg.py
--rw-rw-rw-   0 root         (0) root         (0)    42027 2023-03-10 18:58:44.000000 arosics-1.8.1/arosics/CoReg_local.py
--rw-rw-rw-   0 root         (0) root         (0)    23187 2023-03-10 18:58:44.000000 arosics-1.8.1/arosics/DeShifter.py
--rwxrwxrwx   0 root         (0) root         (0)    62923 2023-03-10 18:58:44.000000 arosics-1.8.1/arosics/Tie_Point_Grid.py
--rw-rw-rw-   0 root         (0) root         (0)     1778 2023-03-10 18:58:44.000000 arosics-1.8.1/arosics/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    20799 2023-03-10 18:58:44.000000 arosics-1.8.1/arosics/arosics_cli.py
--rwxrwxrwx   0 root         (0) root         (0)     6933 2023-03-10 18:58:44.000000 arosics-1.8.1/arosics/geometry.py
--rw-rw-rw-   0 root         (0) root         (0)     3925 2023-03-10 18:58:44.000000 arosics-1.8.1/arosics/plotting.py
--rw-rw-rw-   0 root         (0) root         (0)     1112 2023-03-10 18:58:44.000000 arosics-1.8.1/arosics/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 18:59:06.176100 arosics-1.8.1/arosics.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7979 2023-03-10 18:59:06.000000 arosics-1.8.1/arosics.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1807 2023-03-10 18:59:06.000000 arosics-1.8.1/arosics.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-10 18:59:06.000000 arosics-1.8.1/arosics.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-03-10 18:59:06.000000 arosics-1.8.1/arosics.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-10 18:59:06.000000 arosics-1.8.1/arosics.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      614 2023-03-10 18:59:06.000000 arosics-1.8.1/arosics.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-03-10 18:59:06.000000 arosics-1.8.1/arosics.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 18:59:06.176100 arosics-1.8.1/docs/
--rw-rw-rw-   0 root         (0) root         (0)     6769 2023-03-10 18:58:44.000000 arosics-1.8.1/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 18:59:06.172100 arosics-1.8.1/docs/_build/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 18:59:06.172100 arosics-1.8.1/docs/_build/html/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 18:59:06.180100 arosics-1.8.1/docs/_build/html/_images/
--rw-r--r--   0 root         (0) root         (0)    43518 2023-03-10 18:51:56.000000 arosics-1.8.1/docs/_build/html/_images/CoregPoints_table.png
--rw-r--r--   0 root         (0) root         (0)   772233 2023-03-10 18:51:56.000000 arosics-1.8.1/docs/_build/html/_images/animation_testcase1_zoom_L8_S2_global_coreg_before_after_900x456.gif
--rw-r--r--   0 root         (0) root         (0)     6615 2023-03-10 18:51:56.000000 arosics-1.8.1/docs/_build/html/_images/arosics_logo.png
--rw-r--r--   0 root         (0) root         (0)   994099 2023-03-10 18:51:56.000000 arosics-1.8.1/docs/_build/html/_images/output_40_1.png
--rw-r--r--   0 root         (0) root         (0)  1009524 2023-03-10 18:51:56.000000 arosics-1.8.1/docs/_build/html/_images/output_44_1.png
--rw-r--r--   0 root         (0) root         (0)   297816 2023-03-10 18:51:56.000000 arosics-1.8.1/docs/_build/html/_images/shift_vectors_testcase1__900x824.gif
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 18:59:06.180100 arosics-1.8.1/docs/_build/html/_static/
--rw-r--r--   0 root         (0) root         (0)     6615 2023-03-10 18:51:56.000000 arosics-1.8.1/docs/_build/html/_static/arosics_logo.png
--rw-r--r--   0 root         (0) root         (0)      286 2022-12-02 16:01:28.000000 arosics-1.8.1/docs/_build/html/_static/file.png
--rw-r--r--   0 root         (0) root         (0)       90 2022-12-02 16:01:28.000000 arosics-1.8.1/docs/_build/html/_static/minus.png
--rw-r--r--   0 root         (0) root         (0)       90 2022-12-02 16:01:28.000000 arosics-1.8.1/docs/_build/html/_static/plus.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 18:59:06.184100 arosics-1.8.1/docs/_static/
--rw-rw-rw-   0 root         (0) root         (0)       50 2023-03-10 18:58:44.000000 arosics-1.8.1/docs/_static/custom.css
--rw-rw-rw-   0 root         (0) root         (0)     2952 2023-03-10 18:58:44.000000 arosics-1.8.1/docs/about.rst
--rw-rw-rw-   0 root         (0) root         (0)      456 2023-03-10 18:58:44.000000 arosics-1.8.1/docs/api_cli_reference.rst
--rw-rw-rw-   0 root         (0) root         (0)       28 2023-03-10 18:58:44.000000 arosics-1.8.1/docs/authors.rst
--rw-rw-rw-   0 root         (0) root         (0)      552 2023-03-10 18:58:44.000000 arosics-1.8.1/docs/cli_reference.rst
--rwxrwxrwx   0 root         (0) root         (0)     9929 2023-03-10 18:58:44.000000 arosics-1.8.1/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-03-10 18:58:44.000000 arosics-1.8.1/docs/contributing.rst
--rw-rw-rw-   0 root         (0) root         (0)       28 2023-03-10 18:58:44.000000 arosics-1.8.1/docs/history.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 18:59:06.188099 arosics-1.8.1/docs/images/
--rw-rw-rw-   0 root         (0) root         (0)    43518 2023-03-10 18:58:44.000000 arosics-1.8.1/docs/images/CoregPoints_table.png
--rw-rw-rw-   0 root         (0) root         (0)   954684 2023-03-10 18:58:44.000000 arosics-1.8.1/docs/images/animation_testcase1_zoom_L8_S2_global_coreg_before_after_1066x540.gif
--rw-rw-rw-   0 root         (0) root         (0)   772233 2023-03-10 18:58:44.000000 arosics-1.8.1/docs/images/animation_testcase1_zoom_L8_S2_global_coreg_before_after_900x456.gif
--rw-rw-rw-   0 root         (0) root         (0)     6615 2023-03-10 18:58:44.000000 arosics-1.8.1/docs/images/arosics_logo.png
--rw-rw-rw-   0 root         (0) root         (0)   994099 2023-03-10 18:58:44.000000 arosics-1.8.1/docs/images/output_40_1.png
--rw-rw-rw-   0 root         (0) root         (0)  1009524 2023-03-10 18:58:44.000000 arosics-1.8.1/docs/images/output_44_1.png
--rw-rw-rw-   0 root         (0) root         (0)   297816 2023-03-10 18:58:44.000000 arosics-1.8.1/docs/images/shift_vectors_testcase1__900x824.gif
--rw-rw-rw-   0 root         (0) root         (0)      310 2023-03-10 18:58:44.000000 arosics-1.8.1/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1720 2023-03-10 18:58:44.000000 arosics-1.8.1/docs/installation.rst
--rw-rw-rw-   0 root         (0) root         (0)     6461 2023-03-10 18:58:44.000000 arosics-1.8.1/docs/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 18:59:06.188099 arosics-1.8.1/docs/usage/
--rw-rw-rw-   0 root         (0) root         (0)    10547 2023-03-10 18:58:44.000000 arosics-1.8.1/docs/usage/global_coreg.rst
--rw-rw-rw-   0 root         (0) root         (0)     3424 2023-03-10 18:58:44.000000 arosics-1.8.1/docs/usage/input_data_requirements.rst
--rw-rw-rw-   0 root         (0) root         (0)     7859 2023-03-10 18:58:44.000000 arosics-1.8.1/docs/usage/local_coreg.rst
--rw-rw-rw-   0 root         (0) root         (0)      753 2023-03-10 18:58:44.000000 arosics-1.8.1/docs/usage.rst
--rw-rw-rw-   0 root         (0) root         (0)      202 2023-03-10 18:58:44.000000 arosics-1.8.1/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      432 2023-03-10 18:59:06.188099 arosics-1.8.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     4127 2023-03-10 18:58:44.000000 arosics-1.8.1/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      481 2023-03-10 18:58:44.000000 arosics-1.8.1/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:04:02.559054 arosics-1.9.0/
+-rw-rw-rw-   0 root         (0) root         (0)      578 2023-05-04 17:03:38.000000 arosics-1.9.0/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)      292 2023-05-04 17:03:38.000000 arosics-1.9.0/.editorconfig
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:04:02.543054 arosics-1.9.0/.github/
+-rw-rw-rw-   0 root         (0) root         (0)      318 2023-05-04 17:03:38.000000 arosics-1.9.0/.github/ISSUE_TEMPLATE.md
+-rw-rw-rw-   0 root         (0) root         (0)      861 2023-05-04 17:03:38.000000 arosics-1.9.0/.github/create_release_from_gitlab_ci.sh
+-rw-rw-rw-   0 root         (0) root         (0)      847 2023-05-04 17:03:38.000000 arosics-1.9.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     3297 2023-05-04 17:03:38.000000 arosics-1.9.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2716 2023-05-04 17:03:38.000000 arosics-1.9.0/.zenodo.json
+-rw-rw-rw-   0 root         (0) root         (0)      173 2023-05-04 17:03:38.000000 arosics-1.9.0/AUTHORS.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1882 2023-05-04 17:03:38.000000 arosics-1.9.0/CITATION
+-rw-rw-rw-   0 root         (0) root         (0)     3798 2023-05-04 17:03:38.000000 arosics-1.9.0/CONTRIBUTING.rst
+-rw-rw-rw-   0 root         (0) root         (0)    24714 2023-05-04 17:03:38.000000 arosics-1.9.0/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)    10140 2023-05-04 17:03:38.000000 arosics-1.9.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      262 2023-05-04 17:03:38.000000 arosics-1.9.0/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     4118 2023-05-04 17:03:38.000000 arosics-1.9.0/Makefile
+-rw-r--r--   0 root         (0) root         (0)     7961 2023-05-04 17:04:02.559054 arosics-1.9.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6418 2023-05-04 17:03:38.000000 arosics-1.9.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:04:02.547054 arosics-1.9.0/arosics/
+-rwxrwxrwx   0 root         (0) root         (0)    86052 2023-05-04 17:03:38.000000 arosics-1.9.0/arosics/CoReg.py
+-rw-rw-rw-   0 root         (0) root         (0)    42345 2023-05-04 17:03:38.000000 arosics-1.9.0/arosics/CoReg_local.py
+-rw-rw-rw-   0 root         (0) root         (0)    23187 2023-05-04 17:03:38.000000 arosics-1.9.0/arosics/DeShifter.py
+-rwxrwxrwx   0 root         (0) root         (0)    70260 2023-05-04 17:03:38.000000 arosics-1.9.0/arosics/Tie_Point_Grid.py
+-rw-rw-rw-   0 root         (0) root         (0)     2195 2023-05-04 17:03:38.000000 arosics-1.9.0/arosics/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    20799 2023-05-04 17:03:38.000000 arosics-1.9.0/arosics/arosics_cli.py
+-rwxrwxrwx   0 root         (0) root         (0)     6933 2023-05-04 17:03:38.000000 arosics-1.9.0/arosics/geometry.py
+-rw-rw-rw-   0 root         (0) root         (0)     3925 2023-05-04 17:03:38.000000 arosics-1.9.0/arosics/plotting.py
+-rw-rw-rw-   0 root         (0) root         (0)     1112 2023-05-04 17:03:38.000000 arosics-1.9.0/arosics/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:04:02.547054 arosics-1.9.0/arosics.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7961 2023-05-04 17:04:02.000000 arosics-1.9.0/arosics.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1807 2023-05-04 17:04:02.000000 arosics-1.9.0/arosics.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 17:04:02.000000 arosics-1.9.0/arosics.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-05-04 17:04:02.000000 arosics-1.9.0/arosics.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 17:04:02.000000 arosics-1.9.0/arosics.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      633 2023-05-04 17:04:02.000000 arosics-1.9.0/arosics.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-04 17:04:02.000000 arosics-1.9.0/arosics.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:04:02.547054 arosics-1.9.0/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     6769 2023-05-04 17:03:38.000000 arosics-1.9.0/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:04:02.539054 arosics-1.9.0/docs/_build/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:04:02.539054 arosics-1.9.0/docs/_build/html/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:04:02.551054 arosics-1.9.0/docs/_build/html/_images/
+-rw-r--r--   0 root         (0) root         (0)    43518 2023-05-04 16:56:43.000000 arosics-1.9.0/docs/_build/html/_images/CoregPoints_table.png
+-rw-r--r--   0 root         (0) root         (0)   772233 2023-05-04 16:56:43.000000 arosics-1.9.0/docs/_build/html/_images/animation_testcase1_zoom_L8_S2_global_coreg_before_after_900x456.gif
+-rw-r--r--   0 root         (0) root         (0)     6615 2023-05-04 16:56:43.000000 arosics-1.9.0/docs/_build/html/_images/arosics_logo.png
+-rw-r--r--   0 root         (0) root         (0)   994099 2023-05-04 16:56:43.000000 arosics-1.9.0/docs/_build/html/_images/output_40_1.png
+-rw-r--r--   0 root         (0) root         (0)  1009524 2023-05-04 16:56:43.000000 arosics-1.9.0/docs/_build/html/_images/output_44_1.png
+-rw-r--r--   0 root         (0) root         (0)   297816 2023-05-04 16:56:43.000000 arosics-1.9.0/docs/_build/html/_images/shift_vectors_testcase1__900x824.gif
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:04:02.551054 arosics-1.9.0/docs/_build/html/_static/
+-rw-r--r--   0 root         (0) root         (0)     6615 2023-05-04 16:56:43.000000 arosics-1.9.0/docs/_build/html/_static/arosics_logo.png
+-rw-r--r--   0 root         (0) root         (0)      286 2022-12-02 16:01:28.000000 arosics-1.9.0/docs/_build/html/_static/file.png
+-rw-r--r--   0 root         (0) root         (0)       90 2022-12-02 16:01:28.000000 arosics-1.9.0/docs/_build/html/_static/minus.png
+-rw-r--r--   0 root         (0) root         (0)       90 2022-12-02 16:01:28.000000 arosics-1.9.0/docs/_build/html/_static/plus.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:04:02.551054 arosics-1.9.0/docs/_static/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-05-04 17:03:38.000000 arosics-1.9.0/docs/_static/custom.css
+-rw-rw-rw-   0 root         (0) root         (0)     2952 2023-05-04 17:03:38.000000 arosics-1.9.0/docs/about.rst
+-rw-rw-rw-   0 root         (0) root         (0)      456 2023-05-04 17:03:38.000000 arosics-1.9.0/docs/api_cli_reference.rst
+-rw-rw-rw-   0 root         (0) root         (0)       28 2023-05-04 17:03:38.000000 arosics-1.9.0/docs/authors.rst
+-rw-rw-rw-   0 root         (0) root         (0)      552 2023-05-04 17:03:38.000000 arosics-1.9.0/docs/cli_reference.rst
+-rwxrwxrwx   0 root         (0) root         (0)     9929 2023-05-04 17:03:38.000000 arosics-1.9.0/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-05-04 17:03:38.000000 arosics-1.9.0/docs/contributing.rst
+-rw-rw-rw-   0 root         (0) root         (0)       28 2023-05-04 17:03:38.000000 arosics-1.9.0/docs/history.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:04:02.559054 arosics-1.9.0/docs/images/
+-rw-rw-rw-   0 root         (0) root         (0)    43518 2023-05-04 17:03:38.000000 arosics-1.9.0/docs/images/CoregPoints_table.png
+-rw-rw-rw-   0 root         (0) root         (0)   954684 2023-05-04 17:03:38.000000 arosics-1.9.0/docs/images/animation_testcase1_zoom_L8_S2_global_coreg_before_after_1066x540.gif
+-rw-rw-rw-   0 root         (0) root         (0)   772233 2023-05-04 17:03:38.000000 arosics-1.9.0/docs/images/animation_testcase1_zoom_L8_S2_global_coreg_before_after_900x456.gif
+-rw-rw-rw-   0 root         (0) root         (0)     6615 2023-05-04 17:03:38.000000 arosics-1.9.0/docs/images/arosics_logo.png
+-rw-rw-rw-   0 root         (0) root         (0)   994099 2023-05-04 17:03:38.000000 arosics-1.9.0/docs/images/output_40_1.png
+-rw-rw-rw-   0 root         (0) root         (0)  1009524 2023-05-04 17:03:38.000000 arosics-1.9.0/docs/images/output_44_1.png
+-rw-rw-rw-   0 root         (0) root         (0)   297816 2023-05-04 17:03:38.000000 arosics-1.9.0/docs/images/shift_vectors_testcase1__900x824.gif
+-rw-rw-rw-   0 root         (0) root         (0)      310 2023-05-04 17:03:38.000000 arosics-1.9.0/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1720 2023-05-04 17:03:38.000000 arosics-1.9.0/docs/installation.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6461 2023-05-04 17:03:38.000000 arosics-1.9.0/docs/make.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:04:02.559054 arosics-1.9.0/docs/usage/
+-rw-rw-rw-   0 root         (0) root         (0)    10547 2023-05-04 17:03:38.000000 arosics-1.9.0/docs/usage/global_coreg.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3424 2023-05-04 17:03:38.000000 arosics-1.9.0/docs/usage/input_data_requirements.rst
+-rw-rw-rw-   0 root         (0) root         (0)     7859 2023-05-04 17:03:38.000000 arosics-1.9.0/docs/usage/local_coreg.rst
+-rw-rw-rw-   0 root         (0) root         (0)      753 2023-05-04 17:03:38.000000 arosics-1.9.0/docs/usage.rst
+-rw-rw-rw-   0 root         (0) root         (0)      221 2023-05-04 17:03:38.000000 arosics-1.9.0/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      432 2023-05-04 17:04:02.559054 arosics-1.9.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     4158 2023-05-04 17:03:38.000000 arosics-1.9.0/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      481 2023-05-04 17:03:39.000000 arosics-1.9.0/tox.ini
```

### Comparing `arosics-1.8.1/.coveragerc` & `arosics-1.9.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `arosics-1.8.1/.github/create_release_from_gitlab_ci.sh` & `arosics-1.9.0/.github/create_release_from_gitlab_ci.sh`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # NOTE: The environment variables are present during the CI job.
 
 URL_RELEASES=https://api.github.com/repos/$GITHUB_USER/$GITHUB_REPONAME/releases
 
 # create the release
 API_JSON=$(printf '{"tag_name":"%s",
-                    "target_commitish":"master",
+                    "target_commitish":"main",
                     "name":"%s",
                     "body":"",
                     "draft":false,
                     "prerelease":false}' $CI_COMMIT_TAG $CI_COMMIT_TAG)
 AUTH_HEADER="Authorization: token $GITHUB_RELEASE_TOKEN"
 curl $URL_RELEASES --data "$API_JSON" -H "$AUTH_HEADER"
```

### Comparing `arosics-1.8.1/.gitignore` & `arosics-1.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `arosics-1.8.1/.gitlab-ci.yml` & `arosics-1.9.0/.gitlab-ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,16 @@
   script:
     - source /opt/conda/bin/activate ci_env
 
     # update py_tools_ds and geoarray
     - pip install -U py_tools_ds -q
     - pip install -U geoarray -q
 
+    - pip install scipy  # TODO remove as soon as CI runner is rebuilt
+
     # run tests
     - make pytest
 
     # create the docs
     - make docs
   artifacts:
     expose_as: 'Test and coverage report'
@@ -77,15 +79,15 @@
     - pwd
     - ls
 
     # test importability
     - python -c "import arosics; print(arosics)"
     - python -c "from arosics import COREG, COREG_LOCAL"
   only:
-    - master
+    - main
 
 
 pages:  # this job must be called 'pages' to advise GitLab to upload content to GitLab Pages
   stage: deploy
   dependencies:
     - test_arosics
   script:
@@ -113,15 +115,15 @@
     - ls -al public/coverage
     - ls -al public/test_reports
   artifacts:
     paths:
       - public
     expire_in: 30 days
   only:
-    - master
+    - main
     - enhancement/improve_docs
 
 
 deploy_pypi:
   stage: deploy
   dependencies:
     - test_arosics
```

### Comparing `arosics-1.8.1/.zenodo.json` & `arosics-1.9.0/.zenodo.json`

 * *Files identical despite different names*

### Comparing `arosics-1.8.1/CITATION` & `arosics-1.9.0/CITATION`

 * *Files identical despite different names*

### Comparing `arosics-1.8.1/CONTRIBUTING.rst` & `arosics-1.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `arosics-1.8.1/HISTORY.rst` & `arosics-1.9.0/HISTORY.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 =======
 History
 =======
 
+1.9.0 (2023-05-04)
+------------------
+
+* Re-implemented interpolation of tie point attributes into space (!23).
+  Three techniques are now supported: RBF, GPR, and Ordinary Kriging. Added scikit-learn to dependencies.
+* Fixed GDAL warning related to PROJ_DATA/PROJ_LIB environment variables (!34).
+* Added parameter 'rs_random_state' (RANSAC random state) and set it to 0 by default (!35).
+
+
 1.8.1 (2023-03-10)
 ------------------
 
 * Fixed https://github.com/GFZ/arosics/issues/20 (out_crea_options has no effect) (!32).
 * Updated copyright (!33).
```

### Comparing `arosics-1.8.1/LICENSE` & `arosics-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arosics-1.8.1/Makefile` & `arosics-1.9.0/Makefile`

 * *Files identical despite different names*

### Comparing `arosics-1.8.1/PKG-INFO` & `arosics-1.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: arosics
-Version: 1.8.1
+Version: 1.9.0
 Summary: An Automated and Robust Open-Source Image Co-Registration Software for Multi-Sensor Satellite Data
 Home-page: https://git.gfz-potsdam.de/danschef/arosics
 Author: Daniel Scheffler
 Author-email: daniel.scheffler@gfz-potsdam.de
 License: Apache-2.0
 Project-URL: Source code, https://git.gfz-potsdam.de/danschef/arosics
 Project-URL: Issue Tracker, https://git.gfz-potsdam.de/danschef/arosics/-/issues
 Project-URL: Documentation, https://danschef.git-pages.gfz-potsdam.de/arosics/doc/
-Project-URL: Change log, https://git.gfz-potsdam.de/danschef/arosics/-/blob/master/HISTORY.rst
+Project-URL: Change log, https://git.gfz-potsdam.de/danschef/arosics/-/blob/main/HISTORY.rst
 Project-URL: Algorithm paper, https://www.mdpi.com/2072-4292/9/7/676
 Project-URL: Zenodo, https://zenodo.org/record/5093940
 Keywords: arosics,image co-registration,geometric pre-processing,remote sensing,sensor fusion
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: Apache Software License
@@ -43,35 +43,35 @@
 * Free software: Apache 2.0
 * **Documentation:** https://danschef.git-pages.gfz-potsdam.de/arosics/doc/
 * The (open-access) **paper** corresponding to this software repository can be found here:
   `Scheffler et al. 2017 <https://www.mdpi.com/2072-4292/9/7/676>`__
   (cite as: Scheffler D, Hollstein A, Diedrich H, Segl K, Hostert P. AROSICS: An Automated and Robust Open-Source
   Image Co-Registration Software for Multi-Sensor Satellite Data. Remote Sensing. 2017; 9(7):676).
 * Information on how to **cite the AROSICS Python package** can be found in the
-  `CITATION <https://git.gfz-potsdam.de/danschef/arosics/-/blob/master/CITATION>`__ file.
+  `CITATION <https://git.gfz-potsdam.de/danschef/arosics/-/blob/main/CITATION>`__ file.
 * Submit feedback by filing an issue `here <https://git.gfz-potsdam.de/danschef/arosics/issues>`__
   or join our chat here: |Gitter|
 
 .. |Gitter| image:: https://badges.gitter.im/Join%20Chat.svg
     :target: https://gitter.im/arosics/Lobby?utm_source=share-link&utm_medium=link&utm_campaign=share-link
     :alt: https://gitter.im/arosics/Lobby?utm_source=share-link&utm_medium=link&utm_campaign=share-link
 
 Status
 ------
 
-.. image:: https://git.gfz-potsdam.de/danschef/arosics/badges/master/pipeline.svg
-        :target: https://git.gfz-potsdam.de/danschef/arosics/commits/master
-.. image:: https://git.gfz-potsdam.de/danschef/arosics/badges/master/coverage.svg
+.. image:: https://git.gfz-potsdam.de/danschef/arosics/badges/main/pipeline.svg
+        :target: https://git.gfz-potsdam.de/danschef/arosics/commits/main
+.. image:: https://git.gfz-potsdam.de/danschef/arosics/badges/main/coverage.svg
         :target: https://danschef.git-pages.gfz-potsdam.de/arosics/coverage/
 .. image:: https://img.shields.io/pypi/v/arosics.svg
         :target: https://pypi.python.org/pypi/arosics
 .. image:: https://img.shields.io/conda/vn/conda-forge/arosics.svg
         :target: https://anaconda.org/conda-forge/arosics
 .. image:: https://img.shields.io/pypi/l/arosics.svg
-        :target: https://git.gfz-potsdam.de/danschef/arosics/blob/master/LICENSE
+        :target: https://git.gfz-potsdam.de/danschef/arosics/blob/main/LICENSE
 .. image:: https://img.shields.io/pypi/pyversions/arosics.svg
         :target: https://img.shields.io/pypi/pyversions/arosics.svg
 .. image:: https://img.shields.io/pypi/dm/arosics.svg
         :target: https://pypi.python.org/pypi/arosics
 .. image:: https://zenodo.org/badge/253474603.svg
         :target: https://zenodo.org/badge/latestdoi/253474603
 
@@ -99,39 +99,39 @@
 This allows very fast co-registration but only corrects for translational (global) X/Y shifts.
 The calculated subpixel-shifts are (by default) applied to the geocoding information of the output image.
 No spatial resampling is done automatically as long as both input images have the same projection. However, AROSICS
 also allows to align the output image to the reference image coordinate grid if needed.
 
 Here is an example of a Landsat-8 / Sentinel-2 image pair before and after co-registration using AROSICS:
 
-.. image:: https://git.gfz-potsdam.de/danschef/arosics/raw/master/docs/images/animation_testcase1_zoom_L8_S2_global_coreg_before_after_900x456.gif
+.. image:: https://git.gfz-potsdam.de/danschef/arosics/raw/main/docs/images/animation_testcase1_zoom_L8_S2_global_coreg_before_after_900x456.gif
 
 
 Local co-registration - for spatially variable shifts but a bit slower
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 A dense grid of tie points is automatically computed, whereas tie points are subsequently validated using a
 multistage workflow. Only those tie points not marked as false-positives are used to compute the parameters of an
 affine transformation. Warping of the target image is done using an appropriate resampling technique
 (cubic by default).
 
 Here is an example of the computed shift vectors after filtering false-positives
 (mainly due to clouds in the target image):
 
-.. image:: https://git.gfz-potsdam.de/danschef/arosics/raw/master/docs/images/shift_vectors_testcase1__900x824.gif
+.. image:: https://git.gfz-potsdam.de/danschef/arosics/raw/main/docs/images/shift_vectors_testcase1__900x824.gif
 
 
 For further details check out the `documentation <https://danschef.git-pages.gfz-potsdam.de/arosics/doc/>`__!
 
 
 History / Changelog
 -------------------
 
 You can find the protocol of recent changes in the AROSICS package
-`here <https://git.gfz-potsdam.de/danschef/arosics/-/blob/master/HISTORY.rst>`__.
+`here <https://git.gfz-potsdam.de/danschef/arosics/-/blob/main/HISTORY.rst>`__.
 
 
 Credits
 -------
 
 AROSICS was developed by Daniel Scheffler (German Research Centre of Geosciences) within the context of the
 `GeoMultiSens <http://www.geomultisens.gfz-potsdam.de/>`__ project funded by the German Federal Ministry of Education and Research
```

### Comparing `arosics-1.8.1/README.rst` & `arosics-1.9.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -9,35 +9,35 @@
 * Free software: Apache 2.0
 * **Documentation:** https://danschef.git-pages.gfz-potsdam.de/arosics/doc/
 * The (open-access) **paper** corresponding to this software repository can be found here:
   `Scheffler et al. 2017 <https://www.mdpi.com/2072-4292/9/7/676>`__
   (cite as: Scheffler D, Hollstein A, Diedrich H, Segl K, Hostert P. AROSICS: An Automated and Robust Open-Source
   Image Co-Registration Software for Multi-Sensor Satellite Data. Remote Sensing. 2017; 9(7):676).
 * Information on how to **cite the AROSICS Python package** can be found in the
-  `CITATION <https://git.gfz-potsdam.de/danschef/arosics/-/blob/master/CITATION>`__ file.
+  `CITATION <https://git.gfz-potsdam.de/danschef/arosics/-/blob/main/CITATION>`__ file.
 * Submit feedback by filing an issue `here <https://git.gfz-potsdam.de/danschef/arosics/issues>`__
   or join our chat here: |Gitter|
 
 .. |Gitter| image:: https://badges.gitter.im/Join%20Chat.svg
     :target: https://gitter.im/arosics/Lobby?utm_source=share-link&utm_medium=link&utm_campaign=share-link
     :alt: https://gitter.im/arosics/Lobby?utm_source=share-link&utm_medium=link&utm_campaign=share-link
 
 Status
 ------
 
-.. image:: https://git.gfz-potsdam.de/danschef/arosics/badges/master/pipeline.svg
-        :target: https://git.gfz-potsdam.de/danschef/arosics/commits/master
-.. image:: https://git.gfz-potsdam.de/danschef/arosics/badges/master/coverage.svg
+.. image:: https://git.gfz-potsdam.de/danschef/arosics/badges/main/pipeline.svg
+        :target: https://git.gfz-potsdam.de/danschef/arosics/commits/main
+.. image:: https://git.gfz-potsdam.de/danschef/arosics/badges/main/coverage.svg
         :target: https://danschef.git-pages.gfz-potsdam.de/arosics/coverage/
 .. image:: https://img.shields.io/pypi/v/arosics.svg
         :target: https://pypi.python.org/pypi/arosics
 .. image:: https://img.shields.io/conda/vn/conda-forge/arosics.svg
         :target: https://anaconda.org/conda-forge/arosics
 .. image:: https://img.shields.io/pypi/l/arosics.svg
-        :target: https://git.gfz-potsdam.de/danschef/arosics/blob/master/LICENSE
+        :target: https://git.gfz-potsdam.de/danschef/arosics/blob/main/LICENSE
 .. image:: https://img.shields.io/pypi/pyversions/arosics.svg
         :target: https://img.shields.io/pypi/pyversions/arosics.svg
 .. image:: https://img.shields.io/pypi/dm/arosics.svg
         :target: https://pypi.python.org/pypi/arosics
 .. image:: https://zenodo.org/badge/253474603.svg
         :target: https://zenodo.org/badge/latestdoi/253474603
 
@@ -65,39 +65,39 @@
 This allows very fast co-registration but only corrects for translational (global) X/Y shifts.
 The calculated subpixel-shifts are (by default) applied to the geocoding information of the output image.
 No spatial resampling is done automatically as long as both input images have the same projection. However, AROSICS
 also allows to align the output image to the reference image coordinate grid if needed.
 
 Here is an example of a Landsat-8 / Sentinel-2 image pair before and after co-registration using AROSICS:
 
-.. image:: https://git.gfz-potsdam.de/danschef/arosics/raw/master/docs/images/animation_testcase1_zoom_L8_S2_global_coreg_before_after_900x456.gif
+.. image:: https://git.gfz-potsdam.de/danschef/arosics/raw/main/docs/images/animation_testcase1_zoom_L8_S2_global_coreg_before_after_900x456.gif
 
 
 Local co-registration - for spatially variable shifts but a bit slower
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 A dense grid of tie points is automatically computed, whereas tie points are subsequently validated using a
 multistage workflow. Only those tie points not marked as false-positives are used to compute the parameters of an
 affine transformation. Warping of the target image is done using an appropriate resampling technique
 (cubic by default).
 
 Here is an example of the computed shift vectors after filtering false-positives
 (mainly due to clouds in the target image):
 
-.. image:: https://git.gfz-potsdam.de/danschef/arosics/raw/master/docs/images/shift_vectors_testcase1__900x824.gif
+.. image:: https://git.gfz-potsdam.de/danschef/arosics/raw/main/docs/images/shift_vectors_testcase1__900x824.gif
 
 
 For further details check out the `documentation <https://danschef.git-pages.gfz-potsdam.de/arosics/doc/>`__!
 
 
 History / Changelog
 -------------------
 
 You can find the protocol of recent changes in the AROSICS package
-`here <https://git.gfz-potsdam.de/danschef/arosics/-/blob/master/HISTORY.rst>`__.
+`here <https://git.gfz-potsdam.de/danschef/arosics/-/blob/main/HISTORY.rst>`__.
 
 
 Credits
 -------
 
 AROSICS was developed by Daniel Scheffler (German Research Centre of Geosciences) within the context of the
 `GeoMultiSens <http://www.geomultisens.gfz-potsdam.de/>`__ project funded by the German Federal Ministry of Education and Research
```

### Comparing `arosics-1.8.1/arosics/CoReg.py` & `arosics-1.9.0/arosics/CoReg.py`

 * *Files identical despite different names*

### Comparing `arosics-1.8.1/arosics/CoReg_local.py` & `arosics-1.9.0/arosics/CoReg_local.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,15 @@
                  s_b4match: int = 1,
                  max_iter: int = 5,
                  max_shift: int = 5,
                  tieP_filter_level: int = 3,
                  min_reliability: float = 60,
                  rs_max_outlier: float = 10,
                  rs_tolerance: float = 2.5,
+                 rs_random_state: Optional[int] = 0,
                  align_grids: bool = True,
                  match_gsd: bool = False,
                  out_gsd: float = None,
                  target_xyGrid=None,
                  resamp_alg_deshift: str = 'cubic',
                  resamp_alg_calc: str = 'cubic',
                  footprint_poly_ref: str = None,
@@ -177,14 +178,17 @@
 
         :param rs_max_outlier:
             RANSAC tie point filtering: proportion of expected outliers (default: 10%)
 
         :param rs_tolerance:
             RANSAC tie point filtering: percentage tolerance for max_outlier_percentage (default: 2.5%)
 
+        :param rs_random_state:
+            RANSAC random state (an integer corresponds to a fixed/pseudo-random state, None randomizes the result)
+
         :param align_grids:
             True: align the input coordinate grid to the reference (does not affect the output pixel size as long as
             input and output pixel sizes are compatible (5:30 or 10:30 but not 4:30), default = True
 
         :param match_gsd:
             True: match the input pixel size to the reference pixel size,
             default = False
@@ -289,14 +293,15 @@
         self.window_size = window_size
         self.max_shift = max_shift
         self.max_iter = max_iter
         self.tieP_filter_level = tieP_filter_level
         self.min_reliability = min_reliability
         self.rs_max_outlier = rs_max_outlier
         self.rs_tolerance = rs_tolerance
+        self.rs_random_state = rs_random_state
         self.align_grids = align_grids
         self.match_gsd = match_gsd
         self.out_gsd = out_gsd
         self.target_xyGrid = target_xyGrid
         self.rspAlg_DS = resamp_alg_deshift  # TODO convert integers to strings
         self.rspAlg_calc = resamp_alg_calc
         self.calc_corners = calc_corners
@@ -471,15 +476,16 @@
                            max_points=self.max_points,
                            outFillVal=self.outFillVal,
                            resamp_alg_calc=self.rspAlg_calc,
                            tieP_filter_level=self.tieP_filter_level,
                            outlDetect_settings=dict(
                                min_reliability=self.min_reliability,
                                rs_max_outlier=self.rs_max_outlier,
-                               rs_tolerance=self.rs_tolerance),
+                               rs_tolerance=self.rs_tolerance,
+                               rs_random_state=self.rs_random_state),
                            dir_out=self.projectDir,
                            CPUs=self.CPUs,
                            progress=self.progress,
                            v=self.v,
                            q=self.q)
         self._tiepoint_grid.get_CoRegPoints_table()
```

### Comparing `arosics-1.8.1/arosics/DeShifter.py` & `arosics-1.9.0/arosics/DeShifter.py`

 * *Files identical despite different names*

### Comparing `arosics-1.8.1/arosics/Tie_Point_Grid.py` & `arosics-1.9.0/arosics/Tie_Point_Grid.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,23 +23,25 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import collections
 import multiprocessing
 import os
 import warnings
-import time
+from time import time, sleep
 from typing import Optional, Union
 
 # custom
 from osgeo import gdal
 import numpy as np
 from geopandas import GeoDataFrame
 from pandas import DataFrame, Series
 from shapely.geometry import Point
+from matplotlib import pyplot as plt
+from scipy.interpolate import RBFInterpolator, RegularGridInterpolator
 
 # internal modules
 from .CoReg import COREG
 from py_tools_ds.geo.projection import isLocal
 from py_tools_ds.io.pathgen import get_generic_outpath
 from py_tools_ds.processing.progress_mon import ProgressBar
 from py_tools_ds.geo.vector.conversion import points_to_raster
@@ -124,15 +126,15 @@
                        - filters all tie points out where shift correction does not increase image similarity within
                          matching window (measured by mean structural similarity index)
             - Level 3: RANSAC outlier detection
 
         :param outlDetect_settings:
             a dictionary with the settings to be passed to arosics.TiePointGrid.Tie_Point_Refiner.
             Available keys: min_reliability, rs_max_outlier, rs_tolerance, rs_max_iter, rs_exclude_previous_outliers,
-            rs_timeout, q. See documentation there.
+            rs_timeout, rs_random_state, q. See documentation there.
 
         :param dir_out:
             output directory to be used for all outputs if nothing else is given to the individual methods
 
         :param CPUs:
             number of CPUs to use during calculation of tie points grid
             (default: None, which means 'all CPUs available')
@@ -167,15 +169,14 @@
 
         self.ref = self.COREG_obj.ref  # type: GeoArray_CoReg
         self.shift = self.COREG_obj.shift  # type: GeoArray_CoReg
 
         self.XY_points, self.XY_mapPoints = self._get_imXY__mapXY_points(self.grid_res)
         self._CoRegPoints_table = None  # set by self.CoRegPoints_table
         self._GCPList = None  # set by self.to_GCPList()
-        self.kriged = None  # set by Raster_using_Kriging()
 
     @property
     def mean_x_shift_px(self):
         return self.CoRegPoints_table['X_SHIFT_PX'][self.CoRegPoints_table['X_SHIFT_PX'] != self.outFillVal].mean()
 
     @property
     def mean_y_shift_px(self):
@@ -387,15 +388,15 @@
             with multiprocessing.Pool(self.CPUs, initializer=mp_initializer, initargs=(self.ref, self.shift)) as pool:
                 if self.q or not self.progress:
                     results = pool.map(self._get_spatial_shifts, list_coreg_kwargs)
                 else:
                     results = pool.map_async(self._get_spatial_shifts, list_coreg_kwargs, chunksize=1)
                     bar = ProgressBar(prefix='\tprogress:')
                     while True:
-                        time.sleep(.1)
+                        sleep(.1)
                         # this does not really represent the remaining tasks but the remaining chunks
                         # -> thus chunksize=1
                         # noinspection PyProtectedMember
                         numberDone = len(GDF) - results._number_left
                         if self.progress:
                             bar.print_progress(percent=numberDone / len(GDF) * 100)
                         if results.ready():
@@ -952,98 +953,58 @@
                                           % (self.grid_res, self.COREG_obj.win_size_XY[0],
                                              self.COREG_obj.win_size_XY[1], self.shift.basename, self.ref.basename))
 
         out_GA.save(path_out, fmt=fmt if fmt else 'Gtiff')
 
         return out_GA
 
-    def to_Raster_using_Kriging(self, attrName, skip_nodata=1, skip_nodata_col='ABS_SHIFT', outGridRes=None,
-                                fName_out=None, tilepos=None, tilesize=500, mp=None):
-
-        mp = False if self.CPUs == 1 else True
-        self._Kriging_sp(attrName, skip_nodata=skip_nodata, skip_nodata_col=skip_nodata_col,
-                         outGridRes=outGridRes, fName_out=fName_out, tilepos=tilepos)
-
-        # if mp:
-        #     tilepositions = UTL.get_image_tileborders([tilesize,tilesize],self.tgt_shape)
-        #     args_kwargs_dicts=[]
-        #     for tp in tilepositions:
-        #         kwargs_dict = {'skip_nodata':skip_nodata,'skip_nodata_col':skip_nodata_col,'outGridRes':outGridRes,
-        #                        'fName_out':fName_out,'tilepos':tp}
-        #         args_kwargs_dicts.append({'args':[attrName],'kwargs':kwargs_dict})
-        #     # self.kriged=[]
-        #     # for i in args_kwargs_dicts:
-        #     #     res = self.Kriging_mp(i)
-        #     #     self.kriged.append(res)
-        #     #     print(res)
-        #
-        #     with multiprocessing.Pool() as pool:
-        #        self.kriged = pool.map(self.Kriging_mp,args_kwargs_dicts)
-        #        pool.close()  # needed to make coverage work in multiprocessing
-        #        pool.join()
-        # else:
-        #     self.Kriging_sp(attrName,skip_nodata=skip_nodata,skip_nodata_col=skip_nodata_col,
-        #                     outGridRes=outGridRes,fName_out=fName_out,tilepos=tilepos)
-        res = self.kriged if mp else None
-        return res
-
-    def _Kriging_sp(self, attrName, skip_nodata=1, skip_nodata_col='ABS_SHIFT', outGridRes=None,
-                    fName_out=None, tilepos=None):
-        GDF = self.CoRegPoints_table
-        GDF2pass = GDF if not skip_nodata else GDF[GDF[skip_nodata_col] != self.outFillVal]
-
-        X_coords, Y_coords, ABS_SHIFT = GDF2pass['X_MAP'], GDF2pass['Y_MAP'], GDF2pass[attrName]
-
-        xmin, ymin, xmax, ymax = GDF2pass.total_bounds
-
-        grid_res = outGridRes if outGridRes else int(min(xmax - xmin, ymax - ymin) / 250)
-        grid_x, grid_y = np.arange(xmin, xmax + grid_res, grid_res), np.arange(ymax, ymin - grid_res, -grid_res)
-
-        # Reference: P.K. Kitanidis, Introduction to Geostatistcs: Applications in Hydrogeology,
-        #            (Cambridge University Press, 1997) 272 p.
-        from pykrige.ok import OrdinaryKriging
-        OK = OrdinaryKriging(X_coords, Y_coords, ABS_SHIFT, variogram_model='spherical', verbose=False)
-        zvalues, sigmasq = OK.execute('grid', grid_x, grid_y, backend='C', n_closest_points=12)
+    def to_interpolated_raster(self,
+                               metric: str = 'ABS_SHIFT',
+                               method: str = 'RBF',
+                               plot_result: bool = False,
+                               lowres_spacing: int = 5,
+                               v: bool = False
+                               ) -> np.ndarray:
+        """Interpolate the point data of the given metric into space.
+
+        :param metric:          metric name to interpolate, i.e., one of the column names of
+                                Tie_Point_Grid.CoRegPoints_table, e.g., 'ABS_SHIFT'.
+        :param method:          interpolation algorithm
+                                - 'RBF' (Radial Basis Function)
+                                - 'GPR' (Gaussian Process Regression; equivalent to Simple Kriging)
+                                - 'Kriging' (Ordinary Kriging based on pykrige)
+        :param plot_result:     plot the result to assess the interpolation quality
+        :param lowres_spacing:  by default, RBF, GPR, and Kriging run a lower resolution which is then linearly
+                                interpolated to the full output image resolution. lowres_spacing defines the number of
+                                pixels between the low resolution grid points
+                                (higher values are faster but less accurate, default: 5)
+        :param v:               enable verbose mode
+        :return:    interpolation result as numpy array in the X/Y dimension of the target image of the co-registration
+        """
+        TPGI = Tie_Point_Grid_Interpolator(self, v=v)
 
-        if self.CPUs is None or self.CPUs > 1:
-            fName_out = fName_out if fName_out else \
-                "Kriging__%s__grid%s_ws%s_%s.tif" % (attrName, self.grid_res, self.COREG_obj.win_size_XY, tilepos)
-        else:
-            fName_out = fName_out if fName_out else \
-                "Kriging__%s__grid%s_ws%s.tif" % (attrName, self.grid_res, self.COREG_obj.win_size_XY)
-        path_out = get_generic_outpath(dir_out=self.dir_out, fName_out=fName_out)
-        # add a half pixel grid points are centered on the output pixels
-        xmin = xmin - grid_res / 2
-        # ymin = ymin - grid_res / 2
-        # xmax = xmax + grid_res / 2
-        ymax = ymax + grid_res / 2
-
-        GeoArray(zvalues,
-                 geotransform=(xmin, grid_res, 0, ymax, 0, -grid_res),
-                 projection=self.COREG_obj.shift.prj).save(path_out)
-
-        return zvalues
-
-    def _Kriging_mp(self, args_kwargs_dict):
-        args = args_kwargs_dict.get('args', [])
-        kwargs = args_kwargs_dict.get('kwargs', [])
+        return TPGI.interpolate(metric=metric, method=method, plot_result=plot_result, lowres_spacing=lowres_spacing)
 
-        return self._Kriging_sp(*args, **kwargs)
+    @staticmethod
+    def to_Raster_using_Kriging(*args, **kwargs):
+        raise NotImplementedError('This method was removed in arosics version 1.8.2. To interpolate tie points into '
+                                  'space, you may now use Tie_Point_Grid.to_interpolated_raster() instead.')
 
 
 class Tie_Point_Refiner(object):
     """A class for performing outlier detection."""
 
     def __init__(self, GDF,
                  min_reliability=60,
                  rs_max_outlier: float = 10,
                  rs_tolerance: float = 2.5,
                  rs_max_iter: int = 15,
                  rs_exclude_previous_outliers: bool = True,
                  rs_timeout: float = 20,
+                 rs_random_state: Optional[int] = 0,
                  q: bool = False):
         """Get an instance of Tie_Point_Refiner.
 
         :param GDF:                             GeoDataFrame like TiePointGrid.CoRegPoints_table containing all tie
                                                 points to be filtered and the corresponding metadata
         :param min_reliability:                 minimum threshold for previously computed tie X/Y shift
                                                 reliability (default: 60%)
@@ -1052,24 +1013,27 @@
         :param rs_tolerance:                    RANSAC: percentage tolerance for max_outlier_percentage
                                                 (default: 2.5%)
         :param rs_max_iter:                     RANSAC: maximum iterations for finding the best RANSAC threshold
                                                 (default: 15)
         :param rs_exclude_previous_outliers:    RANSAC: whether to exclude points that have been flagged as
                                                 outlier by earlier filtering (default:True)
         :param rs_timeout:                      RANSAC: timeout for iteration loop in seconds (default: 20)
+        :param rs_random_state:                 RANSAC random state (an integer corresponds to a fixed/pseudo-random
+                                                state, None randomizes the result)
 
         :param q:
         """
         self.GDF = GDF.copy()
         self.min_reliability = min_reliability
         self.rs_max_outlier_percentage = rs_max_outlier
         self.rs_tolerance = rs_tolerance
         self.rs_max_iter = rs_max_iter
         self.rs_exclude_previous_outliers = rs_exclude_previous_outliers
         self.rs_timeout = rs_timeout
+        self.rs_random_state = rs_random_state
         self.q = q
         self.new_cols = []
         self.ransac_model_robust = None
 
     def run_filtering(self, level=3):
         """Filter tie points used for shift correction.
 
@@ -1181,15 +1145,15 @@
 
         model_robust, inliers = None, None
         count_inliers = None
         th = 5  # start RANSAC threshold
         th_checked = {}  # dict of thresholds that already have been tried + calculated inlier percentage
         th_substract = 2
         count_iter = 0
-        time_start = time.time()
+        time_start = time()
         ideal_count = min_inlier_percentage * src_coords.shape[0] / 100
 
         # optimize RANSAC threshold so that it marks not much more or less than the given outlier percentage
         while True:
             if th_checked:
                 th_too_strict = count_inliers < ideal_count  # True if too less inliers remaining
 
@@ -1234,15 +1198,16 @@
                            max_trials=2000,
                            stop_sample_num=int(
                                (min_inlier_percentage - self.rs_tolerance) /
                                100 * src_coords.shape[0]
                            ),
                            stop_residuals_sum=int(
                                (self.rs_max_outlier_percentage - self.rs_tolerance) /
-                               100 * src_coords.shape[0])
+                               100 * src_coords.shape[0]),
+                           random_state=self.rs_random_state
                            )
             else:
                 warnings.warn('RANSAC filtering could not be applied '
                               'because there were too few tie points to fit a model.')
                 inliers = np.array([])
                 break
 
@@ -1254,15 +1219,15 @@
             if min_inlier_percentage - self.rs_tolerance <\
                th_checked[th] <\
                min_inlier_percentage + self.rs_tolerance:
                 # print('in tolerance')
                 break
 
             if count_iter > self.rs_max_iter or \
-               time.time() - time_start > self.rs_timeout:
+               time() - time_start > self.rs_timeout:
                 break  # keep last values and break while loop
 
             count_iter += 1
 
         outliers = inliers.__eq__(False) if inliers is not None and inliers.size else np.array([])
 
         if inGDF.empty or outliers is None or \
@@ -1285,7 +1250,208 @@
 
         assert len(outseries) == len(self.GDF), \
             'RANSAC output validation failed.'
 
         self.ransac_model_robust = model_robust
 
         return outseries
+
+
+class Tie_Point_Grid_Interpolator(object):
+    """Class to interpolate tie point data into space."""
+
+    def __init__(self, tiepointgrid: Tie_Point_Grid, v: bool = False) -> None:
+        """Get an instance of Tie_Point_Grid_Interpolator.
+
+        :param tiepointgrid:    instance of Tie_Point_Grid after computing spatial shifts
+        :param v:               enable verbose mode
+        """
+        self.tpg = tiepointgrid
+        self.v = v
+
+    def interpolate(self,
+                    metric: str,
+                    method: str = 'RBF',
+                    plot_result: bool = False,
+                    lowres_spacing: int = 5
+                    ) -> np.array:
+        """Interpolate the point data of the given metric into space.
+
+        :param metric:          metric name to interpolate, i.e., one of the column names of
+                                Tie_Point_Grid.CoRegPoints_table, e.g., 'ABS_SHIFT'.
+        :param method:          interpolation algorithm
+                                - 'RBF' (Radial Basis Function)
+                                - 'GPR' (Gaussian Process Regression; equivalent to Simple Kriging)
+                                - 'Kriging' (Ordinary Kriging based on pykrige)
+        :param plot_result:     plot the result to assess the interpolation quality
+        :param lowres_spacing:  by default, RBF, GPR, and Kriging run a lower resolution which is then linearly
+                                interpolated to the full output image resolution. lowres_spacing defines the number of
+                                pixels between the low resolution grid points
+                                (higher values are faster but less accurate, default: 5)
+        :return:    interpolation result as numpy array in the X/Y dimension of the target image of the co-registration
+        """
+        t0 = time()
+
+        rows, cols, data = self._get_pointdata(metric)
+        nrows_out, ncols_out = self.tpg.shift.shape[:2]
+
+        rows_lowres = np.arange(0, nrows_out + lowres_spacing, lowres_spacing)
+        cols_lowres = np.arange(0, ncols_out + lowres_spacing, lowres_spacing)
+        args = rows, cols, data, rows_lowres, cols_lowres
+
+        if method == 'RBF':
+            data_lowres = self._interpolate_via_rbf(*args)
+        elif method == 'GPR':
+            data_lowres = self._interpolate_via_gpr(*args)
+        elif method == 'Kriging':
+            data_lowres = self._interpolate_via_kriging(*args)
+        else:
+            raise ValueError(method)
+
+        if lowres_spacing > 1:
+            rows_full = np.arange(nrows_out)
+            cols_full = np.arange(ncols_out)
+            data_full = self._interpolate_regulargrid(rows_lowres, cols_lowres, data_lowres, rows_full, cols_full)
+        else:
+            data_full = data_lowres
+
+        if self.v:
+            print('interpolation runtime: %.2fs' % (time() - t0))
+        if plot_result:
+            self._plot_interpolation_result(data_full, rows, cols, data, metric)
+
+        return data_full
+
+    def _get_pointdata(self, metric: str):
+        """Get the point data for the given metric from Tie_Point_Grid.CoRegPoints_table while ignoring outliers."""
+        tiepoints = self.tpg.CoRegPoints_table[self.tpg.CoRegPoints_table.OUTLIER.__eq__(False)].copy()
+
+        rows = np.array(tiepoints.Y_IM)
+        cols = np.array(tiepoints.X_IM)
+        data = np.array(tiepoints[metric])
+
+        return rows, cols, data
+
+    @staticmethod
+    def _plot_interpolation_result(data_full: np.ndarray,
+                                   rows: np.ndarray,
+                                   cols: np.ndarray,
+                                   data: np.ndarray,
+                                   metric: str
+                                   ):
+        """Plot the interpolation result together with the input point data."""
+        plt.figure(figsize=(7, 7))
+        im = plt.imshow(data_full)
+        plt.colorbar(im)
+        plt.scatter(cols, rows, c=data, edgecolors='black')
+        plt.title(metric)
+        plt.show()
+
+    @staticmethod
+    def _interpolate_regulargrid(rows: np.ndarray,
+                                 cols: np.ndarray,
+                                 data: np.ndarray,
+                                 rows_full: np.ndarray,
+                                 cols_full: np.ndarray
+                                 ):
+        """Run linear regular grid interpolation."""
+        RGI = RegularGridInterpolator(points=[cols, rows],
+                                      values=data.T,  # must be in shape [x, y]
+                                      method='linear',
+                                      bounds_error=False)
+        data_full = RGI(np.dstack(np.meshgrid(cols_full, rows_full)))
+        return data_full
+
+    @staticmethod
+    def _interpolate_via_rbf(rows: np.ndarray,
+                             cols: np.ndarray,
+                             data: np.ndarray,
+                             rows_full: np.ndarray,
+                             cols_full: np.ndarray
+                             ):
+        """Run Radial Basis Function (RBF) interpolation.
+
+        -> https://github.com/agile-geoscience/xlines/blob/master/notebooks/11_Gridding_map_data.ipynb
+        -> documents the legacy scipy.interpolate.Rbf
+        """
+        rbf = RBFInterpolator(
+            np.column_stack([cols, rows]), data,
+            kernel="linear",
+            # kernel="thin_plate_spline",
+        )
+        cols_grid, rows_grid = np.meshgrid(cols_full, rows_full)
+        data_full = \
+            rbf(np.column_stack([cols_grid.flat, rows_grid.flat]))\
+            .reshape(rows_grid.shape)
+
+        return data_full
+
+    @staticmethod
+    def _interpolate_via_gpr(rows: np.ndarray,
+                             cols: np.ndarray,
+                             data: np.ndarray,
+                             rows_full: np.ndarray,
+                             cols_full: np.ndarray
+                             ):
+        """Run Gaussian Process Regression (GPR) interpolation.
+
+        -> https://stackoverflow.com/questions/24978052/interpolation-over-regular-grid-in-python
+        """
+        try:
+            import sklearn  # noqa F401
+        except ModuleNotFoundError:
+            raise ModuleNotFoundError(
+                "GPR interpolation requires the optional package 'scikit-learn' to be installed. You may install it "
+                "with Conda (conda install -c conda-forge scikit-learn) or Pip (pip install scikit-learn)."
+            )
+
+        from sklearn.gaussian_process.kernels import RBF
+        from sklearn.gaussian_process import GaussianProcessRegressor
+
+        gp = GaussianProcessRegressor(
+            normalize_y=False,
+            alpha=0.001,  # Larger values imply more input noise and result in smoother grids; default: 1e-10
+            kernel=RBF(length_scale=100))
+        gp.fit(np.column_stack([cols, rows]), data.T)
+
+        cols_grid, rows_grid = np.meshgrid(cols_full, rows_full)
+        data_full = \
+            gp.predict(np.column_stack([cols_grid.flat, rows_grid.flat]))\
+            .reshape(rows_grid.shape)
+
+        return data_full
+
+    @staticmethod
+    def _interpolate_via_kriging(rows: np.ndarray,
+                                 cols: np.ndarray,
+                                 data: np.ndarray,
+                                 rows_full: np.ndarray,
+                                 cols_full: np.ndarray
+                                 ):
+        """Run Ordinary Kriging interpolation based on pykrige.
+
+        Reference: P.K. Kitanidis, Introduction to Geostatistics: Applications in Hydrogeology,
+                   (Cambridge University Press, 1997) 272 p.
+        """
+        try:
+            import pykrige  # noqa F401
+        except ModuleNotFoundError:
+            raise ModuleNotFoundError(
+                "Ordinary Kriging requires the optional package 'pykrige' to be installed. You may install it with "
+                "Conda (conda install -c conda-forge pykrige) or Pip (pip install pykrige)."
+            )
+
+        from pykrige.ok import OrdinaryKriging
+
+        OK = OrdinaryKriging(cols.astype(float), rows.astype(float), data.astype(float),
+                             variogram_model='spherical',
+                             verbose=False)
+
+        data_full, sigmasq = \
+            OK.execute('grid',
+                       cols_full.astype(float),
+                       rows_full.astype(float),
+                       backend='C',
+                       # n_closest_points=12
+                       )
+
+        return data_full
```

### Comparing `arosics-1.8.1/arosics/__init__.py` & `arosics-1.9.0/arosics/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Top-level package for arosics."""
 
 import warnings as _warnings
 from pkgutil import find_loader as _find_loader
+import os as __os
 
 from arosics.CoReg import COREG
 from arosics.CoReg_local import COREG_LOCAL
 from arosics.DeShifter import DESHIFTER
 from arosics.Tie_Point_Grid import Tie_Point_Grid
 
 from .version import __version__, __versionalias__   # noqa (E402 + F401)
@@ -43,7 +44,14 @@
            'DESHIFTER',
            'Tie_Point_Grid']
 
 
 # check optional dependencies
 if not _find_loader('pyfftw'):
     _warnings.warn('PYFFTW library is missing. However, coregistration works. But in some cases it can be much slower.')
+
+
+# $PROJ_LIB was renamed to $PROJ_DATA in proj=9.1.1, which leads to issues with fiona>=1.8.20,<1.9
+# https://github.com/conda-forge/pyproj-feedstock/issues/130
+# -> fix it by setting PROJ_DATA
+if 'GDAL_DATA' in __os.environ and 'PROJ_DATA' not in __os.environ and 'PROJ_LIB' not in __os.environ:
+    __os.environ['PROJ_DATA'] = __os.path.join(__os.path.dirname(__os.environ['GDAL_DATA']), 'proj')
```

### Comparing `arosics-1.8.1/arosics/arosics_cli.py` & `arosics-1.9.0/arosics/arosics_cli.py`

 * *Files identical despite different names*

### Comparing `arosics-1.8.1/arosics/geometry.py` & `arosics-1.9.0/arosics/geometry.py`

 * *Files identical despite different names*

### Comparing `arosics-1.8.1/arosics/plotting.py` & `arosics-1.9.0/arosics/plotting.py`

 * *Files identical despite different names*

### Comparing `arosics-1.8.1/arosics/version.py` & `arosics-1.9.0/arosics/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,9 +20,9 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '1.8.1'
-__versionalias__ = '2023-03-10_01'
+__version__ = '1.9.0'
+__versionalias__ = '2023-05-04_01'
```

### Comparing `arosics-1.8.1/arosics.egg-info/PKG-INFO` & `arosics-1.9.0/arosics.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: arosics
-Version: 1.8.1
+Version: 1.9.0
 Summary: An Automated and Robust Open-Source Image Co-Registration Software for Multi-Sensor Satellite Data
 Home-page: https://git.gfz-potsdam.de/danschef/arosics
 Author: Daniel Scheffler
 Author-email: daniel.scheffler@gfz-potsdam.de
 License: Apache-2.0
 Project-URL: Source code, https://git.gfz-potsdam.de/danschef/arosics
 Project-URL: Issue Tracker, https://git.gfz-potsdam.de/danschef/arosics/-/issues
 Project-URL: Documentation, https://danschef.git-pages.gfz-potsdam.de/arosics/doc/
-Project-URL: Change log, https://git.gfz-potsdam.de/danschef/arosics/-/blob/master/HISTORY.rst
+Project-URL: Change log, https://git.gfz-potsdam.de/danschef/arosics/-/blob/main/HISTORY.rst
 Project-URL: Algorithm paper, https://www.mdpi.com/2072-4292/9/7/676
 Project-URL: Zenodo, https://zenodo.org/record/5093940
 Keywords: arosics,image co-registration,geometric pre-processing,remote sensing,sensor fusion
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: Apache Software License
@@ -43,35 +43,35 @@
 * Free software: Apache 2.0
 * **Documentation:** https://danschef.git-pages.gfz-potsdam.de/arosics/doc/
 * The (open-access) **paper** corresponding to this software repository can be found here:
   `Scheffler et al. 2017 <https://www.mdpi.com/2072-4292/9/7/676>`__
   (cite as: Scheffler D, Hollstein A, Diedrich H, Segl K, Hostert P. AROSICS: An Automated and Robust Open-Source
   Image Co-Registration Software for Multi-Sensor Satellite Data. Remote Sensing. 2017; 9(7):676).
 * Information on how to **cite the AROSICS Python package** can be found in the
-  `CITATION <https://git.gfz-potsdam.de/danschef/arosics/-/blob/master/CITATION>`__ file.
+  `CITATION <https://git.gfz-potsdam.de/danschef/arosics/-/blob/main/CITATION>`__ file.
 * Submit feedback by filing an issue `here <https://git.gfz-potsdam.de/danschef/arosics/issues>`__
   or join our chat here: |Gitter|
 
 .. |Gitter| image:: https://badges.gitter.im/Join%20Chat.svg
     :target: https://gitter.im/arosics/Lobby?utm_source=share-link&utm_medium=link&utm_campaign=share-link
     :alt: https://gitter.im/arosics/Lobby?utm_source=share-link&utm_medium=link&utm_campaign=share-link
 
 Status
 ------
 
-.. image:: https://git.gfz-potsdam.de/danschef/arosics/badges/master/pipeline.svg
-        :target: https://git.gfz-potsdam.de/danschef/arosics/commits/master
-.. image:: https://git.gfz-potsdam.de/danschef/arosics/badges/master/coverage.svg
+.. image:: https://git.gfz-potsdam.de/danschef/arosics/badges/main/pipeline.svg
+        :target: https://git.gfz-potsdam.de/danschef/arosics/commits/main
+.. image:: https://git.gfz-potsdam.de/danschef/arosics/badges/main/coverage.svg
         :target: https://danschef.git-pages.gfz-potsdam.de/arosics/coverage/
 .. image:: https://img.shields.io/pypi/v/arosics.svg
         :target: https://pypi.python.org/pypi/arosics
 .. image:: https://img.shields.io/conda/vn/conda-forge/arosics.svg
         :target: https://anaconda.org/conda-forge/arosics
 .. image:: https://img.shields.io/pypi/l/arosics.svg
-        :target: https://git.gfz-potsdam.de/danschef/arosics/blob/master/LICENSE
+        :target: https://git.gfz-potsdam.de/danschef/arosics/blob/main/LICENSE
 .. image:: https://img.shields.io/pypi/pyversions/arosics.svg
         :target: https://img.shields.io/pypi/pyversions/arosics.svg
 .. image:: https://img.shields.io/pypi/dm/arosics.svg
         :target: https://pypi.python.org/pypi/arosics
 .. image:: https://zenodo.org/badge/253474603.svg
         :target: https://zenodo.org/badge/latestdoi/253474603
 
@@ -99,39 +99,39 @@
 This allows very fast co-registration but only corrects for translational (global) X/Y shifts.
 The calculated subpixel-shifts are (by default) applied to the geocoding information of the output image.
 No spatial resampling is done automatically as long as both input images have the same projection. However, AROSICS
 also allows to align the output image to the reference image coordinate grid if needed.
 
 Here is an example of a Landsat-8 / Sentinel-2 image pair before and after co-registration using AROSICS:
 
-.. image:: https://git.gfz-potsdam.de/danschef/arosics/raw/master/docs/images/animation_testcase1_zoom_L8_S2_global_coreg_before_after_900x456.gif
+.. image:: https://git.gfz-potsdam.de/danschef/arosics/raw/main/docs/images/animation_testcase1_zoom_L8_S2_global_coreg_before_after_900x456.gif
 
 
 Local co-registration - for spatially variable shifts but a bit slower
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 A dense grid of tie points is automatically computed, whereas tie points are subsequently validated using a
 multistage workflow. Only those tie points not marked as false-positives are used to compute the parameters of an
 affine transformation. Warping of the target image is done using an appropriate resampling technique
 (cubic by default).
 
 Here is an example of the computed shift vectors after filtering false-positives
 (mainly due to clouds in the target image):
 
-.. image:: https://git.gfz-potsdam.de/danschef/arosics/raw/master/docs/images/shift_vectors_testcase1__900x824.gif
+.. image:: https://git.gfz-potsdam.de/danschef/arosics/raw/main/docs/images/shift_vectors_testcase1__900x824.gif
 
 
 For further details check out the `documentation <https://danschef.git-pages.gfz-potsdam.de/arosics/doc/>`__!
 
 
 History / Changelog
 -------------------
 
 You can find the protocol of recent changes in the AROSICS package
-`here <https://git.gfz-potsdam.de/danschef/arosics/-/blob/master/HISTORY.rst>`__.
+`here <https://git.gfz-potsdam.de/danschef/arosics/-/blob/main/HISTORY.rst>`__.
 
 
 Credits
 -------
 
 AROSICS was developed by Daniel Scheffler (German Research Centre of Geosciences) within the context of the
 `GeoMultiSens <http://www.geomultisens.gfz-potsdam.de/>`__ project funded by the German Federal Ministry of Education and Research
```

### Comparing `arosics-1.8.1/arosics.egg-info/SOURCES.txt` & `arosics-1.9.0/arosics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arosics-1.8.1/arosics.egg-info/requires.txt` & `arosics-1.9.0/arosics.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 pandas
 plotly
 pyfftw
 pykrige
 pyproj>2.2.0
 py_tools_ds>=0.18.0
 scikit-image>=0.16.0
+scikit-learn
+scipy
 shapely
 
 [dev]
 setuptools
 setuptools-git
 pytest
 pytest-cov
```

### Comparing `arosics-1.8.1/docs/Makefile` & `arosics-1.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `arosics-1.8.1/docs/_build/html/_images/CoregPoints_table.png` & `arosics-1.9.0/docs/_build/html/_images/CoregPoints_table.png`

 * *Files identical despite different names*

### Comparing `arosics-1.8.1/docs/_build/html/_images/animation_testcase1_zoom_L8_S2_global_coreg_before_after_900x456.gif` & `arosics-1.9.0/docs/_build/html/_images/animation_testcase1_zoom_L8_S2_global_coreg_before_after_900x456.gif`

 * *Files identical despite different names*

### Comparing `arosics-1.8.1/docs/_build/html/_images/arosics_logo.png` & `arosics-1.9.0/docs/_build/html/_images/arosics_logo.png`

 * *Files identical despite different names*

### Comparing `arosics-1.8.1/docs/_build/html/_images/output_40_1.png` & `arosics-1.9.0/docs/_build/html/_images/output_40_1.png`

 * *Files identical despite different names*

### Comparing `arosics-1.8.1/docs/_build/html/_images/output_44_1.png` & `arosics-1.9.0/docs/_build/html/_images/output_44_1.png`

 * *Files identical despite different names*

### Comparing `arosics-1.8.1/docs/_build/html/_images/shift_vectors_testcase1__900x824.gif` & `arosics-1.9.0/docs/_build/html/_images/shift_vectors_testcase1__900x824.gif`

 * *Files identical despite different names*

### Comparing `arosics-1.8.1/docs/_build/html/_static/arosics_logo.png` & `arosics-1.9.0/docs/_build/html/_static/arosics_logo.png`

 * *Files identical despite different names*

### Comparing `arosics-1.8.1/docs/about.rst` & `arosics-1.9.0/docs/about.rst`

 * *Files identical despite different names*

### Comparing `arosics-1.8.1/docs/cli_reference.rst` & `arosics-1.9.0/docs/cli_reference.rst`

 * *Files identical despite different names*

### Comparing `arosics-1.8.1/docs/conf.py` & `arosics-1.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `arosics-1.8.1/docs/images/CoregPoints_table.png` & `arosics-1.9.0/docs/images/CoregPoints_table.png`

 * *Files identical despite different names*

### Comparing `arosics-1.8.1/docs/images/animation_testcase1_zoom_L8_S2_global_coreg_before_after_1066x540.gif` & `arosics-1.9.0/docs/images/animation_testcase1_zoom_L8_S2_global_coreg_before_after_1066x540.gif`

 * *Files identical despite different names*

### Comparing `arosics-1.8.1/docs/images/animation_testcase1_zoom_L8_S2_global_coreg_before_after_900x456.gif` & `arosics-1.9.0/docs/images/animation_testcase1_zoom_L8_S2_global_coreg_before_after_900x456.gif`

 * *Files identical despite different names*

### Comparing `arosics-1.8.1/docs/images/arosics_logo.png` & `arosics-1.9.0/docs/images/arosics_logo.png`

 * *Files identical despite different names*

### Comparing `arosics-1.8.1/docs/images/output_40_1.png` & `arosics-1.9.0/docs/images/output_40_1.png`

 * *Files identical despite different names*

### Comparing `arosics-1.8.1/docs/images/output_44_1.png` & `arosics-1.9.0/docs/images/output_44_1.png`

 * *Files identical despite different names*

### Comparing `arosics-1.8.1/docs/images/shift_vectors_testcase1__900x824.gif` & `arosics-1.9.0/docs/images/shift_vectors_testcase1__900x824.gif`

 * *Files identical despite different names*

### Comparing `arosics-1.8.1/docs/installation.rst` & `arosics-1.9.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `arosics-1.8.1/docs/make.bat` & `arosics-1.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `arosics-1.8.1/docs/usage/global_coreg.rst` & `arosics-1.9.0/docs/usage/global_coreg.rst`

 * *Files identical despite different names*

### Comparing `arosics-1.8.1/docs/usage/input_data_requirements.rst` & `arosics-1.9.0/docs/usage/input_data_requirements.rst`

 * *Files identical despite different names*

### Comparing `arosics-1.8.1/docs/usage/local_coreg.rst` & `arosics-1.9.0/docs/usage/local_coreg.rst`

 * *Files identical despite different names*

### Comparing `arosics-1.8.1/docs/usage.rst` & `arosics-1.9.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `arosics-1.8.1/setup.py` & `arosics-1.9.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,14 +54,16 @@
     'pandas',
     'plotly',
     'pyfftw',
     'pykrige',
     'pyproj>2.2.0',
     'py_tools_ds>=0.18.0',
     'scikit-image>=0.16.0',
+    'scikit-learn',
+    'scipy',
     'shapely',
 ]
 
 req_setup = [
     'setuptools',
     'setuptools-git'
 ]
@@ -111,15 +113,15 @@
     long_description=readme,
     name='arosics',
     packages=find_packages(exclude=['tests*']),
     project_urls={
         "Source code": "https://git.gfz-potsdam.de/danschef/arosics",
         "Issue Tracker": "https://git.gfz-potsdam.de/danschef/arosics/-/issues",
         "Documentation": "https://danschef.git-pages.gfz-potsdam.de/arosics/doc/",
-        "Change log": "https://git.gfz-potsdam.de/danschef/arosics/-/blob/master/HISTORY.rst",
+        "Change log": "https://git.gfz-potsdam.de/danschef/arosics/-/blob/main/HISTORY.rst",
         "Algorithm paper": "https://www.mdpi.com/2072-4292/9/7/676",
         "Zenodo": "https://zenodo.org/record/5093940"
     },
     python_requires='>3.8',
     setup_requires=req_setup,
     test_suite='tests',
     tests_require=req + req_test,
```

