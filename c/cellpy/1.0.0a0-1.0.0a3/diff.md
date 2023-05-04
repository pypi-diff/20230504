# Comparing `tmp/cellpy-1.0.0a0.tar.gz` & `tmp/cellpy-1.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellpy-1.0.0a0.tar", last modified: Mon May  1 14:46:53 2023, max compression
+gzip compressed data, was "cellpy-1.0.0a3.tar", last modified: Thu May  4 13:01:03 2023, max compression
```

## Comparing `cellpy-1.0.0a0.tar` & `cellpy-1.0.0a3.tar`

### file list

```diff
@@ -1,215 +1,215 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 14:46:53.558574 cellpy-1.0.0a0/
--rw-rw-rw-   0        0        0      480 2023-05-01 14:07:00.000000 cellpy-1.0.0a0/AUTHORS.rst
--rw-rw-rw-   0        0        0     3086 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     3908 2023-05-01 13:41:10.000000 cellpy-1.0.0a0/HISTORY.rst
--rw-rw-rw-   0        0        0     1089 2021-12-21 09:11:58.000000 cellpy-1.0.0a0/LICENSE
--rw-rw-rw-   0        0        0      645 2022-05-27 12:07:50.000000 cellpy-1.0.0a0/MANIFEST.in
--rw-rw-rw-   0        0        0     6518 2023-05-01 14:46:53.557561 cellpy-1.0.0a0/PKG-INFO
--rw-rw-rw-   0        0        0     1872 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-01 14:46:53.248331 cellpy-1.0.0a0/cellpy/
--rw-rw-rw-   0        0        0      805 2023-04-30 13:34:58.000000 cellpy-1.0.0a0/cellpy/__init__.py
--rw-rw-rw-   0        0        0       24 2023-04-30 13:34:58.000000 cellpy-1.0.0a0/cellpy/_version.py
--rw-rw-rw-   0        0        0    53661 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/cellpy/cli.py
--rw-rw-rw-   0        0        0     1228 2023-04-30 13:34:58.000000 cellpy-1.0.0a0/cellpy/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-01 14:46:53.260332 cellpy-1.0.0a0/cellpy/internals/
--rw-rw-rw-   0        0        0        0 2023-04-30 13:34:58.000000 cellpy-1.0.0a0/cellpy/internals/__init__.py
--rw-rw-rw-   0        0        0    24093 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/cellpy/internals/core.py
--rw-rw-rw-   0        0        0     4838 2023-04-30 13:34:58.000000 cellpy-1.0.0a0/cellpy/log.py
--rw-rw-rw-   0        0        0     1750 2021-12-21 09:11:58.000000 cellpy-1.0.0a0/cellpy/logging.json
-drwxrwxrwx   0        0        0        0 2023-05-01 14:46:53.268333 cellpy-1.0.0a0/cellpy/parameters/
--rw-rw-rw-   0        0        0     3301 2023-04-30 13:34:58.000000 cellpy-1.0.0a0/cellpy/parameters/.cellpy_prms_default.conf
--rw-rw-rw-   0        0        0        2 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/cellpy/parameters/__init__.py
--rw-rw-rw-   0        0        0    23361 2023-04-30 13:34:58.000000 cellpy-1.0.0a0/cellpy/parameters/internal_settings.py
-drwxrwxrwx   0        0        0        0 2023-05-01 14:46:53.271331 cellpy-1.0.0a0/cellpy/parameters/legacy/
--rw-rw-rw-   0        0        0        0 2021-12-21 09:11:58.000000 cellpy-1.0.0a0/cellpy/parameters/legacy/__init__.py
--rw-rw-rw-   0        0        0    24146 2023-04-30 13:34:58.000000 cellpy-1.0.0a0/cellpy/parameters/legacy/update_headers.py
--rw-rw-rw-   0        0        0    12410 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/cellpy/parameters/prmreader.py
--rw-rw-rw-   0        0        0    12593 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/cellpy/parameters/prms.py
-drwxrwxrwx   0        0        0        0 2023-05-01 14:46:53.282337 cellpy-1.0.0a0/cellpy/readers/
--rw-rw-rw-   0        0        0        2 2021-12-21 09:11:58.000000 cellpy-1.0.0a0/cellpy/readers/__init__.py
--rw-rw-rw-   0        0        0   227868 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/cellpy/readers/cellreader.py
--rw-rw-rw-   0        0        0    39447 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/cellpy/readers/core.py
--rw-rw-rw-   0        0        0    22998 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/cellpy/readers/dbreader.py
--rw-rw-rw-   0        0        0     9448 2023-04-30 13:34:58.000000 cellpy-1.0.0a0/cellpy/readers/filefinder.py
-drwxrwxrwx   0        0        0        0 2023-05-01 14:46:53.308331 cellpy-1.0.0a0/cellpy/readers/instruments/
--rw-rw-rw-   0        0        0        0 2021-12-21 09:11:58.000000 cellpy-1.0.0a0/cellpy/readers/instruments/__init__.py
--rw-rw-rw-   0        0        0    50849 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/cellpy/readers/instruments/arbin_res.py
--rw-rw-rw-   0        0        0    19381 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/cellpy/readers/instruments/arbin_sql.py
--rw-rw-rw-   0        0        0    21062 2023-04-30 13:34:58.000000 cellpy-1.0.0a0/cellpy/readers/instruments/arbin_sql_7.py
--rw-rw-rw-   0        0        0    11134 2023-04-30 13:34:58.000000 cellpy-1.0.0a0/cellpy/readers/instruments/arbin_sql_csv.py
--rw-rw-rw-   0        0        0     7126 2023-04-30 13:34:58.000000 cellpy-1.0.0a0/cellpy/readers/instruments/arbin_sql_h5.py
--rw-rw-rw-   0        0        0     9883 2023-04-30 13:34:58.000000 cellpy-1.0.0a0/cellpy/readers/instruments/arbin_sql_xlsx.py
--rw-rw-rw-   0        0        0    27501 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/cellpy/readers/instruments/base.py
--rw-rw-rw-   0        0        0    22693 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/cellpy/readers/instruments/biologics_mpr.py
-drwxrwxrwx   0        0        0        0 2023-05-01 14:46:53.321083 cellpy-1.0.0a0/cellpy/readers/instruments/configurations/
--rw-rw-rw-   0        0        0     6607 2022-06-03 19:58:41.000000 cellpy-1.0.0a0/cellpy/readers/instruments/configurations/__init__.py
--rw-rw-rw-   0        0        0     1700 2023-04-30 13:34:58.000000 cellpy-1.0.0a0/cellpy/readers/instruments/configurations/maccor_txt_four.py
--rw-rw-rw-   0        0        0     4084 2023-04-30 13:34:58.000000 cellpy-1.0.0a0/cellpy/readers/instruments/configurations/maccor_txt_one.py
--rw-rw-rw-   0        0        0     1990 2023-04-30 13:34:58.000000 cellpy-1.0.0a0/cellpy/readers/instruments/configurations/maccor_txt_three.py
--rw-rw-rw-   0        0        0     1788 2023-04-30 13:34:58.000000 cellpy-1.0.0a0/cellpy/readers/instruments/configurations/maccor_txt_two.py
--rw-rw-rw-   0        0        0     3549 2023-04-30 13:34:58.000000 cellpy-1.0.0a0/cellpy/readers/instruments/configurations/maccor_txt_zero.py
--rw-rw-rw-   0        0        0     2132 2023-04-30 13:34:58.000000 cellpy-1.0.0a0/cellpy/readers/instruments/configurations/neware_txt_zero.py
--rw-rw-rw-   0        0        0    10327 2023-04-30 13:34:58.000000 cellpy-1.0.0a0/cellpy/readers/instruments/custom.py
--rw-rw-rw-   0        0        0     3760 2023-04-30 13:34:58.000000 cellpy-1.0.0a0/cellpy/readers/instruments/ext_nda_reader.py
-drwxrwxrwx   0        0        0        0 2023-05-01 14:46:53.324137 cellpy-1.0.0a0/cellpy/readers/instruments/loader_specific_modules/
--rw-rw-rw-   0        0        0        0 2022-06-03 19:58:41.000000 cellpy-1.0.0a0/cellpy/readers/instruments/loader_specific_modules/__init__.py
--rw-rw-rw-   0        0        0    22115 2022-06-03 19:58:41.000000 cellpy-1.0.0a0/cellpy/readers/instruments/loader_specific_modules/biologic_file_format.py
--rw-rw-rw-   0        0        0     1067 2023-04-30 13:34:58.000000 cellpy-1.0.0a0/cellpy/readers/instruments/local_instrument.py
--rw-rw-rw-   0        0        0    12886 2023-04-30 13:34:58.000000 cellpy-1.0.0a0/cellpy/readers/instruments/maccor_txt.py
--rw-rw-rw-   0        0        0     3488 2023-04-30 13:34:58.000000 cellpy-1.0.0a0/cellpy/readers/instruments/neware_txt.py
--rw-rw-rw-   0        0        0    16769 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/cellpy/readers/instruments/pec_csv.py
-drwxrwxrwx   0        0        0        0 2023-05-01 14:46:53.329260 cellpy-1.0.0a0/cellpy/readers/instruments/processors/
--rw-rw-rw-   0        0        0        0 2022-05-27 12:07:50.000000 cellpy-1.0.0a0/cellpy/readers/instruments/processors/__init__.py
--rw-rw-rw-   0        0        0    15265 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/cellpy/readers/instruments/processors/post_processors.py
--rw-rw-rw-   0        0        0     1450 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/cellpy/readers/instruments/processors/pre_processors.py
--rw-rw-rw-   0        0        0    26852 2023-04-30 13:34:58.000000 cellpy-1.0.0a0/cellpy/readers/sql_dbreader.py
-drwxrwxrwx   0        0        0        0 2023-05-01 14:46:53.354259 cellpy-1.0.0a0/cellpy/utils/
--rw-rw-rw-   0        0        0      192 2021-12-21 09:11:58.000000 cellpy-1.0.0a0/cellpy/utils/__init__.py
--rw-rw-rw-   0        0        0    49251 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/cellpy/utils/batch.py
-drwxrwxrwx   0        0        0        0 2023-05-01 14:46:53.376257 cellpy-1.0.0a0/cellpy/utils/batch_tools/
--rw-rw-rw-   0        0        0        0 2021-12-21 09:11:58.000000 cellpy-1.0.0a0/cellpy/utils/batch_tools/__init__.py
--rw-rw-rw-   0        0        0     7578 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/cellpy/utils/batch_tools/batch_analyzers.py
--rw-rw-rw-   0        0        0    19566 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/cellpy/utils/batch_tools/batch_core.py
--rw-rw-rw-   0        0        0    40821 2023-04-30 13:34:58.000000 cellpy-1.0.0a0/cellpy/utils/batch_tools/batch_experiments.py
--rw-rw-rw-   0        0        0     2931 2023-04-30 13:34:58.000000 cellpy-1.0.0a0/cellpy/utils/batch_tools/batch_exporters.py
--rw-rw-rw-   0        0        0    13909 2023-04-30 13:34:58.000000 cellpy-1.0.0a0/cellpy/utils/batch_tools/batch_helpers.py
--rw-rw-rw-   0        0        0    28305 2023-04-30 13:34:58.000000 cellpy-1.0.0a0/cellpy/utils/batch_tools/batch_journals.py
--rw-rw-rw-   0        0        0    29066 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/cellpy/utils/batch_tools/batch_plotters.py
--rw-rw-rw-   0        0        0      245 2021-12-21 09:11:58.000000 cellpy-1.0.0a0/cellpy/utils/batch_tools/batch_reporters.py
--rw-rw-rw-   0        0        0     3339 2022-05-27 12:03:59.000000 cellpy-1.0.0a0/cellpy/utils/batch_tools/dumpers.py
--rw-rw-rw-   0        0        0    10117 2023-04-30 13:34:58.000000 cellpy-1.0.0a0/cellpy/utils/batch_tools/engines.py
--rw-rw-rw-   0        0        0     5294 2023-04-30 13:34:58.000000 cellpy-1.0.0a0/cellpy/utils/batch_tools/sqlite_from_excel_db.py
--rw-rw-rw-   0        0        0    63308 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/cellpy/utils/collectors.py
--rw-rw-rw-   0        0        0    45461 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/cellpy/utils/collectors_old.py
-drwxrwxrwx   0        0        0        0 2023-05-01 14:46:53.378258 cellpy-1.0.0a0/cellpy/utils/data/
--rw-rw-rw-   0        0        0  3700143 2023-04-30 18:07:05.000000 cellpy-1.0.0a0/cellpy/utils/data/20160805_test001_45_cc.h5
-drwxrwxrwx   0        0        0        0 2023-05-01 14:46:53.388258 cellpy-1.0.0a0/cellpy/utils/data/raw/
--rw-rw-rw-   0        0        0  1613824 2021-12-21 09:11:58.000000 cellpy-1.0.0a0/cellpy/utils/data/raw/20160805_test001_45_cc_01.res
--rw-rw-rw-   0        0        0      260 2022-05-27 12:07:50.000000 cellpy-1.0.0a0/cellpy/utils/diagnostics.py
--rw-rw-rw-   0        0        0    79016 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/cellpy/utils/easyplot.py
--rw-rw-rw-   0        0        0     1576 2023-04-30 13:34:58.000000 cellpy-1.0.0a0/cellpy/utils/example_data.py
--rw-rw-rw-   0        0        0    39446 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/cellpy/utils/helpers.py
--rw-rw-rw-   0        0        0    38967 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/cellpy/utils/ica.py
--rw-rw-rw-   0        0        0      189 2022-05-27 12:07:50.000000 cellpy-1.0.0a0/cellpy/utils/live.py
--rw-rw-rw-   0        0        0    24037 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/cellpy/utils/ocv_rlx.py
--rw-rw-rw-   0        0        0    45397 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/cellpy/utils/plotutils.py
--rw-rw-rw-   0        0        0     1787 2023-04-30 13:34:58.000000 cellpy-1.0.0a0/cellpy/utils/processor.py
-drwxrwxrwx   0        0        0        0 2023-05-01 14:46:53.258332 cellpy-1.0.0a0/cellpy.egg-info/
--rw-rw-rw-   0        0        0     6518 2023-05-01 14:46:52.000000 cellpy-1.0.0a0/cellpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7846 2023-05-01 14:46:53.000000 cellpy-1.0.0a0/cellpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 14:46:52.000000 cellpy-1.0.0a0/cellpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-05-01 14:46:52.000000 cellpy-1.0.0a0/cellpy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-05-01 14:46:52.000000 cellpy-1.0.0a0/cellpy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      337 2023-05-01 14:46:52.000000 cellpy-1.0.0a0/cellpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-01 14:46:52.000000 cellpy-1.0.0a0/cellpy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-01 14:46:53.401260 cellpy-1.0.0a0/docs/
--rw-rw-rw-   0        0        0     6939 2022-09-20 08:21:07.000000 cellpy-1.0.0a0/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-05-01 14:46:53.222812 cellpy-1.0.0a0/docs/_build/
-drwxrwxrwx   0        0        0        0 2023-05-01 14:46:53.221812 cellpy-1.0.0a0/docs/_build/.doctrees/
-drwxrwxrwx   0        0        0        0 2023-05-01 14:46:53.409259 cellpy-1.0.0a0/docs/_build/.doctrees/nbsphinx/
--rw-rw-rw-   0        0        0    15014 2023-04-30 13:53:57.000000 cellpy-1.0.0a0/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_6_0.png
--rw-rw-rw-   0        0        0    14599 2023-04-30 13:53:57.000000 cellpy-1.0.0a0/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_7_0.png
--rw-rw-rw-   0        0        0    13527 2023-04-30 13:53:57.000000 cellpy-1.0.0a0/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_8_0.png
--rw-rw-rw-   0        0        0    25669 2023-04-30 13:54:02.000000 cellpy-1.0.0a0/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_simple_plot_2_0.png
-drwxrwxrwx   0        0        0        0 2023-05-01 14:46:53.444899 cellpy-1.0.0a0/docs/_build/_images/
--rw-rw-rw-   0        0        0    15014 2023-04-27 15:02:55.000000 cellpy-1.0.0a0/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_6_0.png
--rw-rw-rw-   0        0        0    14599 2023-04-27 15:02:55.000000 cellpy-1.0.0a0/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_7_0.png
--rw-rw-rw-   0        0        0    13527 2023-04-27 15:02:55.000000 cellpy-1.0.0a0/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_8_0.png
--rw-rw-rw-   0        0        0    25669 2023-04-27 15:03:02.000000 cellpy-1.0.0a0/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_simple_plot_2_0.png
--rw-rw-rw-   0        0        0    11678 2023-04-29 14:19:31.000000 cellpy-1.0.0a0/docs/_build/_images/graphviz-22185705e237fa530df24e4af50cb25833165e25.png
--rw-rw-rw-   0        0        0    22040 2023-04-29 14:33:27.000000 cellpy-1.0.0a0/docs/_build/_images/graphviz-246f2486cd940f2ea40a07f847c86c22b2607ca8.png
--rw-rw-rw-   0        0        0    21790 2023-04-29 14:26:00.000000 cellpy-1.0.0a0/docs/_build/_images/graphviz-42e9bc826d476a3d361a7f410e989ed34dc1aa85.png
--rw-rw-rw-   0        0        0    32991 2023-04-29 14:26:01.000000 cellpy-1.0.0a0/docs/_build/_images/graphviz-619216a42370fd49669c083549129b8470c8fae1.png
--rw-rw-rw-   0        0        0    32991 2023-04-30 20:02:23.000000 cellpy-1.0.0a0/docs/_build/_images/graphviz-6412a7c74952b4793798e9032f5bc4e7a1ab70c1.png
--rw-rw-rw-   0        0        0     7231 2023-04-29 14:12:31.000000 cellpy-1.0.0a0/docs/_build/_images/graphviz-6deb64a460668e8ef9bf0ca653314119adeeae66.png
--rw-rw-rw-   0        0        0    13360 2023-04-29 14:36:26.000000 cellpy-1.0.0a0/docs/_build/_images/graphviz-83b62e03ef369ff0a30f027892dba95b91ea8b6c.png
--rw-rw-rw-   0        0        0    21790 2023-04-30 20:02:22.000000 cellpy-1.0.0a0/docs/_build/_images/graphviz-8ec82d564b1a6ea5b95a36a4a213f7a78aaedc63.png
--rw-rw-rw-   0        0        0     5391 2023-04-29 14:10:02.000000 cellpy-1.0.0a0/docs/_build/_images/graphviz-ce8a9fe2ba01194aed847e0248d749db4093aca1.png
--rw-rw-rw-   0        0        0    20826 2023-04-29 14:29:06.000000 cellpy-1.0.0a0/docs/_build/_images/graphviz-e94a5352318e02fcc5ef1f813e02a526c39af791.png
--rw-rw-rw-   0        0        0    88743 2023-04-19 13:49:30.000000 cellpy-1.0.0a0/docs/_build/_images/templates_jupyterlab_001.png
--rw-rw-rw-   0        0        0   296908 2022-05-27 12:07:51.000000 cellpy-1.0.0a0/docs/_build/_images/tutorials_utils_plotting_fig1.png
--rw-rw-rw-   0        0        0    54588 2022-05-27 12:07:51.000000 cellpy-1.0.0a0/docs/_build/_images/tutorials_utils_plotting_fig2.png
-drwxrwxrwx   0        0        0        0 2023-05-01 14:46:53.450047 cellpy-1.0.0a0/docs/_build/_static/
--rw-rw-rw-   0        0        0      286 2023-04-25 11:20:36.000000 cellpy-1.0.0a0/docs/_build/_static/file.png
--rw-rw-rw-   0        0        0       90 2023-04-25 11:20:36.000000 cellpy-1.0.0a0/docs/_build/_static/minus.png
--rw-rw-rw-   0        0        0       90 2023-04-25 11:20:36.000000 cellpy-1.0.0a0/docs/_build/_static/plus.png
--rw-rw-rw-   0        0        0     1695 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/docs/adapted_readme.rst
--rw-rw-rw-   0        0        0    10731 2023-04-30 13:34:58.000000 cellpy-1.0.0a0/docs/conf.py
-drwxrwxrwx   0        0        0        0 2023-05-01 14:46:53.464048 cellpy-1.0.0a0/docs/developers_guide/
--rw-rw-rw-   0        0        0     1334 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/docs/developers_guide/dev_cellpy_data_structure.rst
--rw-rw-rw-   0        0        0     5904 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/docs/developers_guide/dev_cellpy_folder_structure.rst
--rw-rw-rw-   0        0        0      935 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/docs/developers_guide/dev_cellpy_packaging_pypi.rst
--rw-rw-rw-   0        0        0     3009 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/docs/developers_guide/dev_cellpy_setup.rst
--rw-rw-rw-   0        0        0     1821 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/docs/developers_guide/dev_conda_package.rst
--rw-rw-rw-   0        0        0     2136 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/docs/developers_guide/dev_docs.rst
--rw-rw-rw-   0        0        0     5218 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/docs/developers_guide/dev_loaders_and_instruments.rst
--rw-rw-rw-   0        0        0     1768 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/docs/developers_guide/dev_various.rst
--rw-rw-rw-   0        0        0      326 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/docs/developers_guide/index.rst
-drwxrwxrwx   0        0        0        0 2023-05-01 14:46:53.474047 cellpy-1.0.0a0/docs/examples_and_tutorials/
-drwxrwxrwx   0        0        0        0 2023-05-01 14:46:53.488048 cellpy-1.0.0a0/docs/examples_and_tutorials/basic_interactions/
--rw-rw-rw-   0        0        0    15786 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/docs/examples_and_tutorials/basic_interactions/01_getting_started_tutorial.rst
--rw-rw-rw-   0        0        0     3909 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/docs/examples_and_tutorials/basic_interactions/02_read_cell_data.rst
--rw-rw-rw-   0        0        0     5485 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/docs/examples_and_tutorials/basic_interactions/03_more_about_get.rst
--rw-rw-rw-   0        0        0     4465 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/docs/examples_and_tutorials/basic_interactions/04_other_interactions.rst
--rw-rw-rw-   0        0        0     5908 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/docs/examples_and_tutorials/basic_interactions/05_configuring.rst
--rw-rw-rw-   0        0        0     1052 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/docs/examples_and_tutorials/basic_interactions/06_pandas.rst
--rw-rw-rw-   0        0        0     1102 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/docs/examples_and_tutorials/basic_interactions/07_data_mining.rst
--rw-rw-rw-   0        0        0     8224 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/docs/examples_and_tutorials/basic_interactions/08_the_cellpy_cmd.rst
--rw-rw-rw-   0        0        0      484 2023-04-30 13:34:58.000000 cellpy-1.0.0a0/docs/examples_and_tutorials/basics.rst
--rw-rw-rw-   0        0        0      366 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/docs/examples_and_tutorials/examples.rst
--rw-rw-rw-   0        0        0      174 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/docs/examples_and_tutorials/index.rst
-drwxrwxrwx   0        0        0        0 2023-05-01 14:46:53.498046 cellpy-1.0.0a0/docs/examples_and_tutorials/loaders/
--rw-rw-rw-   0        0        0       49 2023-04-30 13:34:58.000000 cellpy-1.0.0a0/docs/examples_and_tutorials/loaders/01_arbin.rst
--rw-rw-rw-   0        0        0       52 2023-04-30 13:34:58.000000 cellpy-1.0.0a0/docs/examples_and_tutorials/loaders/02_maccor.rst
--rw-rw-rw-   0        0        0       43 2023-04-30 13:34:58.000000 cellpy-1.0.0a0/docs/examples_and_tutorials/loaders/03_PEC.rst
--rw-rw-rw-   0        0        0       54 2023-04-30 13:34:58.000000 cellpy-1.0.0a0/docs/examples_and_tutorials/loaders/04_Neware.rst
--rw-rw-rw-   0        0        0       62 2023-04-30 13:34:58.000000 cellpy-1.0.0a0/docs/examples_and_tutorials/loaders/05_biologics.rst
--rw-rw-rw-   0        0        0       54 2023-04-30 13:34:58.000000 cellpy-1.0.0a0/docs/examples_and_tutorials/loaders/06_custom.rst
--rw-rw-rw-   0        0        0      260 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/docs/examples_and_tutorials/loaders.rst
-drwxrwxrwx   0        0        0        0 2023-05-01 14:46:53.224850 cellpy-1.0.0a0/docs/examples_and_tutorials/notebooks/
-drwxrwxrwx   0        0        0        0 2023-05-01 14:46:53.502048 cellpy-1.0.0a0/docs/examples_and_tutorials/notebooks/images/
--rw-rw-rw-   0        0        0    88743 2023-04-30 13:34:58.000000 cellpy-1.0.0a0/docs/examples_and_tutorials/notebooks/images/templates_jupyterlab_001.png
--rw-rw-rw-   0        0        0    95663 2023-04-30 13:34:58.000000 cellpy-1.0.0a0/docs/examples_and_tutorials/notebooks/images/templates_jupyterlab_002.png
--rw-rw-rw-   0        0        0      231 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/docs/examples_and_tutorials/notebooks.rst
--rw-rw-rw-   0        0        0     1797 2023-04-30 13:34:58.000000 cellpy-1.0.0a0/docs/examples_and_tutorials/tips_and_tricks.rst
-drwxrwxrwx   0        0        0        0 2023-05-01 14:46:53.513049 cellpy-1.0.0a0/docs/examples_and_tutorials/utils/
--rw-rw-rw-   0        0        0     4388 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/docs/examples_and_tutorials/utils/batch.rst
--rw-rw-rw-   0        0        0       59 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/docs/examples_and_tutorials/utils/collectors.rst
--rw-rw-rw-   0        0        0       53 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/docs/examples_and_tutorials/utils/easyplot.rst
-drwxrwxrwx   0        0        0        0 2023-05-01 14:46:53.518048 cellpy-1.0.0a0/docs/examples_and_tutorials/utils/figures/
--rw-rw-rw-   0        0        0   296908 2023-04-30 13:34:58.000000 cellpy-1.0.0a0/docs/examples_and_tutorials/utils/figures/tutorials_utils_plotting_fig1.png
--rw-rw-rw-   0        0        0    54588 2023-04-30 13:34:58.000000 cellpy-1.0.0a0/docs/examples_and_tutorials/utils/figures/tutorials_utils_plotting_fig2.png
--rw-rw-rw-   0        0        0     1219 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/docs/examples_and_tutorials/utils/ica.rst
--rw-rw-rw-   0        0        0     2063 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/docs/examples_and_tutorials/utils/plotting.rst
--rw-rw-rw-   0        0        0      338 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/docs/examples_and_tutorials/utils/templates.rst
--rw-rw-rw-   0        0        0     1379 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/docs/examples_and_tutorials/utils/tut_ocv_rlx.rst
--rw-rw-rw-   0        0        0      371 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/docs/examples_and_tutorials/utils.rst
-drwxrwxrwx   0        0        0        0 2023-05-01 14:46:53.522046 cellpy-1.0.0a0/docs/figures/
--rw-rw-rw-   0        0        0     9981 2023-04-30 13:34:58.000000 cellpy-1.0.0a0/docs/figures/cellpy-icon-bw.png
--rw-rw-rw-   0        0        0    10302 2023-04-30 13:34:58.000000 cellpy-1.0.0a0/docs/figures/cellpy-logo-v1.png
--rw-rw-rw-   0        0        0      593 2023-04-30 13:34:58.000000 cellpy-1.0.0a0/docs/index.rst
-drwxrwxrwx   0        0        0        0 2023-05-01 14:46:53.534561 cellpy-1.0.0a0/docs/main_description/
--rw-rw-rw-   0        0        0       32 2023-04-30 13:34:58.000000 cellpy-1.0.0a0/docs/main_description/authors.rst
--rw-rw-rw-   0        0        0       37 2023-04-30 13:34:58.000000 cellpy-1.0.0a0/docs/main_description/contributing.rst
--rw-rw-rw-   0        0        0    16327 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/docs/main_description/formats.rst
--rw-rw-rw-   0        0        0       32 2023-04-30 13:34:58.000000 cellpy-1.0.0a0/docs/main_description/history.rst
--rw-rw-rw-   0        0        0      182 2023-04-30 13:34:58.000000 cellpy-1.0.0a0/docs/main_description/index.rst
--rw-rw-rw-   0        0        0     4288 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/docs/main_description/installation.rst
--rw-rw-rw-   0        0        0     3444 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/docs/main_description/usage.rst
--rwxrwxrwx   0        0        0     6701 2022-09-20 08:21:07.000000 cellpy-1.0.0a0/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-05-01 14:46:53.556582 cellpy-1.0.0a0/docs/source/
--rw-rw-rw-   0        0        0      367 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/docs/source/cellpy.internals.rst
--rw-rw-rw-   0        0        0      447 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/docs/source/cellpy.parameters.legacy.rst
--rw-rw-rw-   0        0        0      847 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/docs/source/cellpy.parameters.rst
--rw-rw-rw-   0        0        0     1911 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/docs/source/cellpy.readers.instruments.configurations.rst
--rw-rw-rw-   0        0        0      631 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/docs/source/cellpy.readers.instruments.loader_specific_modules.rst
--rw-rw-rw-   0        0        0      783 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/docs/source/cellpy.readers.instruments.processors.rst
--rw-rw-rw-   0        0        0     3413 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/docs/source/cellpy.readers.instruments.rst
--rw-rw-rw-   0        0        0     1139 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/docs/source/cellpy.readers.rst
--rw-rw-rw-   0        0        0      721 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/docs/source/cellpy.rst
--rw-rw-rw-   0        0        0     2610 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/docs/source/cellpy.utils.batch_tools.rst
--rw-rw-rw-   0        0        0     2222 2023-05-01 10:21:37.000000 cellpy-1.0.0a0/docs/source/cellpy.utils.rst
--rw-rw-rw-   0        0        0       62 2023-05-01 10:14:23.000000 cellpy-1.0.0a0/docs/source/modules.rst
--rw-rw-rw-   0        0        0      281 2023-04-30 13:34:58.000000 cellpy-1.0.0a0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-01 14:46:53.558574 cellpy-1.0.0a0/setup.cfg
--rw-rw-rw-   0        0        0     2952 2023-04-30 13:34:58.000000 cellpy-1.0.0a0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 13:01:03.083461 cellpy-1.0.0a3/
+-rw-rw-rw-   0        0        0      503 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3086 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     3908 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/HISTORY.rst
+-rw-rw-rw-   0        0        0     1089 2021-12-21 09:11:58.000000 cellpy-1.0.0a3/LICENSE
+-rw-rw-rw-   0        0        0      645 2022-05-27 12:07:50.000000 cellpy-1.0.0a3/MANIFEST.in
+-rw-rw-rw-   0        0        0     6518 2023-05-04 13:01:03.082460 cellpy-1.0.0a3/PKG-INFO
+-rw-rw-rw-   0        0        0     1872 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-04 13:01:02.227799 cellpy-1.0.0a3/cellpy/
+-rw-rw-rw-   0        0        0      805 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/__init__.py
+-rw-rw-rw-   0        0        0       25 2023-05-04 13:00:22.000000 cellpy-1.0.0a3/cellpy/_version.py
+-rw-rw-rw-   0        0        0    51949 2023-05-02 11:55:35.000000 cellpy-1.0.0a3/cellpy/cli.py
+-rw-rw-rw-   0        0        0     1228 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-04 13:01:02.256840 cellpy-1.0.0a3/cellpy/internals/
+-rw-rw-rw-   0        0        0        0 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/internals/__init__.py
+-rw-rw-rw-   0        0        0    26690 2023-05-04 11:47:01.000000 cellpy-1.0.0a3/cellpy/internals/core.py
+-rw-rw-rw-   0        0        0     4838 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/log.py
+-rw-rw-rw-   0        0        0     1750 2021-12-21 09:11:58.000000 cellpy-1.0.0a3/cellpy/logging.json
+drwxrwxrwx   0        0        0        0 2023-05-04 13:01:02.277877 cellpy-1.0.0a3/cellpy/parameters/
+-rw-rw-rw-   0        0        0     3183 2023-05-02 11:51:31.000000 cellpy-1.0.0a3/cellpy/parameters/.cellpy_prms_default.conf
+-rw-rw-rw-   0        0        0        2 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/parameters/__init__.py
+-rw-rw-rw-   0        0        0    23361 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/parameters/internal_settings.py
+drwxrwxrwx   0        0        0        0 2023-05-04 13:01:02.283879 cellpy-1.0.0a3/cellpy/parameters/legacy/
+-rw-rw-rw-   0        0        0        0 2021-12-21 09:11:58.000000 cellpy-1.0.0a3/cellpy/parameters/legacy/__init__.py
+-rw-rw-rw-   0        0        0    24146 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/parameters/legacy/update_headers.py
+-rw-rw-rw-   0        0        0    12142 2023-05-02 11:42:19.000000 cellpy-1.0.0a3/cellpy/parameters/prmreader.py
+-rw-rw-rw-   0        0        0    12220 2023-05-02 11:49:22.000000 cellpy-1.0.0a3/cellpy/parameters/prms.py
+drwxrwxrwx   0        0        0        0 2023-05-04 13:01:02.309923 cellpy-1.0.0a3/cellpy/readers/
+-rw-rw-rw-   0        0        0        2 2021-12-21 09:11:58.000000 cellpy-1.0.0a3/cellpy/readers/__init__.py
+-rw-rw-rw-   0        0        0   227868 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/readers/cellreader.py
+-rw-rw-rw-   0        0        0    39447 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/readers/core.py
+-rw-rw-rw-   0        0        0    22998 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/readers/dbreader.py
+-rw-rw-rw-   0        0        0    13468 2023-05-04 11:58:58.000000 cellpy-1.0.0a3/cellpy/readers/filefinder.py
+drwxrwxrwx   0        0        0        0 2023-05-04 13:01:02.387862 cellpy-1.0.0a3/cellpy/readers/instruments/
+-rw-rw-rw-   0        0        0        0 2021-12-21 09:11:58.000000 cellpy-1.0.0a3/cellpy/readers/instruments/__init__.py
+-rw-rw-rw-   0        0        0    50849 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/readers/instruments/arbin_res.py
+-rw-rw-rw-   0        0        0    19381 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/readers/instruments/arbin_sql.py
+-rw-rw-rw-   0        0        0    21062 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/readers/instruments/arbin_sql_7.py
+-rw-rw-rw-   0        0        0    11134 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/readers/instruments/arbin_sql_csv.py
+-rw-rw-rw-   0        0        0     7126 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/readers/instruments/arbin_sql_h5.py
+-rw-rw-rw-   0        0        0     9883 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/readers/instruments/arbin_sql_xlsx.py
+-rw-rw-rw-   0        0        0    27501 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/readers/instruments/base.py
+-rw-rw-rw-   0        0        0    22693 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/readers/instruments/biologics_mpr.py
+drwxrwxrwx   0        0        0        0 2023-05-04 13:01:02.417245 cellpy-1.0.0a3/cellpy/readers/instruments/configurations/
+-rw-rw-rw-   0        0        0     6607 2022-06-03 19:58:41.000000 cellpy-1.0.0a3/cellpy/readers/instruments/configurations/__init__.py
+-rw-rw-rw-   0        0        0     1700 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/readers/instruments/configurations/maccor_txt_four.py
+-rw-rw-rw-   0        0        0     4084 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/readers/instruments/configurations/maccor_txt_one.py
+-rw-rw-rw-   0        0        0     1990 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/readers/instruments/configurations/maccor_txt_three.py
+-rw-rw-rw-   0        0        0     1788 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/readers/instruments/configurations/maccor_txt_two.py
+-rw-rw-rw-   0        0        0     3549 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/readers/instruments/configurations/maccor_txt_zero.py
+-rw-rw-rw-   0        0        0     2132 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/readers/instruments/configurations/neware_txt_zero.py
+-rw-rw-rw-   0        0        0    10327 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/readers/instruments/custom.py
+-rw-rw-rw-   0        0        0     3760 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/readers/instruments/ext_nda_reader.py
+drwxrwxrwx   0        0        0        0 2023-05-04 13:01:02.425247 cellpy-1.0.0a3/cellpy/readers/instruments/loader_specific_modules/
+-rw-rw-rw-   0        0        0        0 2022-06-03 19:58:41.000000 cellpy-1.0.0a3/cellpy/readers/instruments/loader_specific_modules/__init__.py
+-rw-rw-rw-   0        0        0    22115 2022-06-03 19:58:41.000000 cellpy-1.0.0a3/cellpy/readers/instruments/loader_specific_modules/biologic_file_format.py
+-rw-rw-rw-   0        0        0     1067 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/readers/instruments/local_instrument.py
+-rw-rw-rw-   0        0        0    12886 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/readers/instruments/maccor_txt.py
+-rw-rw-rw-   0        0        0     3488 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/readers/instruments/neware_txt.py
+-rw-rw-rw-   0        0        0    16769 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/readers/instruments/pec_csv.py
+drwxrwxrwx   0        0        0        0 2023-05-04 13:01:02.439260 cellpy-1.0.0a3/cellpy/readers/instruments/processors/
+-rw-rw-rw-   0        0        0        0 2022-05-27 12:07:50.000000 cellpy-1.0.0a3/cellpy/readers/instruments/processors/__init__.py
+-rw-rw-rw-   0        0        0    15265 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/readers/instruments/processors/post_processors.py
+-rw-rw-rw-   0        0        0     1450 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/readers/instruments/processors/pre_processors.py
+-rw-rw-rw-   0        0        0    26852 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/readers/sql_dbreader.py
+drwxrwxrwx   0        0        0        0 2023-05-04 13:01:02.502372 cellpy-1.0.0a3/cellpy/utils/
+-rw-rw-rw-   0        0        0      192 2021-12-21 09:11:58.000000 cellpy-1.0.0a3/cellpy/utils/__init__.py
+-rw-rw-rw-   0        0        0    48182 2023-05-03 09:31:40.000000 cellpy-1.0.0a3/cellpy/utils/batch.py
+drwxrwxrwx   0        0        0        0 2023-05-04 13:01:02.551372 cellpy-1.0.0a3/cellpy/utils/batch_tools/
+-rw-rw-rw-   0        0        0        0 2021-12-21 09:11:58.000000 cellpy-1.0.0a3/cellpy/utils/batch_tools/__init__.py
+-rw-rw-rw-   0        0        0     7578 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/utils/batch_tools/batch_analyzers.py
+-rw-rw-rw-   0        0        0    19566 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/utils/batch_tools/batch_core.py
+-rw-rw-rw-   0        0        0    40001 2023-05-03 09:29:45.000000 cellpy-1.0.0a3/cellpy/utils/batch_tools/batch_experiments.py
+-rw-rw-rw-   0        0        0     2931 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/utils/batch_tools/batch_exporters.py
+-rw-rw-rw-   0        0        0    13636 2023-05-02 11:59:40.000000 cellpy-1.0.0a3/cellpy/utils/batch_tools/batch_helpers.py
+-rw-rw-rw-   0        0        0    27683 2023-05-02 13:39:36.000000 cellpy-1.0.0a3/cellpy/utils/batch_tools/batch_journals.py
+-rw-rw-rw-   0        0        0    29066 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/utils/batch_tools/batch_plotters.py
+-rw-rw-rw-   0        0        0      245 2021-12-21 09:11:58.000000 cellpy-1.0.0a3/cellpy/utils/batch_tools/batch_reporters.py
+-rw-rw-rw-   0        0        0     3339 2022-05-27 12:03:59.000000 cellpy-1.0.0a3/cellpy/utils/batch_tools/dumpers.py
+-rw-rw-rw-   0        0        0     9872 2023-05-02 10:20:24.000000 cellpy-1.0.0a3/cellpy/utils/batch_tools/engines.py
+-rw-rw-rw-   0        0        0     5294 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/utils/batch_tools/sqlite_from_excel_db.py
+-rw-rw-rw-   0        0        0    63308 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/utils/collectors.py
+-rw-rw-rw-   0        0        0    45461 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/utils/collectors_old.py
+drwxrwxrwx   0        0        0        0 2023-05-04 13:01:02.558373 cellpy-1.0.0a3/cellpy/utils/data/
+-rw-rw-rw-   0        0        0  3700143 2023-05-03 22:26:41.000000 cellpy-1.0.0a3/cellpy/utils/data/20160805_test001_45_cc.h5
+drwxrwxrwx   0        0        0        0 2023-05-04 13:01:02.579371 cellpy-1.0.0a3/cellpy/utils/data/raw/
+-rw-rw-rw-   0        0        0  1613824 2021-12-21 09:11:58.000000 cellpy-1.0.0a3/cellpy/utils/data/raw/20160805_test001_45_cc_01.res
+-rw-rw-rw-   0        0        0      260 2022-05-27 12:07:50.000000 cellpy-1.0.0a3/cellpy/utils/diagnostics.py
+-rw-rw-rw-   0        0        0    79016 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/utils/easyplot.py
+-rw-rw-rw-   0        0        0     1576 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/utils/example_data.py
+-rw-rw-rw-   0        0        0    39446 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/utils/helpers.py
+-rw-rw-rw-   0        0        0    38967 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/utils/ica.py
+-rw-rw-rw-   0        0        0      189 2022-05-27 12:07:50.000000 cellpy-1.0.0a3/cellpy/utils/live.py
+-rw-rw-rw-   0        0        0    24037 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/utils/ocv_rlx.py
+-rw-rw-rw-   0        0        0    45397 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/utils/plotutils.py
+-rw-rw-rw-   0        0        0     1787 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/utils/processor.py
+drwxrwxrwx   0        0        0        0 2023-05-04 13:01:02.248839 cellpy-1.0.0a3/cellpy.egg-info/
+-rw-rw-rw-   0        0        0     6518 2023-05-04 13:01:01.000000 cellpy-1.0.0a3/cellpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7846 2023-05-04 13:01:02.000000 cellpy-1.0.0a3/cellpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 13:01:01.000000 cellpy-1.0.0a3/cellpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 13:01:01.000000 cellpy-1.0.0a3/cellpy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-04 13:00:59.000000 cellpy-1.0.0a3/cellpy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      337 2023-05-04 13:01:01.000000 cellpy-1.0.0a3/cellpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-04 13:01:01.000000 cellpy-1.0.0a3/cellpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-04 13:01:02.606375 cellpy-1.0.0a3/docs/
+-rw-rw-rw-   0        0        0     6939 2022-09-20 08:21:07.000000 cellpy-1.0.0a3/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-05-04 13:01:02.177629 cellpy-1.0.0a3/docs/_build/
+drwxrwxrwx   0        0        0        0 2023-05-04 13:01:02.176629 cellpy-1.0.0a3/docs/_build/.doctrees/
+drwxrwxrwx   0        0        0        0 2023-05-04 13:01:02.622371 cellpy-1.0.0a3/docs/_build/.doctrees/nbsphinx/
+-rw-rw-rw-   0        0        0    15014 2023-04-30 13:53:57.000000 cellpy-1.0.0a3/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_6_0.png
+-rw-rw-rw-   0        0        0    14599 2023-04-30 13:53:57.000000 cellpy-1.0.0a3/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_7_0.png
+-rw-rw-rw-   0        0        0    13527 2023-04-30 13:53:57.000000 cellpy-1.0.0a3/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_8_0.png
+-rw-rw-rw-   0        0        0    25669 2023-04-30 13:54:02.000000 cellpy-1.0.0a3/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_simple_plot_2_0.png
+drwxrwxrwx   0        0        0        0 2023-05-04 13:01:02.696856 cellpy-1.0.0a3/docs/_build/_images/
+-rw-rw-rw-   0        0        0    15014 2023-04-27 15:02:55.000000 cellpy-1.0.0a3/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_6_0.png
+-rw-rw-rw-   0        0        0    14599 2023-04-27 15:02:55.000000 cellpy-1.0.0a3/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_7_0.png
+-rw-rw-rw-   0        0        0    13527 2023-04-27 15:02:55.000000 cellpy-1.0.0a3/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_8_0.png
+-rw-rw-rw-   0        0        0    25669 2023-04-27 15:03:02.000000 cellpy-1.0.0a3/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_simple_plot_2_0.png
+-rw-rw-rw-   0        0        0    11678 2023-04-29 14:19:31.000000 cellpy-1.0.0a3/docs/_build/_images/graphviz-22185705e237fa530df24e4af50cb25833165e25.png
+-rw-rw-rw-   0        0        0    22040 2023-04-29 14:33:27.000000 cellpy-1.0.0a3/docs/_build/_images/graphviz-246f2486cd940f2ea40a07f847c86c22b2607ca8.png
+-rw-rw-rw-   0        0        0    21790 2023-04-29 14:26:00.000000 cellpy-1.0.0a3/docs/_build/_images/graphviz-42e9bc826d476a3d361a7f410e989ed34dc1aa85.png
+-rw-rw-rw-   0        0        0    32991 2023-04-29 14:26:01.000000 cellpy-1.0.0a3/docs/_build/_images/graphviz-619216a42370fd49669c083549129b8470c8fae1.png
+-rw-rw-rw-   0        0        0    32991 2023-04-30 20:02:23.000000 cellpy-1.0.0a3/docs/_build/_images/graphviz-6412a7c74952b4793798e9032f5bc4e7a1ab70c1.png
+-rw-rw-rw-   0        0        0     7231 2023-04-29 14:12:31.000000 cellpy-1.0.0a3/docs/_build/_images/graphviz-6deb64a460668e8ef9bf0ca653314119adeeae66.png
+-rw-rw-rw-   0        0        0    13360 2023-04-29 14:36:26.000000 cellpy-1.0.0a3/docs/_build/_images/graphviz-83b62e03ef369ff0a30f027892dba95b91ea8b6c.png
+-rw-rw-rw-   0        0        0    21790 2023-04-30 20:02:22.000000 cellpy-1.0.0a3/docs/_build/_images/graphviz-8ec82d564b1a6ea5b95a36a4a213f7a78aaedc63.png
+-rw-rw-rw-   0        0        0     5391 2023-04-29 14:10:02.000000 cellpy-1.0.0a3/docs/_build/_images/graphviz-ce8a9fe2ba01194aed847e0248d749db4093aca1.png
+-rw-rw-rw-   0        0        0    20826 2023-04-29 14:29:06.000000 cellpy-1.0.0a3/docs/_build/_images/graphviz-e94a5352318e02fcc5ef1f813e02a526c39af791.png
+-rw-rw-rw-   0        0        0    88743 2023-04-19 13:49:30.000000 cellpy-1.0.0a3/docs/_build/_images/templates_jupyterlab_001.png
+-rw-rw-rw-   0        0        0   296908 2022-05-27 12:07:51.000000 cellpy-1.0.0a3/docs/_build/_images/tutorials_utils_plotting_fig1.png
+-rw-rw-rw-   0        0        0    54588 2022-05-27 12:07:51.000000 cellpy-1.0.0a3/docs/_build/_images/tutorials_utils_plotting_fig2.png
+drwxrwxrwx   0        0        0        0 2023-05-04 13:01:02.708851 cellpy-1.0.0a3/docs/_build/_static/
+-rw-rw-rw-   0        0        0      286 2023-04-25 11:20:36.000000 cellpy-1.0.0a3/docs/_build/_static/file.png
+-rw-rw-rw-   0        0        0       90 2023-04-25 11:20:36.000000 cellpy-1.0.0a3/docs/_build/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2023-04-25 11:20:36.000000 cellpy-1.0.0a3/docs/_build/_static/plus.png
+-rw-rw-rw-   0        0        0     1695 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/adapted_readme.rst
+-rw-rw-rw-   0        0        0    10731 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/conf.py
+drwxrwxrwx   0        0        0        0 2023-05-04 13:01:02.741848 cellpy-1.0.0a3/docs/developers_guide/
+-rw-rw-rw-   0        0        0     1334 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/developers_guide/dev_cellpy_data_structure.rst
+-rw-rw-rw-   0        0        0     5904 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/developers_guide/dev_cellpy_folder_structure.rst
+-rw-rw-rw-   0        0        0      935 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/developers_guide/dev_cellpy_packaging_pypi.rst
+-rw-rw-rw-   0        0        0     3009 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/developers_guide/dev_cellpy_setup.rst
+-rw-rw-rw-   0        0        0     1821 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/developers_guide/dev_conda_package.rst
+-rw-rw-rw-   0        0        0     2136 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/developers_guide/dev_docs.rst
+-rw-rw-rw-   0        0        0     5218 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/developers_guide/dev_loaders_and_instruments.rst
+-rw-rw-rw-   0        0        0     1768 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/developers_guide/dev_various.rst
+-rw-rw-rw-   0        0        0      326 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/developers_guide/index.rst
+drwxrwxrwx   0        0        0        0 2023-05-04 13:01:02.766850 cellpy-1.0.0a3/docs/examples_and_tutorials/
+drwxrwxrwx   0        0        0        0 2023-05-04 13:01:02.797848 cellpy-1.0.0a3/docs/examples_and_tutorials/basic_interactions/
+-rw-rw-rw-   0        0        0    15786 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/basic_interactions/01_getting_started_tutorial.rst
+-rw-rw-rw-   0        0        0     3909 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/basic_interactions/02_read_cell_data.rst
+-rw-rw-rw-   0        0        0     5485 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/basic_interactions/03_more_about_get.rst
+-rw-rw-rw-   0        0        0     4465 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/basic_interactions/04_other_interactions.rst
+-rw-rw-rw-   0        0        0     5908 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/basic_interactions/05_configuring.rst
+-rw-rw-rw-   0        0        0     1052 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/basic_interactions/06_pandas.rst
+-rw-rw-rw-   0        0        0     1102 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/basic_interactions/07_data_mining.rst
+-rw-rw-rw-   0        0        0     8224 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/basic_interactions/08_the_cellpy_cmd.rst
+-rw-rw-rw-   0        0        0      484 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/basics.rst
+-rw-rw-rw-   0        0        0      366 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/examples.rst
+-rw-rw-rw-   0        0        0      174 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/index.rst
+drwxrwxrwx   0        0        0        0 2023-05-04 13:01:02.816847 cellpy-1.0.0a3/docs/examples_and_tutorials/loaders/
+-rw-rw-rw-   0        0        0       49 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/loaders/01_arbin.rst
+-rw-rw-rw-   0        0        0       52 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/loaders/02_maccor.rst
+-rw-rw-rw-   0        0        0       43 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/loaders/03_PEC.rst
+-rw-rw-rw-   0        0        0       54 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/loaders/04_Neware.rst
+-rw-rw-rw-   0        0        0       62 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/loaders/05_biologics.rst
+-rw-rw-rw-   0        0        0       54 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/loaders/06_custom.rst
+-rw-rw-rw-   0        0        0      260 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/loaders.rst
+drwxrwxrwx   0        0        0        0 2023-05-04 13:01:02.181153 cellpy-1.0.0a3/docs/examples_and_tutorials/notebooks/
+drwxrwxrwx   0        0        0        0 2023-05-04 13:01:02.974146 cellpy-1.0.0a3/docs/examples_and_tutorials/notebooks/images/
+-rw-rw-rw-   0        0        0    88743 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/notebooks/images/templates_jupyterlab_001.png
+-rw-rw-rw-   0        0        0    95663 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/notebooks/images/templates_jupyterlab_002.png
+-rw-rw-rw-   0        0        0      231 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/notebooks.rst
+-rw-rw-rw-   0        0        0     1797 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/tips_and_tricks.rst
+drwxrwxrwx   0        0        0        0 2023-05-04 13:01:02.998377 cellpy-1.0.0a3/docs/examples_and_tutorials/utils/
+-rw-rw-rw-   0        0        0     4388 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/utils/batch.rst
+-rw-rw-rw-   0        0        0       59 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/utils/collectors.rst
+-rw-rw-rw-   0        0        0       53 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/utils/easyplot.rst
+drwxrwxrwx   0        0        0        0 2023-05-04 13:01:03.005398 cellpy-1.0.0a3/docs/examples_and_tutorials/utils/figures/
+-rw-rw-rw-   0        0        0   296908 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/utils/figures/tutorials_utils_plotting_fig1.png
+-rw-rw-rw-   0        0        0    54588 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/utils/figures/tutorials_utils_plotting_fig2.png
+-rw-rw-rw-   0        0        0     1219 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/utils/ica.rst
+-rw-rw-rw-   0        0        0     2063 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/utils/plotting.rst
+-rw-rw-rw-   0        0        0      338 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/utils/templates.rst
+-rw-rw-rw-   0        0        0     1379 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/utils/tut_ocv_rlx.rst
+-rw-rw-rw-   0        0        0      371 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/utils.rst
+drwxrwxrwx   0        0        0        0 2023-05-04 13:01:03.012399 cellpy-1.0.0a3/docs/figures/
+-rw-rw-rw-   0        0        0     9981 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/figures/cellpy-icon-bw.png
+-rw-rw-rw-   0        0        0    10302 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/figures/cellpy-logo-v1.png
+-rw-rw-rw-   0        0        0      593 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/index.rst
+drwxrwxrwx   0        0        0        0 2023-05-04 13:01:03.035463 cellpy-1.0.0a3/docs/main_description/
+-rw-rw-rw-   0        0        0       32 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/main_description/authors.rst
+-rw-rw-rw-   0        0        0       37 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/main_description/contributing.rst
+-rw-rw-rw-   0        0        0    16327 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/main_description/formats.rst
+-rw-rw-rw-   0        0        0       32 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/main_description/history.rst
+-rw-rw-rw-   0        0        0      182 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/main_description/index.rst
+-rw-rw-rw-   0        0        0     4288 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/main_description/installation.rst
+-rw-rw-rw-   0        0        0     3444 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/main_description/usage.rst
+-rwxrwxrwx   0        0        0     6701 2022-09-20 08:21:07.000000 cellpy-1.0.0a3/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-05-04 13:01:03.079462 cellpy-1.0.0a3/docs/source/
+-rw-rw-rw-   0        0        0      367 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/source/cellpy.internals.rst
+-rw-rw-rw-   0        0        0      447 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/source/cellpy.parameters.legacy.rst
+-rw-rw-rw-   0        0        0      847 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/source/cellpy.parameters.rst
+-rw-rw-rw-   0        0        0     1911 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/source/cellpy.readers.instruments.configurations.rst
+-rw-rw-rw-   0        0        0      631 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/source/cellpy.readers.instruments.loader_specific_modules.rst
+-rw-rw-rw-   0        0        0      783 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/source/cellpy.readers.instruments.processors.rst
+-rw-rw-rw-   0        0        0     3413 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/source/cellpy.readers.instruments.rst
+-rw-rw-rw-   0        0        0     1139 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/source/cellpy.readers.rst
+-rw-rw-rw-   0        0        0      721 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/source/cellpy.rst
+-rw-rw-rw-   0        0        0     2610 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/source/cellpy.utils.batch_tools.rst
+-rw-rw-rw-   0        0        0     2222 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/source/cellpy.utils.rst
+-rw-rw-rw-   0        0        0       62 2023-05-01 10:14:23.000000 cellpy-1.0.0a3/docs/source/modules.rst
+-rw-rw-rw-   0        0        0      281 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-04 13:01:03.084462 cellpy-1.0.0a3/setup.cfg
+-rw-rw-rw-   0        0        0     2952 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/setup.py
```

### Comparing `cellpy-1.0.0a0/CONTRIBUTING.rst` & `cellpy-1.0.0a3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/HISTORY.rst` & `cellpy-1.0.0a3/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/LICENSE` & `cellpy-1.0.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/MANIFEST.in` & `cellpy-1.0.0a3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/PKG-INFO` & `cellpy-1.0.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellpy
-Version: 1.0.0a0
+Version: 1.0.0a3
 Summary: Extract and manipulate data from battery data testers.
 Home-page: https://github.com/jepegit/cellpy
 Author: Jan Petter Maehlen
 Author-email: jepe@ife.no
 License: MIT license
 Keywords: cellpy
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cellpy-1.0.0a0/README.rst` & `cellpy-1.0.0a3/README.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/cellpy/__init__.py` & `cellpy-1.0.0a3/cellpy/__init__.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/cellpy/cli.py` & `cellpy-1.0.0a3/cellpy/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,1688 +1,1688 @@
-import base64
-import getpass
-import logging
-import os
-import pathlib
-from pprint import pprint
-import re
-import subprocess
-import sys
-from typing import Union
-import urllib
-from pathlib import Path
-
-import click
-import pkg_resources
-from github import Github
-
-import cellpy._version
-from cellpy.exceptions import ConfigFileNotWritten
-from cellpy.parameters import prmreader
-from cellpy.parameters.internal_settings import OTHERPATHS
-from cellpy.internals.core import OtherPath
-
-VERSION = cellpy._version.__version__
-REPO = "jepegit/cellpy"
-USER = "jepegit"
-GITHUB_PWD_VAR_NAME = "GD_PWD"
-
-
-def save_prm_file(prm_filename):
-    """saves (writes) the prms to file"""
-    prmreader._write_prm_file(prm_filename)
-
-
-def get_package_prm_dir():
-    """gets the folder where the cellpy package lives"""
-    prm_dir = pkg_resources.resource_filename("cellpy", "parameters")
-    return pathlib.Path(prm_dir)
-
-
-def get_default_config_file_path(init_filename=None):
-    """gets the path to the default config-file"""
-    prm_dir = get_package_prm_dir()
-    if not init_filename:
-        init_filename = prmreader.DEFAULT_FILENAME
-    src = prm_dir / init_filename
-    return src
-
-
-def get_dst_file(user_dir, init_filename):
-    user_dir = pathlib.Path(user_dir)
-    dst_file = user_dir / init_filename
-    return dst_file
-
-
-def check_if_needed_modules_exists():
-    pass
-
-
-def modify_config_file():
-    pass
-
-
-def create_cellpy_folders():
-    pass
-
-
-@click.group("cellpy")
-def cli():
-    pass
-
-
-# ----------------------- setup --------------------------------------
-@click.command()
-@click.option(
-    "--interactive",
-    "-i",
-    is_flag=True,
-    default=False,
-    help="Allows you to specify div. folders and setting.",
-)
-@click.option(
-    "--not-relative",
-    "-nr",
-    is_flag=True,
-    default=False,
-    help="If root-dir is given, put it directly in the root (/) folder"
-    " i.e. don't put it in your home directory. Defaults to False. Remark"
-    " that if you specifically write a path name instead of selecting the"
-    " suggested default, the path you write will be used as is.",
-)
-@click.option(
-    "--dry-run",
-    "-dr",
-    is_flag=True,
-    default=False,
-    help="Run setup in dry mode (only print - do not execute). This is"
-    " typically used when developing and testing cellpy. Defaults to"
-    " False.",
-)
-@click.option(
-    "--reset",
-    "-r",
-    is_flag=True,
-    default=False,
-    help="Do not suggest path defaults based on your current configuration-file",
-)
-@click.option(
-    "--root-dir",
-    "-d",
-    default=None,
-    type=click.Path(),
-    help="Use custom root dir. If not given, your home directory"
-    " will be used as the top level where cellpy-folders"
-    " will be put. The folder path must follow"
-    " directly after this option (if used). Example:\n"
-    " $ cellpy setup -d 'MyDir'",
-)
-@click.option(
-    "--folder-name",
-    "-n",
-    default=None,
-    type=click.Path(),
-    help="",
-)
-@click.option(
-    "--test_user", "-t", default=None, help="Fake name for fake user (for testing)"
-)
-def setup(interactive, not_relative, dry_run, reset, root_dir, folder_name, test_user):
-    """This will help you to set up cellpy."""
-
-    click.echo("[cellpy] (setup)")
-    click.echo(f"[cellpy] root-dir: {root_dir}")
-
-    # generate variables
-    init_filename = prmreader.create_custom_init_filename()
-    user_dir, dst_file = prmreader.get_user_dir_and_dst(init_filename)
-
-    if dry_run:
-        click.echo("Create custom init filename and get user_dir and destination")
-        click.echo(f"Got the following parameters:")
-        click.echo(f" - init_filename: {init_filename}")
-        click.echo(f" - user_dir: {user_dir}")
-        click.echo(f" - dst_file: {dst_file}")
-        click.echo(f" - not_relative: {not_relative}")
-
-    if root_dir and not interactive:
-        click.echo("[cellpy] custom root-dir can only be used in interactive mode")
-        click.echo("[cellpy] -> setting interactive mode")
-        interactive = True
-
-    if not root_dir:
-        root_dir = user_dir
-        # root_dir = pathlib.Path(os.getcwd())
-    root_dir = pathlib.Path(root_dir)
-
-    if dry_run:
-        click.echo(f" - root_dir: {root_dir}")
-
-    if test_user:
-        click.echo(f"[cellpy] (setup) DEV-MODE test_user: {test_user}")
-        init_filename = prmreader.create_custom_init_filename(test_user)
-        user_dir = root_dir
-        dst_file = get_dst_file(user_dir, init_filename)
-        click.echo(f"[cellpy] (setup) DEV-MODE user_dir: {user_dir}")
-        click.echo(f"[cellpy] (setup) DEV-MODE dst_file: {dst_file}")
-
-    if not pathlib.Path(dst_file).is_file():
-        click.echo(f"[cellpy] {dst_file} not found -> I will make one for you!")
-        reset = True
-
-    if interactive:
-        click.echo(" interactive mode ".center(80, "-"))
-        _update_paths(
-            custom_dir=root_dir,
-            relative_home=not not_relative,
-            default_dir=folder_name,
-            dry_run=dry_run,
-            reset=reset,
-        )
-        _write_config_file(user_dir, dst_file, init_filename, dry_run)
-        _check(dry_run=dry_run)
-
-    else:
-        if reset:
-            _update_paths(
-                user_dir,
-                False,
-                default_dir=folder_name,
-                dry_run=dry_run,
-                reset=True,
-                silent=True,
-            )
-        _write_config_file(user_dir, dst_file, init_filename, dry_run)
-        _check(dry_run=dry_run)
-
-
-def _update_paths(
-    custom_dir=None,
-    relative_home=True,
-    reset=False,
-    dry_run=False,
-    default_dir=None,
-    silent=False,
-):
-    # please, refactor me :-(
-
-    h = prmreader.get_user_dir()
-
-    if default_dir is None:
-        default_dir = "cellpy_data"
-
-    if dry_run:
-        click.echo(f" - default_dir: {default_dir}")
-        click.echo(f" - custom_dir: {custom_dir}")
-        click.echo(f" - retalive_home: {relative_home}")
-
-    if custom_dir:
-        reset = True
-        if relative_home:
-            h = h / custom_dir
-        if not custom_dir.parts[-1] == default_dir:
-            h = h / default_dir
-
-    if not reset:
-        outdatadir = pathlib.Path(prmreader.prms.Paths.outdatadir)
-        rawdatadir = OtherPath(prmreader.prms.Paths.rawdatadir)
-        cellpydatadir = OtherPath(prmreader.prms.Paths.cellpydatadir)
-        filelogdir = pathlib.Path(prmreader.prms.Paths.filelogdir)
-        examplesdir = pathlib.Path(prmreader.prms.Paths.examplesdir)
-        db_path = pathlib.Path(prmreader.prms.Paths.db_path)
-        db_filename = prmreader.prms.Paths.db_filename
-        notebookdir = pathlib.Path(prmreader.prms.Paths.notebookdir)
-        batchfiledir = pathlib.Path(prmreader.prms.Paths.batchfiledir)
-        templatedir = pathlib.Path(prmreader.prms.Paths.templatedir)
-        instrumentdir = pathlib.Path(prmreader.prms.Paths.instrumentsdir)
-    else:
-        outdatadir = "out"
-        rawdatadir = "raw"
-        cellpydatadir = "cellpyfiles"
-        filelogdir = "logs"
-        examplesdir = "examples"
-        db_path = "db"
-        db_filename = "cellpy_db.xlsx"
-        notebookdir = "notebooks"
-        batchfiledir = "batchfiles"
-        templatedir = "templates"
-        instrumentdir = "instruments"
-
-    outdatadir = h / outdatadir
-    rawdatadir = h / rawdatadir
-    cellpydatadir = h / cellpydatadir
-    filelogdir = h / filelogdir
-    examplesdir = h / examplesdir
-    db_path = h / db_path
-    notebookdir = h / notebookdir
-    batchfiledir = h / batchfiledir
-    templatedir = h / templatedir
-    instrumentdir = h / instrumentdir
-
-    if dry_run:
-        click.echo(f" - base (h): {h}")
-
-    if not silent:
-        outdatadir = _ask_about_path(
-            "where to output processed data and results", outdatadir
-        )
-        rawdatadir = _ask_about_otherpath("where your raw data are located", rawdatadir)
-        cellpydatadir = _ask_about_otherpath("where to put cellpy-files", cellpydatadir)
-        filelogdir = _ask_about_path("where to dump the log-files", filelogdir)
-        examplesdir = _ask_about_path(
-            "where to download cellpy examples and tests", examplesdir
-        )
-        db_path = _ask_about_path("what folder your db file lives in", db_path)
-        db_filename = _ask_about_name("the name of your db-file", db_filename)
-        notebookdir = _ask_about_path(
-            "where to put your jupyter notebooks", notebookdir
-        )
-        batchfiledir = _ask_about_path("where to put your batch files", batchfiledir)
-        templatedir = _ask_about_path("where to put your batch files", templatedir)
-        instrumentdir = _ask_about_path("where to put your batch files", instrumentdir)
-
-    # update folders based on suggestions
-    for d in [
-        outdatadir,
-        rawdatadir,
-        cellpydatadir,
-        filelogdir,
-        examplesdir,
-        notebookdir,
-        db_path,
-        batchfiledir,
-        templatedir,
-        instrumentdir,
-    ]:
-        if not dry_run:
-            _create_dir(d)
-        else:
-            click.echo(f"dry run (so I did not create {d})")
-
-    # update config-file based on suggestions
-    prmreader.prms.Paths.outdatadir = str(outdatadir)
-    prmreader.prms.Paths.rawdatadir = str(rawdatadir)
-    prmreader.prms.Paths.cellpydatadir = str(cellpydatadir)
-    prmreader.prms.Paths.filelogdir = str(filelogdir)
-    prmreader.prms.Paths.examplesdir = str(examplesdir)
-    prmreader.prms.Paths.db_path = str(db_path)
-    prmreader.prms.Paths.db_filename = str(db_filename)
-    prmreader.prms.Paths.notebookdir = str(notebookdir)
-    prmreader.prms.Paths.batchfiledir = str(batchfiledir)
-    prmreader.prms.Paths.templatedir = str(templatedir)
-    prmreader.prms.Paths.instrumentdir = str(instrumentdir)
-
-
-def _ask_about_path(q, p):
-    click.echo(f"\n[cellpy] (setup) input {q}")
-    click.echo(f"[cellpy] (setup) current: {p}")
-    new_path = input("[cellpy] (setup) [KEEP/new value] >>> ").strip()
-    if not new_path:
-        new_path = p
-    return pathlib.Path(new_path)
-
-
-def _ask_about_otherpath(q, p):
-    click.echo(f"\n[cellpy] (setup) input {q}")
-    click.echo(f"[cellpy] (setup) current: {p}")
-    new_path = input("[cellpy] (setup) [KEEP/new value] >>> ").strip()
-    if not new_path:
-        new_path = p
-    return OtherPath(new_path)
-
-
-def _ask_about_name(q, n):
-    click.echo(f"\n[cellpy] (setup) input {q}")
-    click.echo(f"[cellpy] (setup) current: {n}")
-    new_name = input("[cellpy] (setup) [KEEP/new value] >>> ").strip()
-    if not new_name:
-        new_name = n
-    return new_name
-
-
-def _create_dir(path, confirm=True, parents=True, exist_ok=True):
-    if isinstance(path, OtherPath):
-        if path.is_external:
-            return path
-    o = path.resolve()
-    if not o.is_dir():
-        o_parent = o.parent
-        create_dir = True
-        if confirm:
-            if not o_parent.is_dir():
-                create_dir = input(
-                    f"\n[cellpy] (setup) {o_parent} does not exist. Create it [y]/n ?"
-                )
-                if not create_dir:
-                    create_dir = True
-                elif create_dir in ["y", "Y"]:
-                    create_dir = True
-                else:
-                    create_dir = False
-
-        if create_dir:
-            try:
-                o.mkdir(parents=parents, exist_ok=exist_ok)
-                click.echo(f"[cellpy] (setup) Created {o}")
-            except FileExistsError:
-                click.echo(f"[cellpy] (setup) {o} already exists.")
-            except FileNotFoundError:
-                click.echo(f"[cellpy] (setup) {o} not available.")
-            except Exception as e:
-                click.echo(f"[cellpy] (setup) WARNING! Could not create {o}.")
-                logging.debug(e)
-                click.echo(f"[cellpy] (setup) ...continuing anyway.")
-        else:
-            click.echo(f"[cellpy] (setup) Could not create {o}")
-    return o
-
-
-def _check_import_cellpy():
-    try:
-        import cellpy
-        from cellpy import log
-        from cellpy.readers import cellreader
-
-        return True
-    except:
-        return False
-
-
-def _check_import_pyodbc():
-    import platform
-
-    from cellpy.parameters import prms
-
-    ODBC = prms._odbc
-    SEARCH_FOR_ODBC_DRIVERS = prms._search_for_odbc_driver
-
-    use_subprocess = prms.Instruments.Arbin.use_subprocess
-    detect_subprocess_need = prms.Instruments.Arbin.detect_subprocess_need
-    click.echo(f" reading prms")
-    click.echo(f" - ODBC: {ODBC}")
-    click.echo(f" - SEARCH_FOR_ODBC_DRIVERS: {SEARCH_FOR_ODBC_DRIVERS}")
-    click.echo(f" - use_subprocess: {use_subprocess}")
-    click.echo(f" - detect_subprocess_need: {detect_subprocess_need}")
-    click.echo(f" - stated office version: {prms.Instruments.Arbin.office_version}")
-
-    click.echo(" checking system")
-    is_posix = False
-    is_macos = False
-    if os.name == "posix":
-        is_posix = True
-        click.echo(f" - running on posix")
-    current_platform = platform.system()
-    if current_platform == "Darwin":
-        is_macos = True
-        click.echo(f" - running on a mac")
-
-    python_version, os_version = platform.architecture()
-    click.echo(f" - python version: {python_version}")
-    click.echo(f" - os version: {os_version}")
-
-    if not is_posix:
-        if not prms.Instruments.Arbin.sub_process_path:
-            sub_process_path = str(prms._sub_process_path)
-        else:
-            sub_process_path = str(prms.Instruments.Arbin.sub_process_path)
-        click.echo(f" stated path to sub-process: {sub_process_path}")
-        if not os.path.isfile(sub_process_path):
-            click.echo(f" - OBS! missing")
-
-    if is_posix:
-        click.echo(" checking existence of mdb-export")
-        sub_process_path = "mdb-export"
-        from subprocess import PIPE, run
-
-        command = ["command", "-v", sub_process_path]
-
-        try:
-            result = run(command, stdout=PIPE, stderr=PIPE, universal_newlines=True)
-            if result.returncode == 0:
-                click.echo(f" - found it: {result.stdout}")
-            else:
-                click.echo(f" - failed finding it")
-
-            if is_macos:
-                driver = "/usr/local/lib/libmdbodbc.dylib"
-                click.echo(f" looks like you are on a mac (driver set to\n {driver})")
-                if not os.path.isfile(driver):
-                    click.echo(" - but cannot find it!")
-                    return False
-            return True
-
-        except AssertionError:
-            click.echo(" - not found")
-            return False
-
-    # not posix - checking for odbc drivers
-    # 1) checking if you have defined one
-    try:
-        driver = prms.Instruments.Arbin.odbc_driver
-        if not driver:
-            raise AttributeError
-        click.echo("You have defined an odbc driver in your conifg file")
-        click.echo(f"driver: {driver}")
-    except AttributeError:
-        click.echo("FYI: you have not defined any odbc_driver(s)")
-        click.echo(
-            "(The name of the driver from the configuration file is "
-            "used as a backup when cellpy cannot locate a driver by itself)"
-        )
-
-    use_ado = False
-
-    if ODBC == "ado":
-        use_ado = True
-        click.echo(" you stated that you prefer the ado loader")
-        click.echo(" checking if adodbapi is installed")
-        try:
-            import adodbapi as dbloader
-        except ImportError:
-            use_ado = False
-            click.echo(" Failed! Try setting pyodbc as your loader or install")
-            click.echo(" adodbapi (http://adodbapi.sourceforge.net/)")
-
-    if not use_ado:
-        if ODBC == "pyodbc":
-            click.echo(" you stated that you prefer the pyodbc loader")
-            try:
-                import pyodbc as dbloader
-            except ImportError:
-                click.echo(" Failed! Could not import it.")
-                click.echo(" Try 'pip install pyodbc'")
-                dbloader = None
-
-        elif ODBC == "pypyodbc":
-            click.echo(" you stated that you prefer the pypyodbc loader")
-            try:
-                import pypyodbc as dbloader
-            except ImportError:
-                click.echo(" Failed! Could not import it.")
-                click.echo(" try 'pip install pypyodbc'")
-                click.echo(" or set pyodbc as your loader in your prm file")
-                click.echo(" (and install it)")
-                dbloader = None
-
-    click.echo(" searching for odbc drivers")
-    try:
-        drivers = [
-            driver
-            for driver in dbloader.drivers()
-            if "Microsoft Access Driver" in driver
-        ]
-        click.echo(f"Found these: {drivers}")
-        driver = drivers[0]
-        click.echo(f"odbc driver: {driver}")
-        return True
-
-    except IndexError as e:
-        logging.debug("Unfortunately, it seems the list of drivers is emtpy.")
-        click.echo(
-            "\nCould not find any odbc-drivers suitable for .res-type files. "
-            "Check out the homepage of pydobc for info on installing drivers"
-        )
-        click.echo(
-            "One solution that might work is downloading "
-            "the Microsoft Access database engine "
-            "(in correct bytes (32 or 64)) "
-            "from:\n"
-            "https://www.microsoft.com/en-us/download/details.aspx?id=13255"
-        )
-        click.echo("Or install mdbtools and set it up (check the cellpy docs for help)")
-        click.echo("\n")
-        return False
-
-
-def _check_config_file():
-    prm_file_name = _configloc()
-    prm_dict = prmreader._read_prm_file_without_updating(prm_file_name)
-    try:
-        prm_paths = prm_dict["Paths"]
-        required_dirs = [
-            "cellpydatadir",
-            "examplesdir",
-            "filelogdir",
-            "notebookdir",
-            "outdatadir",
-            "rawdatadir",
-            "batchfiledir",
-            "templatedir",
-            "db_path",
-        ]
-        missing = 0
-        for k in required_dirs:
-            value = prm_paths.get(k, None)
-            click.echo(f"{k}: {value}")
-            # splitting this into two if-statements to make it easier to debug if OtherPath changes
-            if value in OTHERPATHS:
-                logging.debug(
-                    "skipping check for external rawdatadir and cellpydatadir (for now)"
-                )
-                if not OtherPath(
-                    value
-                ).is_dir():  # Assuming OtherPath returns True if it is external.
-                    missing += 1
-                    click.echo("COULD NOT CONNECT!")
-                    click.echo(f"({value} is not a directory)")
-            elif value and not pathlib.Path(value).is_dir():
-                missing += 1
-                click.echo("COULD NOT CONNECT!")
-                click.echo(f"({value} is not a directory)")
-            if not value:
-                missing += 1
-                click.echo("MISSING")
-
-        value = prm_paths.get("db_filename", None)
-        click.echo(f"db_filename: {value}")
-        if not value:
-            missing += 1
-            click.echo("MISSING")
-
-        if missing:
-            return False
-        else:
-            return True
-
-    except Exception as e:
-        click.echo("Following error occurred:")
-        click.echo(e)
-        return False
-
-
-def _check(dry_run=False):
-    click.echo(" checking ".center(80, "="))
-    if dry_run:
-        click.echo("*** dry-run: skipping the test")
-        return
-    failed_checks = 0
-    number_of_checks = 0
-
-    def sub_check(check_type, check_func):
-        failed = 0
-        click.echo(f"[cellpy] * - Checking {check_type}")
-        if check_func():
-            click.echo(f"[cellpy] -> succeeded!")
-        else:
-            click.echo("f[cellpy] -> failed!!!!")
-            failed = 1
-        click.echo(80 * "-")
-        return failed
-
-    check_types = ["cellpy imports", "importing pyodbc", "configuration (prm) file"]
-    check_funcs = [_check_import_cellpy, _check_import_pyodbc, _check_config_file]
-
-    for ct, cf in zip(check_types, check_funcs):
-        try:
-            failed_checks += sub_check(ct, cf)
-        except Exception as e:
-            click.echo(f"[cellpy] check raised an exception ({e})")
-        number_of_checks += 1
-    succeeded_checks = number_of_checks - failed_checks
-    if failed_checks > 0:
-        click.echo(f"[cellpy] OH NO!!! You (or I) failed!")
-        click.echo(f"[cellpy] Failed {failed_checks} out of {number_of_checks} checks.")
-    else:
-        click.echo(
-            f"[cellpy] Succeeded {succeeded_checks} out of {number_of_checks} checks."
-        )
-    click.echo(80 * "=")
-
-
-def _write_config_file(user_dir, dst_file, init_filename, dry_run):
-    click.echo(" update configuration ".center(80, "-"))
-    click.echo("[cellpy] (setup) Writing configurations to user directory:")
-    click.echo(f"\n         {user_dir}\n")
-
-    if os.path.isfile(dst_file):
-        click.echo("[cellpy] (setup) File already exists!")
-        click.echo("[cellpy] (setup) Keeping most of the old configuration parameters")
-    try:
-        if dry_run:
-            click.echo(
-                f"*** dry-run: skipping actual saving of {dst_file} ***", color="red"
-            )
-        else:
-            click.echo(f"[cellpy] (setup) Saving file ({dst_file})")
-            save_prm_file(dst_file)
-
-    except ConfigFileNotWritten:
-        click.echo("[cellpy] (setup) Something went wrong! Could not write the file")
-        click.echo(
-            "[cellpy] (setup) Trying to write a file"
-            + f"called {prmreader.DEFAULT_FILENAME} instead"
-        )
-
-        try:
-            user_dir, dst_file = prmreader.get_user_dir_and_dst(init_filename)
-            if dry_run:
-                click.echo(
-                    f"*** dry-run: skipping actual saving of {dst_file} ***",
-                    color="red",
-                )
-            else:
-                save_prm_file(dst_file)
-
-        except ConfigFileNotWritten:
-            _txt = "[cellpy] (setup) No, that did not work either.\n"
-            _txt += "[cellpy] (setup) Well, guess you have to talk to the developers."
-            click.echo(_txt)
-    else:
-        click.echo(f"[cellpy] (setup) Configuration file written!")
-        click.echo(
-            f"[cellpy] (setup) OK! Now you can edit it. For example by "
-            f"issuing \n\n         [your-favourite-editor] {init_filename}\n"
-        )
-
-
-# ----------------------- edit ---------------------------------------
-@click.command()
-@click.option(
-    "--default-editor",
-    "-e",
-    default=None,
-    type=str,
-    help="try to use this editor instead (e.g. notepad.exe)",
-)
-def edit(default_editor):
-    """Edit your cellpy config file."""
-
-    config_file = _configloc()
-    if config_file:
-        config_file_str = str(config_file.resolve())
-
-        if default_editor is not None:
-            args = [default_editor, config_file_str]
-            click.echo(f"[cellpy] (edit) Calling '{default_editor}'")
-            try:
-                subprocess.call(args)
-            except:
-                click.echo(f"[cellpy] (edit) Failed!")
-                click.echo(
-                    "[cellpy] (edit) Try 'cellpy edit -e notepad.exe' if you are on Windows"
-                )
-
-        if default_editor is None:
-            try:
-                import editor
-
-                editor.edit(filename=config_file_str)
-            except ImportError:
-                click.echo(f"[cellpy] (edit) Failed!")
-                click.echo(
-                    f"[cellpy] (edit) Searching for editors uses the python-editor package"
-                )
-                click.echo(f"[cellpy] (edit) Possible fixes:")
-                click.echo(
-                    f"[cellpy] (edit) - provide a default editor "
-                    f"using the -e option (e.g. cellpy edit -e notepad.exe)"
-                )
-                click.echo(
-                    f"[cellpy] (edit) - install teh python-editor package "
-                    f"(pip install python-editor)"
-                )
-
-
-# ----------------------- info ---------------------------------------
-@click.command()
-@click.option("--version", "-v", is_flag=True, help="Print version information.")
-@click.option(
-    "--configloc", "-l", is_flag=True, help="Print full path to the config file."
-)
-@click.option("--params", "-p", is_flag=True, help="Dump all parameters to screen.")
-@click.option(
-    "--check",
-    "-c",
-    is_flag=True,
-    help="Do a sanity check to see if things" " works as they should.",
-)
-def info(version, configloc, params, check):
-    """This will give you some valuable information about your cellpy."""
-    complete_info = True
-
-    if check:
-        complete_info = False
-        _check()
-
-    if version:
-        complete_info = False
-        _version()
-
-    if configloc:
-        complete_info = False
-        _configloc()
-
-    if params:
-        complete_info = False
-        _dump_params()
-
-    if complete_info:
-        _version()
-        _configloc()
-
-
-# ----------------------- run ----------------------------------------
-@click.command()
-@click.option(
-    "--journal",
-    "-j",
-    is_flag=True,
-    help="Run a batch job defined in the given journal-file",
-)
-@click.option("--key", "-k", is_flag=True, help="Run a batch job defined by batch-name")
-@click.option(
-    "--folder",
-    "-f",
-    is_flag=True,
-    help="Run all batch jobs iteratively in a given folder",
-)
-@click.option(
-    "--cellpy-project",
-    "-p",
-    is_flag=True,
-    help="Use PaperMill to run the notebook(s) within the given project folder "
-    "(will only work properly if the notebooks can be sorted in correct run-order by 'sorted'). "
-    "Warning! since we are using `click` - the NAME will be 'converted' when it is loaded "
-    "(same as print(name) does) - "
-    "so you can't use backslash ('\\') as normal in windows (use either '/' or '\\\\' instead).",
-)
-@click.option("--debug", "-d", is_flag=True, help="Run in debug mode.")
-@click.option("--silent", "-s", is_flag=True, help="Run in silent mode.")
-@click.option("--raw", is_flag=True, help="Force loading raw-file(s).")
-@click.option("--cellpyfile", is_flag=True, help="Force cellpy-file(s).")
-@click.option("--minimal", is_flag=True, help="Minimal processing.")
-@click.option(
-    "--nom-cap",
-    default=None,
-    type=float,
-    help="nominal capacity (used in calculating rates etc)",
-)
-@click.option(
-    "--batch_col",
-    default=None,
-    type=str,
-    help="batch column (if selecting running from db)",
-)
-@click.option(
-    "--project",
-    default=None,
-    type=str,
-    help="name of the project (if selecting running from db)",
-)
-@click.option("--list", "-l", "list_", is_flag=True, help="List batch-files.")
-@click.argument("name", default="NONE")
-def run(
-    journal,
-    key,
-    folder,
-    cellpy_project,
-    debug,
-    silent,
-    raw,
-    cellpyfile,
-    minimal,
-    nom_cap,
-    batch_col,
-    project,
-    list_,
-    name,
-):
-    """Run a cellpy process (batch-job, edit db, ...).
-
-    You can use this to launch specific applications.
-
-    Examples:
-
-        edit your cellpy database
-
-           cellpy run db
-
-        run a batch job described in a journal file
-
-           cellpy run -j my_experiment.json
-
-    """
-    if list_:
-        _run_list(name)
-        return
-
-    if name == "NONE":
-        click.echo(
-            "Usage: cellpy run [OPTIONS] NAME\n"
-            "Try 'cellpy run --help' for help.\n\n"
-            "Error: Missing argument 'NAME'."
-        )
-        sys.exit(-1)
-
-    if debug:
-        click.echo("[cellpy] (run) debug mode on")
-
-    if silent:
-        click.echo("[cellpy] (run) silent mode on")
-
-    click.echo("[cellpy]\n")
-
-    if cellpy_project:
-        _run_project(name)
-
-    elif journal:
-        _run_journal(name, debug, silent, raw, cellpyfile, minimal, nom_cap)
-
-    elif folder:
-        _run_journals(name, debug, silent, raw, cellpyfile, minimal)
-
-    elif key:
-        _run_from_db(
-            name,
-            debug,
-            silent,
-            raw,
-            cellpyfile,
-            minimal,
-            nom_cap,
-            batch_col,
-            project,
-        )
-
-    elif name.lower() == "db":
-        _run_db(debug, silent)
-
-    else:
-        _run(name, debug, silent)
-
-
-def _run_from_db(
-    name,
-    debug,
-    silent,
-    raw,
-    cellpyfile,
-    minimal,
-    nom_cap,
-    batch_col,
-    project,
-):
-    click.echo(
-        f"running from db \nkey={name}, batch_col={batch_col}, project={project}"
-    )
-
-    kwargs = dict()
-    kwargs["name"] = name
-
-    if debug:
-        kwargs["default_log_level"] = "DEBUG"
-    if not minimal:
-        kwargs["export_raw"] = False
-        kwargs["export_cycles"] = False
-        kwargs["export_ica"] = False
-
-    if batch_col is not None:
-        kwargs["batch_col"] = batch_col
-    if project is None:
-        kwargs["project"] = "various"
-    else:
-        kwargs["project"] = project
-
-    click.echo("Warming up ...")
-
-    from cellpy.utils import batch
-
-    click.echo("  - starting batch processing")
-    b = batch.process_batch(
-        force_raw_file=raw,
-        force_cellpy=cellpyfile,
-        nom_cap=nom_cap,
-        backend="matplotlib",
-        **kwargs,
-    )
-
-    if b is not None and not silent:
-        print(b)
-    click.echo("---")
-
-
-def _run_journal(file_name, debug, silent, raw, cellpyfile, minimal, nom_cap):
-    click.echo(f"running journal {file_name}")
-    # click.echo(f" --debug [{debug}]")
-    # click.echo(f" --silent [{silent}]")
-    # click.echo(f" --raw [{raw}]")
-    # click.echo(f" --cellpyfile [{cellpyfile}]")
-    # click.echo(f" --minimal [{minimal}]")
-    # click.echo(f" --nom_cap [{nom_cap}] {type(nom_cap)}")
-
-    kwargs = dict()
-    if debug:
-        kwargs["default_log_level"] = "DEBUG"
-    if not minimal:
-        kwargs["export_raw"] = False
-        kwargs["export_cycles"] = False
-        kwargs["export_ica"] = False
-
-    from cellpy import prms
-    from cellpy.utils import batch
-
-    batchfiledir = pathlib.Path(prms.Paths.batchfiledir)
-    file = pathlib.Path(file_name)
-    if not file.is_file():
-        click.echo(f"file_name={file_name} not found - looking into batchfiledir")
-        if not batchfiledir.is_dir():
-            click.echo("batchfiledir not found - aborting")
-            return
-        file = batchfiledir / file.name
-
-    if not file.is_file():
-        click.echo(f"{file} not found - aborting")
-        return
-
-    b = batch.process_batch(
-        file,
-        force_raw_file=raw,
-        force_cellpy=cellpyfile,
-        nom_cap=nom_cap,
-        backend="matplotlib",
-        **kwargs,
-    )
-    if b is not None and not silent:
-        print(b)
-    click.echo("---")
-
-
-def _run_list(batchfiledir):
-    from cellpy import prms
-
-    if batchfiledir == "NONE" or batchfiledir is None:
-        batchfiledir = pathlib.Path(prms.Paths.batchfiledir)
-    else:
-        batchfiledir = pathlib.Path(batchfiledir).resolve()
-
-    if batchfiledir.is_dir():
-        click.echo(f"Content of '{batchfiledir}':\n")
-        i = 0
-        for i, f in enumerate(batchfiledir.glob("cellpy*.json")):
-            click.echo(f"{f.name}")
-        if i:
-            print(f"\nnumber of batch-files located: {i}")
-        else:
-            print("No batch-files found in this directory.")
-    else:
-        click.echo(f"{batchfiledir} not found.")
-
-
-def _run_journals(folder_name, debug, silent, raw, cellpyfile, minimal):
-    click.echo(f"running journals in {folder_name}")
-    # click.echo(f" --debug [{debug}]")
-    # click.echo(f" --silent [{silent}]")
-    # click.echo(f" --raw [{raw}]")
-    # click.echo(f" --cellpyfile [{cellpyfile}]")
-    # click.echo(f" --minimal [{minimal}]")
-
-    kwargs = dict()
-    if debug:
-        kwargs["default_log_level"] = "DEBUG"
-    if not minimal:
-        kwargs["export_raw"] = False
-        kwargs["export_cycles"] = False
-        kwargs["export_ica"] = False
-
-    from cellpy.utils import batch
-
-    folder_name = pathlib.Path(folder_name).resolve()
-
-    if not folder_name.is_dir():
-        click.echo(f"{folder_name} not found - aborting")
-        return
-
-    batch.iterate_batches(
-        folder_name, force_raw_file=raw, force_cellpy=cellpyfile, silent=True, **kwargs
-    )
-    click.echo("---")
-
-
-def _run_project(our_new_project, **kwargs):
-    try:
-        import papermill as pm
-    except ImportError:
-        click.echo(
-            "[cellpy]: You need to install papermill for automatically execute the notebooks."
-        )
-        click.echo("[cellpy]: You can install it using pip like this:")
-        click.echo(" >> pip install papermill")
-        return
-    our_new_project = pathlib.Path(our_new_project)
-    click.echo(f"[cellpy]: trying to run notebooks in {our_new_project}")
-    notebooks = sorted(list(our_new_project.glob("*.ipynb")))
-    for notebook in notebooks:
-        click.echo(f"[cellpy - papermill] running {notebook.name}")
-        pm.execute_notebook(notebook, notebook, parameters=kwargs)
-
-
-def _run(name, debug, silent):
-    click.echo(f"running {name}")
-    click.echo(f" --debug [{debug}]")
-    click.echo(f" --silent [{silent}]")
-
-
-def _run_db(debug, silent):
-    import platform
-
-    from cellpy import prms
-
-    if not silent:
-        click.echo(f"running database editor")
-    if debug:
-        click.echo("running in debug-mode, but nothing to tell")
-
-    db_path = Path(prms.Paths.db_path) / prms.Paths.db_filename
-
-    if platform.system() == "Windows":
-        try:
-            os.system(f'start excel "{str(db_path)}"')
-        except Exception as e:
-            click.echo("Something went wrong trying to open")
-            click.echo(db_path)
-            print()
-            print(e)
-
-    elif platform.system() == "Linux":
-        click.echo("RUNNING LINUX")
-        # not tested
-        subprocess.check_call(["open", "-a", "Microsoft Excel", db_path])
-
-    elif platform.system() == "Darwin":
-        click.echo(f" - running on a mac")
-        subprocess.check_call(["open", "-a", "Microsoft Excel", db_path])
-
-    else:
-        print("RUNNING SOMETHING ELSE")
-        print(platform.system())
-        # not tested
-        subprocess.check_call(["open", "-a", "Microsoft Excel", db_path])
-
-
-# ----------------------- pull ---------------------------------------
-@click.command()
-@click.option("--tests", "-t", is_flag=True, help="Download test-files from repo.")
-@click.option(
-    "--examples", "-e", is_flag=True, help="Download example-files from repo."
-)
-@click.option("--clone", "-c", is_flag=True, help="Clone the full repo.")
-@click.option("--directory", "-d", default=None, help="Save into custom directory DIR")
-@click.option("--password", "-p", default=None, help="Password option for the repo")
-def pull(tests, examples, clone, directory, password):
-    """Download examples or tests from the big internet (needs git)."""
-    if directory is not None:
-        click.echo(f"[cellpy] (pull) custom directory: {directory}")
-    else:
-        directory = pathlib.Path(prmreader.prms.Paths.examplesdir)
-
-    if password is not None:
-        click.echo("DEV MODE: password provided")
-    if clone:
-        _clone_repo(directory, password)
-    else:
-        if tests:
-            _pull_tests(directory, password)
-        if examples:
-            _pull_examples(directory, password)
-        else:
-            click.echo(
-                f"[cellpy] (pull) Nothing selected for pulling. "
-                f"Please select an option (--tests,--examples, -clone, ...) "
-            )
-
-
-def _clone_repo(directory, password):
-    directory = pathlib.Path(directory)
-    txt = "[cellpy] The plan is that this "
-    txt += "[cellpy] cmd will pull (clone) the cellpy repo.\n"
-    txt += "[cellpy] For now it only prints the link to the git-hub\n"
-    txt += "[cellpy] repository:\n"
-    txt += "[cellpy]\n"
-    txt += "[cellpy] https://github.com/jepegit/cellpy.git\n"
-    txt += "[cellpy]\n"
-    click.echo(txt)
-
-
-def _pull_tests(directory, pw=None):
-    txt = (
-        "[cellpy] (pull) Pulling tests from",
-        " https://github.com/jepegit/cellpy.git",
-    )
-    click.echo(txt)
-    _pull(gdirpath="tests", rootpath=directory, pw=pw)
-    _pull(gdirpath="testdata", rootpath=directory, pw=pw)
-
-
-def _pull_examples(directory, pw):
-    txt = (
-        "[cellpy] (pull) Pulling examples from",
-        " https://github.com/jepegit/cellpy.git",
-    )
-    click.echo(txt)
-    _pull(gdirpath="examples", rootpath=directory, pw=pw)
-
-
-def _version():
-    txt = "[cellpy] version: " + str(VERSION)
-    click.echo(txt)
-
-
-def _configloc():
-    _, config_file_name = prmreader.get_user_dir_and_dst()
-    click.echo("[cellpy] ->%s" % config_file_name)
-    if not os.path.isfile(config_file_name):
-        click.echo("[cellpy] File does not exist!")
-    else:
-        return config_file_name
-
-
-def _dump_params():
-    click.echo("[cellpy] Dumping parameters to screen:\n")
-    prmreader.info()
-
-
-def _download_g_blob(name, local_path):
-    import urllib.request
-
-    dirs = local_path.parent
-    if not dirs.is_dir():
-        click.echo(f"[cellpy] (pull) creating dir: {dirs}")
-        dirs.mkdir(parents=True)
-
-    filename, headers = urllib.request.urlretrieve(
-        name.download_url, filename=local_path
-    )
-    click.echo(f"[cellpy] (pull) downloaded blob: {filename}")
-
-
-def _parse_g_dir(repo, gdirpath):
-    """parses a repo directory two-levels deep"""
-    for f in repo.get_contents(gdirpath):
-        if f.type == "dir":
-            for sf in repo.get_contents(f.path):
-                yield sf
-        else:
-            yield f
-
-
-def _get_user_name():
-    return "jepegit"
-
-
-def _get_pw(method):
-    if method == "ask":
-        return getpass.getpass()
-    elif method == "env":
-        return os.environ.get(GITHUB_PWD_VAR_NAME, None)
-
-    else:
-        return None
-
-
-def _pull(gdirpath="examples", rootpath=None, u=None, pw=None):
-    if rootpath is None:
-        rootpath = prmreader.prms.Paths.examplesdir
-
-    rootpath = pathlib.Path(rootpath)
-
-    ndirpath = rootpath / gdirpath
-
-    if pw is not None:
-        click.echo(" DEV MODE ".center(80, "-"))
-        u = _get_user_name()
-        if pw == "ask":
-            click.echo("   - ask for password")
-            pw = _get_pw(pw)
-        elif pw == "env":
-            click.echo("   - check environ for password ")
-            pw = _get_pw(pw)
-            click.echo("   - got something")
-            if pw is None:
-                click.echo("   - only None")
-                u = None
-
-    g = Github(u, pw)
-    repo = g.get_repo(REPO)
-
-    click.echo(f"[cellpy] (pull) pulling {gdirpath}")
-    click.echo(f"[cellpy] (pull) -> {ndirpath}")
-
-    if not ndirpath.is_dir():
-        click.echo(f"[cellpy] (pull) creating dir: {ndirpath}")
-        ndirpath.mkdir(parents=True)
-
-    for gfile in _parse_g_dir(repo, gdirpath):
-        gfilename = pathlib.Path(gfile.path)
-        nfilename = rootpath / gfilename
-
-        _download_g_blob(gfile, nfilename)
-
-
-def _get_default_template():
-    template = "standard"
-    try:
-        template = prmreader.prms.Batch.template
-    except:
-        logging.debug("You dont have any default template defined in you .conf file")
-    return template
-
-
-def _read_local_templates(local_templates_path=None):
-    if local_templates_path is None:
-        local_templates_path = pathlib.Path(prmreader.prms.Paths.templatedir)
-    templates = {}
-    for p in list(local_templates_path.rglob("cellpy_cookie*.zip")):
-        label = p.stem.strip()[len("cellpy_cookie_") :]
-        templates[label] = (str(p), None)
-    logging.debug(f"Found the following templates: {templates}")
-    return templates
-
-
-# ----------------------- new ----------------------------------------
-@click.command()
-@click.option("--template", "-t", help="Provide template name.")
-@click.option("--directory", "-d", default=None, help="Create in custom directory.")
-@click.option(
-    "--project",
-    "-p",
-    default=None,
-    help="Provide project name (i.e. sub-directory name).",
-)
-@click.option(
-    "--experiment",
-    "-e",
-    default=None,
-    help="Provide experiment name (i.e. lookup-value).",
-)
-@click.option(
-    "--local-user-template",
-    "-u",
-    is_flag=True,
-    default=False,
-    help="Use local template from the templates directory.",
-)
-@click.option("--serve", "-s", "serve_", is_flag=True, help="Run Jupyter.")
-@click.option(
-    "--run",
-    "-r",
-    "run_",
-    is_flag=True,
-    help="Use PaperMill to run the notebook(s) from the template "
-    "(will only work properly if the notebooks can be sorted in correct run-order by 'sorted'.",
-)
-@click.option(
-    "--lab",
-    "-j",
-    is_flag=True,
-    help="Use Jupyter Lab instead of Notebook when serving.",
-)
-@click.option(
-    "--list", "-l", "list_", is_flag=True, help="List available templates and exit."
-)
-def new(
-    template,
-    directory,
-    project,
-    experiment,
-    local_user_template,
-    serve_,
-    run_,
-    lab,
-    list_,
-):
-    """Set up a batch experiment (might need git installed)."""
-    _new(
-        template,
-        directory=directory,
-        project_dir=project,
-        session_id=experiment,
-        local_user_template=local_user_template,
-        serve_=serve_,
-        run_=run_,
-        lab=lab,
-        list_=list_,
-    )
-
-
-def _new(
-    template: str,
-    directory: Union[Path, str, None] = None,
-    project_dir: Union[str, None] = None,
-    local_user_template: bool = False,
-    serve_: bool = False,
-    run_: bool = False,
-    lab: bool = False,
-    list_: bool = False,
-    session_id: str = "experiment_001",
-    no_input: bool = False,
-    cookie_directory: str = "",
-):
-    """Set up a batch experiment (might need git installed).
-
-    Args:
-        template: short-name of template.
-        directory: the directory for your cellpy projects.
-        local_user_template: use local template if True.
-        serve_: serve the notebook after creation if True.
-        run_: run the notebooks using papermill if True.
-        lab: use jupyter-lab instead of jupyter notebook if True.
-        list_: list all available templates and return if True.
-        project_dir: your project directory.
-        session_id: the lookup value.
-        no_input: accept defaults if True (only valid when providing project_dir and session_id)
-        cookie_directory: name of the directory for your cookie (inside the repository or zip file).
-    Returns:
-        None
-    """
-
-    from cellpy.parameters import prms
-
-    if list_:
-        click.echo(f"\n[cellpy] batch templates")
-
-        default_template = _get_default_template()
-        local_templates = _read_local_templates()
-        local_templates_path = prmreader.prms.Paths.templatedir
-        registered_templates = prms._registered_templates
-        click.echo(f"[cellpy] - default: {default_template}")
-        click.echo("[cellpy] - registered templates (on github):")
-        for label, link in registered_templates.items():
-            click.echo(f"\t\t{label:18s} {link}")
-
-        if local_templates:
-            click.echo(f"[cellpy] - local templates ({local_templates_path}):")
-            for label, link in local_templates.items():
-                click.echo(f"\t\t{label:18s} {link}")
-        else:
-            click.echo(f"[cellpy] - local templates ({local_templates_path}): none")
-
-        return
-
-    if project_dir is None or session_id is None:
-        no_input = False
-
-    if not template:
-        template = _get_default_template()
-
-    if lab:
-        server = "lab"
-    else:
-        server = "notebook"
-
-    try:
-        import cookiecutter.exceptions
-        import cookiecutter.main
-        import cookiecutter.prompt
-
-    except ModuleNotFoundError:
-        click.echo("Could not import cookiecutter.")
-        click.echo("Try installing it, for example by writing:")
-        click.echo("\npip install cookiecutter\n")
-
-    click.echo(f"Template: {template}")
-    if local_user_template:
-        # forcing using local template
-        templates = _read_local_templates()
-
-        if not templates:
-            click.echo(
-                "You asked me to use a local template, but you have none. Aborting."
-            )
-            return
-    else:
-        templates = prms._registered_templates
-        if local_templates := _read_local_templates():
-            templates.update(local_templates)
-
-    if not template.lower() in templates.keys():
-        click.echo("This template does not exist. Aborting.")
-        return
-
-    if directory is None:
-        logging.debug("no dir given")
-        directory = prms.Paths.notebookdir
-
-    if not os.path.isdir(directory):
-        click.echo("Sorry. This did not work as expected!")
-        click.echo(f" - {directory} does not exist")
-        return
-
-    directory = Path(directory)
-    selected_project_dir = None
-
-    if project_dir:
-        selected_project_dir = directory / project_dir
-        if not selected_project_dir.is_dir():
-            if cookiecutter.prompt.read_user_yes_no(
-                f"{project_dir} does not exist. Create?", "yes"
-            ):
-                os.mkdir(selected_project_dir)
-                click.echo(f"Created {selected_project_dir}")
-
-            else:
-                selected_project_dir = None
-                click.echo(f"Select another directory instead")
-
-    if not selected_project_dir:
-        project_dirs = [
-            d.name
-            for d in directory.iterdir()
-            if d.is_dir() and not d.name.startswith(".")
-        ]
-        project_dirs.insert(0, "[create new dir]")
-
-        project_dir = cookiecutter.prompt.read_user_choice(
-            "project folder", project_dirs
-        )
-
-        if project_dir == "[create new dir]":
-            default_name = "cellpy_project"
-            temp_default_name = default_name
-            for j in range(999):
-                if temp_default_name in project_dirs:
-                    temp_default_name = default_name + str(j + 1).zfill(3)
-                else:
-                    default_name = temp_default_name
-                    break
-
-            project_dir = cookiecutter.prompt.read_user_variable(
-                "New name", default_name
-            )
-            try:
-                os.mkdir(directory / project_dir)
-                click.echo(f"created {project_dir}")
-            except FileExistsError:
-                click.echo("OK - but this directory already exists!")
-        selected_project_dir = directory / project_dir
-
-    # get a list of all folders
-    existing_projects = os.listdir(selected_project_dir)
-
-    os.chdir(selected_project_dir)
-    cellpy_version = cellpy.__version__
-
-    try:
-        selected_template, cookie_dir = templates[template.lower()]
-
-        if cookie_directory:
-            cookie_dir = cookie_directory
-        if not cookie_dir:
-            cookie_dir = template.lower()
-
-        cookiecutter.main.cookiecutter(
-            selected_template,
-            extra_context={
-                "author_name": os.getlogin(),
-                "project_name": project_dir,
-                "cellpy_version": cellpy_version,
-                "session_id": session_id,
-            },
-            no_input=no_input,
-            directory=cookie_dir,
-        )
-    except cookiecutter.exceptions.OutputDirExistsException as e:
-        click.echo("Sorry. This did not work as expected!")
-        click.echo(" - cookiecutter refused to create the project")
-        click.echo(e)
-
-    if serve_:
-        os.chdir(directory)
-        _serve(server)
-
-    if run_:
-        try:
-            import papermill as pm
-        except ImportError:
-            click.echo(
-                "[cellpy]: You need to install papermill for automatically execute the notebooks."
-            )
-            click.echo("[cellpy]: You can install it using pip like this:")
-            click.echo(" >> pip install papermill")
-            return
-        new_existing_projects = os.listdir(selected_project_dir)
-        our_new_projects = list(set(new_existing_projects) - set(existing_projects))
-
-        if not len(our_new_projects):
-            click.echo(
-                "[cellpy]: Sorry, could not deiced what is the new project "
-                "- so I don't dare to try to execute automatically."
-            )
-            return
-        our_new_project = selected_project_dir / our_new_projects[0]
-
-        _run_project(our_new_project)
-
-
-def _serve(server):
-    click.echo(f"serving with jupyter {server}")
-    subprocess.run(["jupyter", server], check=True)
-    click.echo("Finished serving.")
-
-
-# ----------------------- serve ---------------------------------------
-@click.command()
-@click.option("--lab", "-l", is_flag=True, help="Use Jupyter Lab instead of Notebook")
-@click.option("--directory", "-d", default=None, help="Start in custom directory DIR")
-def serve(lab, directory):
-    """Start a Jupyter server."""
-
-    from cellpy.parameters import prms
-
-    if directory is None:
-        directory = prms.Paths.notebookdir
-    elif directory == "home":
-        directory = Path().home()
-    elif directory == "here":
-        directory = Path(os.getcwd())
-
-    if not os.path.isdir(directory):
-        click.echo("Sorry. This did not work as expected!")
-        click.echo(f" - {directory} does not exist")
-        return
-
-    if lab:
-        server = "lab"
-    else:
-        server = "notebook"
-
-    os.chdir(directory)
-    _serve(server)
-
-
-cli.add_command(setup)
-cli.add_command(info)
-cli.add_command(edit)
-cli.add_command(pull)
-cli.add_command(run)
-cli.add_command(new)
-cli.add_command(serve)
-
-
-# tests etc
-def _main_pull():
-    if sys.platform == "win32":
-        rootpath = pathlib.Path(r"C:\Temp\cellpy_user")
-    else:
-        rootpath = pathlib.Path("/Users/jepe/scripting/tmp/cellpy_test_user")
-    _pull_examples(rootpath, pw="env")
-    _pull_tests(rootpath, pw="env")
-    # _pull(gdirpath="examples", rootpath=rootpath, u="ask", pw="ask")
-    # _pull(gdirpath="tests", rootpath=rootpath, u="ask", pw="ask")
-    # _pull(gdirpath="testdata", rootpath=rootpath, u="ask", pw="ask")
-
-
-def _main():
-    file_name = prmreader.create_custom_init_filename()
-    click.echo(file_name)
-    user_directory, destination_file_name = prmreader.get_user_dir_and_dst(file_name)
-    click.echo(user_directory)
-    click.echo(destination_file_name)
-    click.echo("trying to save it")
-    save_prm_file(destination_file_name + "_dummy")
-
-    click.echo(" Testing setup ".center(80, "="))
-    setup(["--interactive", "--reset"])
-
-
-def _cli_setup_interactive():
-    from click.testing import CliRunner
-
-    if sys.platform == "win32":
-        root_dir = r"C:\Temp\cellpy_user"
-    else:
-        root_dir = "/Users/jepe/scripting/tmp/cellpy_test_user"
-    testuser = "tester"
-    init_filename = prmreader.create_custom_init_filename(testuser)
-    dst_file = get_dst_file(root_dir, init_filename)
-    init_file = pathlib.Path(dst_file)
-    opts = list()
-    opts.append("setup")
-    opts.append("-i")
-    # opts.append("-nr")
-    opts.append("-r")
-    opts.extend(["-d", root_dir])
-    opts.extend(["-t", testuser])
-
-    input_str = "\n"  # out
-    input_str += "\n"  # rawdatadir
-    input_str += "\n"  # cellpyfiles
-    input_str += "\n"  # log
-    input_str += "\n"  # examples
-    input_str += "\n"  # dbfolder
-    input_str += "\n"  # dbfile
-    runner = CliRunner()
-    result = runner.invoke(cli, opts, input=input_str)
-
-    click.echo(" out ".center(80, "."))
-    click.echo(result.output)
-    from pprint import pprint
-
-    pprint(prmreader.prms.Paths)
-    click.echo(" conf-file ".center(80, "."))
-    click.echo(init_file)
-    click.echo()
-    with init_file.open() as f:
-        for line in f.readlines():
-            click.echo(line.strip())
-
-
-def check_it(var=None):
-    import pathlib
-    import sys
-
-    p_env = pathlib.Path(sys.prefix)
-    print(p_env.name)
-    new(list_=True)
-
-
-if __name__ == "__main__":
-    u1 = os.getlogin()
-    u2 = os.path.expanduser("~")
-    u3 = os.environ.get("USERNAME")
-
-    print(u1)
-    print(u2)
-    print(u3)
-    # check_it()
-    # click.echo("\n\n", " RUNNING MAIN PULL ".center(80, "*"), "\n")
-    # _main_pull()
-    # click.echo("ok")
+import base64
+import getpass
+import logging
+import os
+import pathlib
+from pprint import pprint
+import re
+import subprocess
+import sys
+from typing import Union
+import urllib
+from pathlib import Path
+
+import click
+import pkg_resources
+from github import Github
+
+import cellpy._version
+from cellpy.exceptions import ConfigFileNotWritten
+from cellpy.parameters import prmreader
+from cellpy.parameters.internal_settings import OTHERPATHS
+from cellpy.internals.core import OtherPath
+
+VERSION = cellpy._version.__version__
+REPO = "jepegit/cellpy"
+USER = "jepegit"
+GITHUB_PWD_VAR_NAME = "GD_PWD"
+
+
+def save_prm_file(prm_filename):
+    """saves (writes) the prms to file"""
+    prmreader._write_prm_file(prm_filename)
+
+
+def get_package_prm_dir():
+    """gets the folder where the cellpy package lives"""
+    prm_dir = pkg_resources.resource_filename("cellpy", "parameters")
+    return pathlib.Path(prm_dir)
+
+
+def get_default_config_file_path(init_filename=None):
+    """gets the path to the default config-file"""
+    prm_dir = get_package_prm_dir()
+    if not init_filename:
+        init_filename = prmreader.DEFAULT_FILENAME
+    src = prm_dir / init_filename
+    return src
+
+
+def get_dst_file(user_dir, init_filename):
+    user_dir = pathlib.Path(user_dir)
+    dst_file = user_dir / init_filename
+    return dst_file
+
+
+def check_if_needed_modules_exists():
+    pass
+
+
+def modify_config_file():
+    pass
+
+
+def create_cellpy_folders():
+    pass
+
+
+@click.group("cellpy")
+def cli():
+    pass
+
+
+# ----------------------- setup --------------------------------------
+@click.command()
+@click.option(
+    "--interactive",
+    "-i",
+    is_flag=True,
+    default=False,
+    help="Allows you to specify div. folders and setting.",
+)
+@click.option(
+    "--not-relative",
+    "-nr",
+    is_flag=True,
+    default=False,
+    help="If root-dir is given, put it directly in the root (/) folder"
+    " i.e. don't put it in your home directory. Defaults to False. Remark"
+    " that if you specifically write a path name instead of selecting the"
+    " suggested default, the path you write will be used as is.",
+)
+@click.option(
+    "--dry-run",
+    "-dr",
+    is_flag=True,
+    default=False,
+    help="Run setup in dry mode (only print - do not execute). This is"
+    " typically used when developing and testing cellpy. Defaults to"
+    " False.",
+)
+@click.option(
+    "--reset",
+    "-r",
+    is_flag=True,
+    default=False,
+    help="Do not suggest path defaults based on your current configuration-file",
+)
+@click.option(
+    "--root-dir",
+    "-d",
+    default=None,
+    type=click.Path(),
+    help="Use custom root dir. If not given, your home directory"
+    " will be used as the top level where cellpy-folders"
+    " will be put. The folder path must follow"
+    " directly after this option (if used). Example:\n"
+    " $ cellpy setup -d 'MyDir'",
+)
+@click.option(
+    "--folder-name",
+    "-n",
+    default=None,
+    type=click.Path(),
+    help="",
+)
+@click.option(
+    "--test_user", "-t", default=None, help="Fake name for fake user (for testing)"
+)
+def setup(interactive, not_relative, dry_run, reset, root_dir, folder_name, test_user):
+    """This will help you to set up cellpy."""
+
+    click.echo("[cellpy] (setup)")
+    click.echo(f"[cellpy] root-dir: {root_dir}")
+
+    # generate variables
+    init_filename = prmreader.create_custom_init_filename()
+    user_dir, dst_file = prmreader.get_user_dir_and_dst(init_filename)
+
+    if dry_run:
+        click.echo("Create custom init filename and get user_dir and destination")
+        click.echo(f"Got the following parameters:")
+        click.echo(f" - init_filename: {init_filename}")
+        click.echo(f" - user_dir: {user_dir}")
+        click.echo(f" - dst_file: {dst_file}")
+        click.echo(f" - not_relative: {not_relative}")
+
+    if root_dir and not interactive:
+        click.echo("[cellpy] custom root-dir can only be used in interactive mode")
+        click.echo("[cellpy] -> setting interactive mode")
+        interactive = True
+
+    if not root_dir:
+        root_dir = user_dir
+        # root_dir = pathlib.Path(os.getcwd())
+    root_dir = pathlib.Path(root_dir)
+
+    if dry_run:
+        click.echo(f" - root_dir: {root_dir}")
+
+    if test_user:
+        click.echo(f"[cellpy] (setup) DEV-MODE test_user: {test_user}")
+        init_filename = prmreader.create_custom_init_filename(test_user)
+        user_dir = root_dir
+        dst_file = get_dst_file(user_dir, init_filename)
+        click.echo(f"[cellpy] (setup) DEV-MODE user_dir: {user_dir}")
+        click.echo(f"[cellpy] (setup) DEV-MODE dst_file: {dst_file}")
+
+    if not pathlib.Path(dst_file).is_file():
+        click.echo(f"[cellpy] {dst_file} not found -> I will make one for you!")
+        reset = True
+
+    if interactive:
+        click.echo(" interactive mode ".center(80, "-"))
+        _update_paths(
+            custom_dir=root_dir,
+            relative_home=not not_relative,
+            default_dir=folder_name,
+            dry_run=dry_run,
+            reset=reset,
+        )
+        _write_config_file(user_dir, dst_file, init_filename, dry_run)
+        _check(dry_run=dry_run)
+
+    else:
+        if reset:
+            _update_paths(
+                user_dir,
+                False,
+                default_dir=folder_name,
+                dry_run=dry_run,
+                reset=True,
+                silent=True,
+            )
+        _write_config_file(user_dir, dst_file, init_filename, dry_run)
+        _check(dry_run=dry_run)
+
+
+def _update_paths(
+    custom_dir=None,
+    relative_home=True,
+    reset=False,
+    dry_run=False,
+    default_dir=None,
+    silent=False,
+):
+    # please, refactor me :-(
+
+    h = prmreader.get_user_dir()
+
+    if default_dir is None:
+        default_dir = "cellpy_data"
+
+    if dry_run:
+        click.echo(f" - default_dir: {default_dir}")
+        click.echo(f" - custom_dir: {custom_dir}")
+        click.echo(f" - retalive_home: {relative_home}")
+
+    if custom_dir:
+        reset = True
+        if relative_home:
+            h = h / custom_dir
+        if not custom_dir.parts[-1] == default_dir:
+            h = h / default_dir
+
+    if not reset:
+        outdatadir = pathlib.Path(prmreader.prms.Paths.outdatadir)
+        rawdatadir = OtherPath(prmreader.prms.Paths.rawdatadir)
+        cellpydatadir = OtherPath(prmreader.prms.Paths.cellpydatadir)
+        filelogdir = pathlib.Path(prmreader.prms.Paths.filelogdir)
+        examplesdir = pathlib.Path(prmreader.prms.Paths.examplesdir)
+        db_path = pathlib.Path(prmreader.prms.Paths.db_path)
+        db_filename = prmreader.prms.Paths.db_filename
+        notebookdir = pathlib.Path(prmreader.prms.Paths.notebookdir)
+        batchfiledir = pathlib.Path(prmreader.prms.Paths.batchfiledir)
+        templatedir = pathlib.Path(prmreader.prms.Paths.templatedir)
+        instrumentdir = pathlib.Path(prmreader.prms.Paths.instrumentsdir)
+    else:
+        outdatadir = "out"
+        rawdatadir = "raw"
+        cellpydatadir = "cellpyfiles"
+        filelogdir = "logs"
+        examplesdir = "examples"
+        db_path = "db"
+        db_filename = "cellpy_db.xlsx"
+        notebookdir = "notebooks"
+        batchfiledir = "batchfiles"
+        templatedir = "templates"
+        instrumentdir = "instruments"
+
+    outdatadir = h / outdatadir
+    rawdatadir = h / rawdatadir
+    cellpydatadir = h / cellpydatadir
+    filelogdir = h / filelogdir
+    examplesdir = h / examplesdir
+    db_path = h / db_path
+    notebookdir = h / notebookdir
+    batchfiledir = h / batchfiledir
+    templatedir = h / templatedir
+    instrumentdir = h / instrumentdir
+
+    if dry_run:
+        click.echo(f" - base (h): {h}")
+
+    if not silent:
+        outdatadir = _ask_about_path(
+            "where to output processed data and results", outdatadir
+        )
+        rawdatadir = _ask_about_otherpath("where your raw data are located", rawdatadir)
+        cellpydatadir = _ask_about_otherpath("where to put cellpy-files", cellpydatadir)
+        filelogdir = _ask_about_path("where to dump the log-files", filelogdir)
+        examplesdir = _ask_about_path(
+            "where to download cellpy examples and tests", examplesdir
+        )
+        db_path = _ask_about_path("what folder your db file lives in", db_path)
+        db_filename = _ask_about_name("the name of your db-file", db_filename)
+        notebookdir = _ask_about_path(
+            "where to put your jupyter notebooks", notebookdir
+        )
+        batchfiledir = _ask_about_path("where to put your batch files", batchfiledir)
+        templatedir = _ask_about_path("where to put your batch files", templatedir)
+        instrumentdir = _ask_about_path("where to put your batch files", instrumentdir)
+
+    # update folders based on suggestions
+    for d in [
+        outdatadir,
+        rawdatadir,
+        cellpydatadir,
+        filelogdir,
+        examplesdir,
+        notebookdir,
+        db_path,
+        batchfiledir,
+        templatedir,
+        instrumentdir,
+    ]:
+        if not dry_run:
+            _create_dir(d)
+        else:
+            click.echo(f"dry run (so I did not create {d})")
+
+    # update config-file based on suggestions
+    prmreader.prms.Paths.outdatadir = str(outdatadir)
+    prmreader.prms.Paths.rawdatadir = str(rawdatadir)
+    prmreader.prms.Paths.cellpydatadir = str(cellpydatadir)
+    prmreader.prms.Paths.filelogdir = str(filelogdir)
+    prmreader.prms.Paths.examplesdir = str(examplesdir)
+    prmreader.prms.Paths.db_path = str(db_path)
+    prmreader.prms.Paths.db_filename = str(db_filename)
+    prmreader.prms.Paths.notebookdir = str(notebookdir)
+    prmreader.prms.Paths.batchfiledir = str(batchfiledir)
+    prmreader.prms.Paths.templatedir = str(templatedir)
+    prmreader.prms.Paths.instrumentdir = str(instrumentdir)
+
+
+def _ask_about_path(q, p):
+    click.echo(f"\n[cellpy] (setup) input {q}")
+    click.echo(f"[cellpy] (setup) current: {p}")
+    new_path = input("[cellpy] (setup) [KEEP/new value] >>> ").strip()
+    if not new_path:
+        new_path = p
+    return pathlib.Path(new_path)
+
+
+def _ask_about_otherpath(q, p):
+    click.echo(f"\n[cellpy] (setup) input {q}")
+    click.echo(f"[cellpy] (setup) current: {p}")
+    new_path = input("[cellpy] (setup) [KEEP/new value] >>> ").strip()
+    if not new_path:
+        new_path = p
+    return OtherPath(new_path)
+
+
+def _ask_about_name(q, n):
+    click.echo(f"\n[cellpy] (setup) input {q}")
+    click.echo(f"[cellpy] (setup) current: {n}")
+    new_name = input("[cellpy] (setup) [KEEP/new value] >>> ").strip()
+    if not new_name:
+        new_name = n
+    return new_name
+
+
+def _create_dir(path, confirm=True, parents=True, exist_ok=True):
+    if isinstance(path, OtherPath):
+        if path.is_external:
+            return path
+    o = path.resolve()
+    if not o.is_dir():
+        o_parent = o.parent
+        create_dir = True
+        if confirm:
+            if not o_parent.is_dir():
+                create_dir = input(
+                    f"\n[cellpy] (setup) {o_parent} does not exist. Create it [y]/n ?"
+                )
+                if not create_dir:
+                    create_dir = True
+                elif create_dir in ["y", "Y"]:
+                    create_dir = True
+                else:
+                    create_dir = False
+
+        if create_dir:
+            try:
+                o.mkdir(parents=parents, exist_ok=exist_ok)
+                click.echo(f"[cellpy] (setup) Created {o}")
+            except FileExistsError:
+                click.echo(f"[cellpy] (setup) {o} already exists.")
+            except FileNotFoundError:
+                click.echo(f"[cellpy] (setup) {o} not available.")
+            except Exception as e:
+                click.echo(f"[cellpy] (setup) WARNING! Could not create {o}.")
+                logging.debug(e)
+                click.echo(f"[cellpy] (setup) ...continuing anyway.")
+        else:
+            click.echo(f"[cellpy] (setup) Could not create {o}")
+    return o
+
+
+def _check_import_cellpy():
+    try:
+        import cellpy
+        from cellpy import log
+        from cellpy.readers import cellreader
+
+        return True
+    except:
+        return False
+
+
+def _check_import_pyodbc():
+    import platform
+
+    from cellpy.parameters import prms
+
+    ODBC = prms._odbc
+    SEARCH_FOR_ODBC_DRIVERS = prms._search_for_odbc_driver
+
+    use_subprocess = prms.Instruments.Arbin.use_subprocess
+    detect_subprocess_need = prms.Instruments.Arbin.detect_subprocess_need
+    click.echo(f" reading prms")
+    click.echo(f" - ODBC: {ODBC}")
+    click.echo(f" - SEARCH_FOR_ODBC_DRIVERS: {SEARCH_FOR_ODBC_DRIVERS}")
+    click.echo(f" - use_subprocess: {use_subprocess}")
+    click.echo(f" - detect_subprocess_need: {detect_subprocess_need}")
+    click.echo(f" - stated office version: {prms.Instruments.Arbin.office_version}")
+
+    click.echo(" checking system")
+    is_posix = False
+    is_macos = False
+    if os.name == "posix":
+        is_posix = True
+        click.echo(f" - running on posix")
+    current_platform = platform.system()
+    if current_platform == "Darwin":
+        is_macos = True
+        click.echo(f" - running on a mac")
+
+    python_version, os_version = platform.architecture()
+    click.echo(f" - python version: {python_version}")
+    click.echo(f" - os version: {os_version}")
+
+    if not is_posix:
+        if not prms.Instruments.Arbin.sub_process_path:
+            sub_process_path = str(prms._sub_process_path)
+        else:
+            sub_process_path = str(prms.Instruments.Arbin.sub_process_path)
+        click.echo(f" stated path to sub-process: {sub_process_path}")
+        if not os.path.isfile(sub_process_path):
+            click.echo(f" - OBS! missing")
+
+    if is_posix:
+        click.echo(" checking existence of mdb-export")
+        sub_process_path = "mdb-export"
+        from subprocess import PIPE, run
+
+        command = ["command", "-v", sub_process_path]
+
+        try:
+            result = run(command, stdout=PIPE, stderr=PIPE, universal_newlines=True)
+            if result.returncode == 0:
+                click.echo(f" - found it: {result.stdout}")
+            else:
+                click.echo(f" - failed finding it")
+
+            if is_macos:
+                driver = "/usr/local/lib/libmdbodbc.dylib"
+                click.echo(f" looks like you are on a mac (driver set to\n {driver})")
+                if not os.path.isfile(driver):
+                    click.echo(" - but cannot find it!")
+                    return False
+            return True
+
+        except AssertionError:
+            click.echo(" - not found")
+            return False
+
+    # not posix - checking for odbc drivers
+    # 1) checking if you have defined one
+    try:
+        driver = prms.Instruments.Arbin.odbc_driver
+        if not driver:
+            raise AttributeError
+        click.echo("You have defined an odbc driver in your conifg file")
+        click.echo(f"driver: {driver}")
+    except AttributeError:
+        click.echo("FYI: you have not defined any odbc_driver(s)")
+        click.echo(
+            "(The name of the driver from the configuration file is "
+            "used as a backup when cellpy cannot locate a driver by itself)"
+        )
+
+    use_ado = False
+
+    if ODBC == "ado":
+        use_ado = True
+        click.echo(" you stated that you prefer the ado loader")
+        click.echo(" checking if adodbapi is installed")
+        try:
+            import adodbapi as dbloader
+        except ImportError:
+            use_ado = False
+            click.echo(" Failed! Try setting pyodbc as your loader or install")
+            click.echo(" adodbapi (http://adodbapi.sourceforge.net/)")
+
+    if not use_ado:
+        if ODBC == "pyodbc":
+            click.echo(" you stated that you prefer the pyodbc loader")
+            try:
+                import pyodbc as dbloader
+            except ImportError:
+                click.echo(" Failed! Could not import it.")
+                click.echo(" Try 'pip install pyodbc'")
+                dbloader = None
+
+        elif ODBC == "pypyodbc":
+            click.echo(" you stated that you prefer the pypyodbc loader")
+            try:
+                import pypyodbc as dbloader
+            except ImportError:
+                click.echo(" Failed! Could not import it.")
+                click.echo(" try 'pip install pypyodbc'")
+                click.echo(" or set pyodbc as your loader in your prm file")
+                click.echo(" (and install it)")
+                dbloader = None
+
+    click.echo(" searching for odbc drivers")
+    try:
+        drivers = [
+            driver
+            for driver in dbloader.drivers()
+            if "Microsoft Access Driver" in driver
+        ]
+        click.echo(f"Found these: {drivers}")
+        driver = drivers[0]
+        click.echo(f"odbc driver: {driver}")
+        return True
+
+    except IndexError as e:
+        logging.debug("Unfortunately, it seems the list of drivers is emtpy.")
+        click.echo(
+            "\nCould not find any odbc-drivers suitable for .res-type files. "
+            "Check out the homepage of pydobc for info on installing drivers"
+        )
+        click.echo(
+            "One solution that might work is downloading "
+            "the Microsoft Access database engine "
+            "(in correct bytes (32 or 64)) "
+            "from:\n"
+            "https://www.microsoft.com/en-us/download/details.aspx?id=13255"
+        )
+        click.echo("Or install mdbtools and set it up (check the cellpy docs for help)")
+        click.echo("\n")
+        return False
+
+
+def _check_config_file():
+    prm_file_name = _configloc()
+    prm_dict = prmreader._read_prm_file_without_updating(prm_file_name)
+    try:
+        prm_paths = prm_dict["Paths"]
+        required_dirs = [
+            "cellpydatadir",
+            "examplesdir",
+            "filelogdir",
+            "notebookdir",
+            "outdatadir",
+            "rawdatadir",
+            "batchfiledir",
+            "templatedir",
+            "db_path",
+        ]
+        missing = 0
+        for k in required_dirs:
+            value = prm_paths.get(k, None)
+            click.echo(f"{k}: {value}")
+            # splitting this into two if-statements to make it easier to debug if OtherPath changes
+            if k in OTHERPATHS:
+                print(
+                    f"skipping check for external {k} (for now)"
+                )
+                # if not OtherPath(
+                #     value
+                # ).is_dir():  # Assuming OtherPath returns True if it is external.
+                #     missing += 1
+                #     click.echo("COULD NOT CONNECT!")
+                #     click.echo(f"({value} is not a directory)")
+            elif value and not pathlib.Path(value).is_dir():
+                missing += 1
+                click.echo("COULD NOT CONNECT!")
+                click.echo(f"({value} is not a directory)")
+            if not value:
+                missing += 1
+                click.echo("MISSING")
+
+        value = prm_paths.get("db_filename", None)
+        click.echo(f"db_filename: {value}")
+        if not value:
+            missing += 1
+            click.echo("MISSING")
+
+        if missing:
+            return False
+        else:
+            return True
+
+    except Exception as e:
+        click.echo("Following error occurred:")
+        click.echo(e)
+        return False
+
+
+def _check(dry_run=False):
+    click.echo(" checking ".center(80, "="))
+    if dry_run:
+        click.echo("*** dry-run: skipping the test")
+        return
+    failed_checks = 0
+    number_of_checks = 0
+
+    def sub_check(check_type, check_func):
+        failed = 0
+        click.echo(f"[cellpy] * - Checking {check_type}")
+        if check_func():
+            click.echo(f"[cellpy] -> succeeded!")
+        else:
+            click.echo("f[cellpy] -> failed!!!!")
+            failed = 1
+        click.echo(80 * "-")
+        return failed
+
+    check_types = ["cellpy imports", "importing pyodbc", "configuration (prm) file"]
+    check_funcs = [_check_import_cellpy, _check_import_pyodbc, _check_config_file]
+
+    for ct, cf in zip(check_types, check_funcs):
+        try:
+            failed_checks += sub_check(ct, cf)
+        except Exception as e:
+            click.echo(f"[cellpy] check raised an exception ({e})")
+        number_of_checks += 1
+    succeeded_checks = number_of_checks - failed_checks
+    if failed_checks > 0:
+        click.echo(f"[cellpy] OH NO!!! You (or I) failed!")
+        click.echo(f"[cellpy] Failed {failed_checks} out of {number_of_checks} checks.")
+    else:
+        click.echo(
+            f"[cellpy] Succeeded {succeeded_checks} out of {number_of_checks} checks."
+        )
+    click.echo(80 * "=")
+
+
+def _write_config_file(user_dir, dst_file, init_filename, dry_run):
+    click.echo(" update configuration ".center(80, "-"))
+    click.echo("[cellpy] (setup) Writing configurations to user directory:")
+    click.echo(f"\n         {user_dir}\n")
+
+    if os.path.isfile(dst_file):
+        click.echo("[cellpy] (setup) File already exists!")
+        click.echo("[cellpy] (setup) Keeping most of the old configuration parameters")
+    try:
+        if dry_run:
+            click.echo(
+                f"*** dry-run: skipping actual saving of {dst_file} ***", color="red"
+            )
+        else:
+            click.echo(f"[cellpy] (setup) Saving file ({dst_file})")
+            save_prm_file(dst_file)
+
+    except ConfigFileNotWritten:
+        click.echo("[cellpy] (setup) Something went wrong! Could not write the file")
+        click.echo(
+            "[cellpy] (setup) Trying to write a file"
+            + f"called {prmreader.DEFAULT_FILENAME} instead"
+        )
+
+        try:
+            user_dir, dst_file = prmreader.get_user_dir_and_dst(init_filename)
+            if dry_run:
+                click.echo(
+                    f"*** dry-run: skipping actual saving of {dst_file} ***",
+                    color="red",
+                )
+            else:
+                save_prm_file(dst_file)
+
+        except ConfigFileNotWritten:
+            _txt = "[cellpy] (setup) No, that did not work either.\n"
+            _txt += "[cellpy] (setup) Well, guess you have to talk to the developers."
+            click.echo(_txt)
+    else:
+        click.echo(f"[cellpy] (setup) Configuration file written!")
+        click.echo(
+            f"[cellpy] (setup) OK! Now you can edit it. For example by "
+            f"issuing \n\n         [your-favourite-editor] {init_filename}\n"
+        )
+
+
+# ----------------------- edit ---------------------------------------
+@click.command()
+@click.option(
+    "--default-editor",
+    "-e",
+    default=None,
+    type=str,
+    help="try to use this editor instead (e.g. notepad.exe)",
+)
+def edit(default_editor):
+    """Edit your cellpy config file."""
+
+    config_file = _configloc()
+    if config_file:
+        config_file_str = str(config_file.resolve())
+
+        if default_editor is not None:
+            args = [default_editor, config_file_str]
+            click.echo(f"[cellpy] (edit) Calling '{default_editor}'")
+            try:
+                subprocess.call(args)
+            except:
+                click.echo(f"[cellpy] (edit) Failed!")
+                click.echo(
+                    "[cellpy] (edit) Try 'cellpy edit -e notepad.exe' if you are on Windows"
+                )
+
+        if default_editor is None:
+            try:
+                import editor
+
+                editor.edit(filename=config_file_str)
+            except ImportError:
+                click.echo(f"[cellpy] (edit) Failed!")
+                click.echo(
+                    f"[cellpy] (edit) Searching for editors uses the python-editor package"
+                )
+                click.echo(f"[cellpy] (edit) Possible fixes:")
+                click.echo(
+                    f"[cellpy] (edit) - provide a default editor "
+                    f"using the -e option (e.g. cellpy edit -e notepad.exe)"
+                )
+                click.echo(
+                    f"[cellpy] (edit) - install teh python-editor package "
+                    f"(pip install python-editor)"
+                )
+
+
+# ----------------------- info ---------------------------------------
+@click.command()
+@click.option("--version", "-v", is_flag=True, help="Print version information.")
+@click.option(
+    "--configloc", "-l", is_flag=True, help="Print full path to the config file."
+)
+@click.option("--params", "-p", is_flag=True, help="Dump all parameters to screen.")
+@click.option(
+    "--check",
+    "-c",
+    is_flag=True,
+    help="Do a sanity check to see if things" " works as they should.",
+)
+def info(version, configloc, params, check):
+    """This will give you some valuable information about your cellpy."""
+    complete_info = True
+
+    if check:
+        complete_info = False
+        _check()
+
+    if version:
+        complete_info = False
+        _version()
+
+    if configloc:
+        complete_info = False
+        _configloc()
+
+    if params:
+        complete_info = False
+        _dump_params()
+
+    if complete_info:
+        _version()
+        _configloc()
+
+
+# ----------------------- run ----------------------------------------
+@click.command()
+@click.option(
+    "--journal",
+    "-j",
+    is_flag=True,
+    help="Run a batch job defined in the given journal-file",
+)
+@click.option("--key", "-k", is_flag=True, help="Run a batch job defined by batch-name")
+@click.option(
+    "--folder",
+    "-f",
+    is_flag=True,
+    help="Run all batch jobs iteratively in a given folder",
+)
+@click.option(
+    "--cellpy-project",
+    "-p",
+    is_flag=True,
+    help="Use PaperMill to run the notebook(s) within the given project folder "
+    "(will only work properly if the notebooks can be sorted in correct run-order by 'sorted'). "
+    "Warning! since we are using `click` - the NAME will be 'converted' when it is loaded "
+    "(same as print(name) does) - "
+    "so you can't use backslash ('\\') as normal in windows (use either '/' or '\\\\' instead).",
+)
+@click.option("--debug", "-d", is_flag=True, help="Run in debug mode.")
+@click.option("--silent", "-s", is_flag=True, help="Run in silent mode.")
+@click.option("--raw", is_flag=True, help="Force loading raw-file(s).")
+@click.option("--cellpyfile", is_flag=True, help="Force cellpy-file(s).")
+@click.option("--minimal", is_flag=True, help="Minimal processing.")
+@click.option(
+    "--nom-cap",
+    default=None,
+    type=float,
+    help="nominal capacity (used in calculating rates etc)",
+)
+@click.option(
+    "--batch_col",
+    default=None,
+    type=str,
+    help="batch column (if selecting running from db)",
+)
+@click.option(
+    "--project",
+    default=None,
+    type=str,
+    help="name of the project (if selecting running from db)",
+)
+@click.option("--list", "-l", "list_", is_flag=True, help="List batch-files.")
+@click.argument("name", default="NONE")
+def run(
+    journal,
+    key,
+    folder,
+    cellpy_project,
+    debug,
+    silent,
+    raw,
+    cellpyfile,
+    minimal,
+    nom_cap,
+    batch_col,
+    project,
+    list_,
+    name,
+):
+    """Run a cellpy process (batch-job, edit db, ...).
+
+    You can use this to launch specific applications.
+
+    Examples:
+
+        edit your cellpy database
+
+           cellpy run db
+
+        run a batch job described in a journal file
+
+           cellpy run -j my_experiment.json
+
+    """
+    if list_:
+        _run_list(name)
+        return
+
+    if name == "NONE":
+        click.echo(
+            "Usage: cellpy run [OPTIONS] NAME\n"
+            "Try 'cellpy run --help' for help.\n\n"
+            "Error: Missing argument 'NAME'."
+        )
+        sys.exit(-1)
+
+    if debug:
+        click.echo("[cellpy] (run) debug mode on")
+
+    if silent:
+        click.echo("[cellpy] (run) silent mode on")
+
+    click.echo("[cellpy]\n")
+
+    if cellpy_project:
+        _run_project(name)
+
+    elif journal:
+        _run_journal(name, debug, silent, raw, cellpyfile, minimal, nom_cap)
+
+    elif folder:
+        _run_journals(name, debug, silent, raw, cellpyfile, minimal)
+
+    elif key:
+        _run_from_db(
+            name,
+            debug,
+            silent,
+            raw,
+            cellpyfile,
+            minimal,
+            nom_cap,
+            batch_col,
+            project,
+        )
+
+    elif name.lower() == "db":
+        _run_db(debug, silent)
+
+    else:
+        _run(name, debug, silent)
+
+
+def _run_from_db(
+    name,
+    debug,
+    silent,
+    raw,
+    cellpyfile,
+    minimal,
+    nom_cap,
+    batch_col,
+    project,
+):
+    click.echo(
+        f"running from db \nkey={name}, batch_col={batch_col}, project={project}"
+    )
+
+    kwargs = dict()
+    kwargs["name"] = name
+
+    if debug:
+        kwargs["default_log_level"] = "DEBUG"
+    if not minimal:
+        kwargs["export_raw"] = False
+        kwargs["export_cycles"] = False
+        kwargs["export_ica"] = False
+
+    if batch_col is not None:
+        kwargs["batch_col"] = batch_col
+    if project is None:
+        kwargs["project"] = "various"
+    else:
+        kwargs["project"] = project
+
+    click.echo("Warming up ...")
+
+    from cellpy.utils import batch
+
+    click.echo("  - starting batch processing")
+    b = batch.process_batch(
+        force_raw_file=raw,
+        force_cellpy=cellpyfile,
+        nom_cap=nom_cap,
+        backend="matplotlib",
+        **kwargs,
+    )
+
+    if b is not None and not silent:
+        print(b)
+    click.echo("---")
+
+
+def _run_journal(file_name, debug, silent, raw, cellpyfile, minimal, nom_cap):
+    click.echo(f"running journal {file_name}")
+    # click.echo(f" --debug [{debug}]")
+    # click.echo(f" --silent [{silent}]")
+    # click.echo(f" --raw [{raw}]")
+    # click.echo(f" --cellpyfile [{cellpyfile}]")
+    # click.echo(f" --minimal [{minimal}]")
+    # click.echo(f" --nom_cap [{nom_cap}] {type(nom_cap)}")
+
+    kwargs = dict()
+    if debug:
+        kwargs["default_log_level"] = "DEBUG"
+    if not minimal:
+        kwargs["export_raw"] = False
+        kwargs["export_cycles"] = False
+        kwargs["export_ica"] = False
+
+    from cellpy import prms
+    from cellpy.utils import batch
+
+    batchfiledir = pathlib.Path(prms.Paths.batchfiledir)
+    file = pathlib.Path(file_name)
+    if not file.is_file():
+        click.echo(f"file_name={file_name} not found - looking into batchfiledir")
+        if not batchfiledir.is_dir():
+            click.echo("batchfiledir not found - aborting")
+            return
+        file = batchfiledir / file.name
+
+    if not file.is_file():
+        click.echo(f"{file} not found - aborting")
+        return
+
+    b = batch.process_batch(
+        file,
+        force_raw_file=raw,
+        force_cellpy=cellpyfile,
+        nom_cap=nom_cap,
+        backend="matplotlib",
+        **kwargs,
+    )
+    if b is not None and not silent:
+        print(b)
+    click.echo("---")
+
+
+def _run_list(batchfiledir):
+    from cellpy import prms
+
+    if batchfiledir == "NONE" or batchfiledir is None:
+        batchfiledir = pathlib.Path(prms.Paths.batchfiledir)
+    else:
+        batchfiledir = pathlib.Path(batchfiledir).resolve()
+
+    if batchfiledir.is_dir():
+        click.echo(f"Content of '{batchfiledir}':\n")
+        i = 0
+        for i, f in enumerate(batchfiledir.glob("cellpy*.json")):
+            click.echo(f"{f.name}")
+        if i:
+            print(f"\nnumber of batch-files located: {i}")
+        else:
+            print("No batch-files found in this directory.")
+    else:
+        click.echo(f"{batchfiledir} not found.")
+
+
+def _run_journals(folder_name, debug, silent, raw, cellpyfile, minimal):
+    click.echo(f"running journals in {folder_name}")
+    # click.echo(f" --debug [{debug}]")
+    # click.echo(f" --silent [{silent}]")
+    # click.echo(f" --raw [{raw}]")
+    # click.echo(f" --cellpyfile [{cellpyfile}]")
+    # click.echo(f" --minimal [{minimal}]")
+
+    kwargs = dict()
+    if debug:
+        kwargs["default_log_level"] = "DEBUG"
+    if not minimal:
+        kwargs["export_raw"] = False
+        kwargs["export_cycles"] = False
+        kwargs["export_ica"] = False
+
+    from cellpy.utils import batch
+
+    folder_name = pathlib.Path(folder_name).resolve()
+
+    if not folder_name.is_dir():
+        click.echo(f"{folder_name} not found - aborting")
+        return
+
+    batch.iterate_batches(
+        folder_name, force_raw_file=raw, force_cellpy=cellpyfile, silent=True, **kwargs
+    )
+    click.echo("---")
+
+
+def _run_project(our_new_project, **kwargs):
+    try:
+        import papermill as pm
+    except ImportError:
+        click.echo(
+            "[cellpy]: You need to install papermill for automatically execute the notebooks."
+        )
+        click.echo("[cellpy]: You can install it using pip like this:")
+        click.echo(" >> pip install papermill")
+        return
+    our_new_project = pathlib.Path(our_new_project)
+    click.echo(f"[cellpy]: trying to run notebooks in {our_new_project}")
+    notebooks = sorted(list(our_new_project.glob("*.ipynb")))
+    for notebook in notebooks:
+        click.echo(f"[cellpy - papermill] running {notebook.name}")
+        pm.execute_notebook(notebook, notebook, parameters=kwargs)
+
+
+def _run(name, debug, silent):
+    click.echo(f"running {name}")
+    click.echo(f" --debug [{debug}]")
+    click.echo(f" --silent [{silent}]")
+
+
+def _run_db(debug, silent):
+    import platform
+
+    from cellpy import prms
+
+    if not silent:
+        click.echo(f"running database editor")
+    if debug:
+        click.echo("running in debug-mode, but nothing to tell")
+
+    db_path = Path(prms.Paths.db_path) / prms.Paths.db_filename
+
+    if platform.system() == "Windows":
+        try:
+            os.system(f'start excel "{str(db_path)}"')
+        except Exception as e:
+            click.echo("Something went wrong trying to open")
+            click.echo(db_path)
+            print()
+            print(e)
+
+    elif platform.system() == "Linux":
+        click.echo("RUNNING LINUX")
+        # not tested
+        subprocess.check_call(["open", "-a", "Microsoft Excel", db_path])
+
+    elif platform.system() == "Darwin":
+        click.echo(f" - running on a mac")
+        subprocess.check_call(["open", "-a", "Microsoft Excel", db_path])
+
+    else:
+        print("RUNNING SOMETHING ELSE")
+        print(platform.system())
+        # not tested
+        subprocess.check_call(["open", "-a", "Microsoft Excel", db_path])
+
+
+# ----------------------- pull ---------------------------------------
+@click.command()
+@click.option("--tests", "-t", is_flag=True, help="Download test-files from repo.")
+@click.option(
+    "--examples", "-e", is_flag=True, help="Download example-files from repo."
+)
+@click.option("--clone", "-c", is_flag=True, help="Clone the full repo.")
+@click.option("--directory", "-d", default=None, help="Save into custom directory DIR")
+@click.option("--password", "-p", default=None, help="Password option for the repo")
+def pull(tests, examples, clone, directory, password):
+    """Download examples or tests from the big internet (needs git)."""
+    if directory is not None:
+        click.echo(f"[cellpy] (pull) custom directory: {directory}")
+    else:
+        directory = pathlib.Path(prmreader.prms.Paths.examplesdir)
+
+    if password is not None:
+        click.echo("DEV MODE: password provided")
+    if clone:
+        _clone_repo(directory, password)
+    else:
+        if tests:
+            _pull_tests(directory, password)
+        if examples:
+            _pull_examples(directory, password)
+        else:
+            click.echo(
+                f"[cellpy] (pull) Nothing selected for pulling. "
+                f"Please select an option (--tests,--examples, -clone, ...) "
+            )
+
+
+def _clone_repo(directory, password):
+    directory = pathlib.Path(directory)
+    txt = "[cellpy] The plan is that this "
+    txt += "[cellpy] cmd will pull (clone) the cellpy repo.\n"
+    txt += "[cellpy] For now it only prints the link to the git-hub\n"
+    txt += "[cellpy] repository:\n"
+    txt += "[cellpy]\n"
+    txt += "[cellpy] https://github.com/jepegit/cellpy.git\n"
+    txt += "[cellpy]\n"
+    click.echo(txt)
+
+
+def _pull_tests(directory, pw=None):
+    txt = (
+        "[cellpy] (pull) Pulling tests from",
+        " https://github.com/jepegit/cellpy.git",
+    )
+    click.echo(txt)
+    _pull(gdirpath="tests", rootpath=directory, pw=pw)
+    _pull(gdirpath="testdata", rootpath=directory, pw=pw)
+
+
+def _pull_examples(directory, pw):
+    txt = (
+        "[cellpy] (pull) Pulling examples from",
+        " https://github.com/jepegit/cellpy.git",
+    )
+    click.echo(txt)
+    _pull(gdirpath="examples", rootpath=directory, pw=pw)
+
+
+def _version():
+    txt = "[cellpy] version: " + str(VERSION)
+    click.echo(txt)
+
+
+def _configloc():
+    _, config_file_name = prmreader.get_user_dir_and_dst()
+    click.echo("[cellpy] ->%s" % config_file_name)
+    if not os.path.isfile(config_file_name):
+        click.echo("[cellpy] File does not exist!")
+    else:
+        return config_file_name
+
+
+def _dump_params():
+    click.echo("[cellpy] Dumping parameters to screen:\n")
+    prmreader.info()
+
+
+def _download_g_blob(name, local_path):
+    import urllib.request
+
+    dirs = local_path.parent
+    if not dirs.is_dir():
+        click.echo(f"[cellpy] (pull) creating dir: {dirs}")
+        dirs.mkdir(parents=True)
+
+    filename, headers = urllib.request.urlretrieve(
+        name.download_url, filename=local_path
+    )
+    click.echo(f"[cellpy] (pull) downloaded blob: {filename}")
+
+
+def _parse_g_dir(repo, gdirpath):
+    """parses a repo directory two-levels deep"""
+    for f in repo.get_contents(gdirpath):
+        if f.type == "dir":
+            for sf in repo.get_contents(f.path):
+                yield sf
+        else:
+            yield f
+
+
+def _get_user_name():
+    return "jepegit"
+
+
+def _get_pw(method):
+    if method == "ask":
+        return getpass.getpass()
+    elif method == "env":
+        return os.environ.get(GITHUB_PWD_VAR_NAME, None)
+
+    else:
+        return None
+
+
+def _pull(gdirpath="examples", rootpath=None, u=None, pw=None):
+    if rootpath is None:
+        rootpath = prmreader.prms.Paths.examplesdir
+
+    rootpath = pathlib.Path(rootpath)
+
+    ndirpath = rootpath / gdirpath
+
+    if pw is not None:
+        click.echo(" DEV MODE ".center(80, "-"))
+        u = _get_user_name()
+        if pw == "ask":
+            click.echo("   - ask for password")
+            pw = _get_pw(pw)
+        elif pw == "env":
+            click.echo("   - check environ for password ")
+            pw = _get_pw(pw)
+            click.echo("   - got something")
+            if pw is None:
+                click.echo("   - only None")
+                u = None
+
+    g = Github(u, pw)
+    repo = g.get_repo(REPO)
+
+    click.echo(f"[cellpy] (pull) pulling {gdirpath}")
+    click.echo(f"[cellpy] (pull) -> {ndirpath}")
+
+    if not ndirpath.is_dir():
+        click.echo(f"[cellpy] (pull) creating dir: {ndirpath}")
+        ndirpath.mkdir(parents=True)
+
+    for gfile in _parse_g_dir(repo, gdirpath):
+        gfilename = pathlib.Path(gfile.path)
+        nfilename = rootpath / gfilename
+
+        _download_g_blob(gfile, nfilename)
+
+
+def _get_default_template():
+    template = "standard"
+    try:
+        template = prmreader.prms.Batch.template
+    except:
+        logging.debug("You dont have any default template defined in you .conf file")
+    return template
+
+
+def _read_local_templates(local_templates_path=None):
+    if local_templates_path is None:
+        local_templates_path = pathlib.Path(prmreader.prms.Paths.templatedir)
+    templates = {}
+    for p in list(local_templates_path.rglob("cellpy_cookie*.zip")):
+        label = p.stem.strip()[len("cellpy_cookie_") :]
+        templates[label] = (str(p), None)
+    logging.debug(f"Found the following templates: {templates}")
+    return templates
+
+
+# ----------------------- new ----------------------------------------
+@click.command()
+@click.option("--template", "-t", help="Provide template name.")
+@click.option("--directory", "-d", default=None, help="Create in custom directory.")
+@click.option(
+    "--project",
+    "-p",
+    default=None,
+    help="Provide project name (i.e. sub-directory name).",
+)
+@click.option(
+    "--experiment",
+    "-e",
+    default=None,
+    help="Provide experiment name (i.e. lookup-value).",
+)
+@click.option(
+    "--local-user-template",
+    "-u",
+    is_flag=True,
+    default=False,
+    help="Use local template from the templates directory.",
+)
+@click.option("--serve", "-s", "serve_", is_flag=True, help="Run Jupyter.")
+@click.option(
+    "--run",
+    "-r",
+    "run_",
+    is_flag=True,
+    help="Use PaperMill to run the notebook(s) from the template "
+    "(will only work properly if the notebooks can be sorted in correct run-order by 'sorted'.",
+)
+@click.option(
+    "--lab",
+    "-j",
+    is_flag=True,
+    help="Use Jupyter Lab instead of Notebook when serving.",
+)
+@click.option(
+    "--list", "-l", "list_", is_flag=True, help="List available templates and exit."
+)
+def new(
+    template,
+    directory,
+    project,
+    experiment,
+    local_user_template,
+    serve_,
+    run_,
+    lab,
+    list_,
+):
+    """Set up a batch experiment (might need git installed)."""
+    _new(
+        template,
+        directory=directory,
+        project_dir=project,
+        session_id=experiment,
+        local_user_template=local_user_template,
+        serve_=serve_,
+        run_=run_,
+        lab=lab,
+        list_=list_,
+    )
+
+
+def _new(
+    template: str,
+    directory: Union[Path, str, None] = None,
+    project_dir: Union[str, None] = None,
+    local_user_template: bool = False,
+    serve_: bool = False,
+    run_: bool = False,
+    lab: bool = False,
+    list_: bool = False,
+    session_id: str = "experiment_001",
+    no_input: bool = False,
+    cookie_directory: str = "",
+):
+    """Set up a batch experiment (might need git installed).
+
+    Args:
+        template: short-name of template.
+        directory: the directory for your cellpy projects.
+        local_user_template: use local template if True.
+        serve_: serve the notebook after creation if True.
+        run_: run the notebooks using papermill if True.
+        lab: use jupyter-lab instead of jupyter notebook if True.
+        list_: list all available templates and return if True.
+        project_dir: your project directory.
+        session_id: the lookup value.
+        no_input: accept defaults if True (only valid when providing project_dir and session_id)
+        cookie_directory: name of the directory for your cookie (inside the repository or zip file).
+    Returns:
+        None
+    """
+
+    from cellpy.parameters import prms
+
+    if list_:
+        click.echo(f"\n[cellpy] batch templates")
+
+        default_template = _get_default_template()
+        local_templates = _read_local_templates()
+        local_templates_path = prmreader.prms.Paths.templatedir
+        registered_templates = prms._registered_templates
+        click.echo(f"[cellpy] - default: {default_template}")
+        click.echo("[cellpy] - registered templates (on github):")
+        for label, link in registered_templates.items():
+            click.echo(f"\t\t{label:18s} {link}")
+
+        if local_templates:
+            click.echo(f"[cellpy] - local templates ({local_templates_path}):")
+            for label, link in local_templates.items():
+                click.echo(f"\t\t{label:18s} {link}")
+        else:
+            click.echo(f"[cellpy] - local templates ({local_templates_path}): none")
+
+        return
+
+    if project_dir is None or session_id is None:
+        no_input = False
+
+    if not template:
+        template = _get_default_template()
+
+    if lab:
+        server = "lab"
+    else:
+        server = "notebook"
+
+    try:
+        import cookiecutter.exceptions
+        import cookiecutter.main
+        import cookiecutter.prompt
+
+    except ModuleNotFoundError:
+        click.echo("Could not import cookiecutter.")
+        click.echo("Try installing it, for example by writing:")
+        click.echo("\npip install cookiecutter\n")
+
+    click.echo(f"Template: {template}")
+    if local_user_template:
+        # forcing using local template
+        templates = _read_local_templates()
+
+        if not templates:
+            click.echo(
+                "You asked me to use a local template, but you have none. Aborting."
+            )
+            return
+    else:
+        templates = prms._registered_templates
+        if local_templates := _read_local_templates():
+            templates.update(local_templates)
+
+    if not template.lower() in templates.keys():
+        click.echo("This template does not exist. Aborting.")
+        return
+
+    if directory is None:
+        logging.debug("no dir given")
+        directory = prms.Paths.notebookdir
+
+    if not os.path.isdir(directory):
+        click.echo("Sorry. This did not work as expected!")
+        click.echo(f" - {directory} does not exist")
+        return
+
+    directory = Path(directory)
+    selected_project_dir = None
+
+    if project_dir:
+        selected_project_dir = directory / project_dir
+        if not selected_project_dir.is_dir():
+            if cookiecutter.prompt.read_user_yes_no(
+                f"{project_dir} does not exist. Create?", "yes"
+            ):
+                os.mkdir(selected_project_dir)
+                click.echo(f"Created {selected_project_dir}")
+
+            else:
+                selected_project_dir = None
+                click.echo(f"Select another directory instead")
+
+    if not selected_project_dir:
+        project_dirs = [
+            d.name
+            for d in directory.iterdir()
+            if d.is_dir() and not d.name.startswith(".")
+        ]
+        project_dirs.insert(0, "[create new dir]")
+
+        project_dir = cookiecutter.prompt.read_user_choice(
+            "project folder", project_dirs
+        )
+
+        if project_dir == "[create new dir]":
+            default_name = "cellpy_project"
+            temp_default_name = default_name
+            for j in range(999):
+                if temp_default_name in project_dirs:
+                    temp_default_name = default_name + str(j + 1).zfill(3)
+                else:
+                    default_name = temp_default_name
+                    break
+
+            project_dir = cookiecutter.prompt.read_user_variable(
+                "New name", default_name
+            )
+            try:
+                os.mkdir(directory / project_dir)
+                click.echo(f"created {project_dir}")
+            except FileExistsError:
+                click.echo("OK - but this directory already exists!")
+        selected_project_dir = directory / project_dir
+
+    # get a list of all folders
+    existing_projects = os.listdir(selected_project_dir)
+
+    os.chdir(selected_project_dir)
+    cellpy_version = cellpy.__version__
+
+    try:
+        selected_template, cookie_dir = templates[template.lower()]
+
+        if cookie_directory:
+            cookie_dir = cookie_directory
+        if not cookie_dir:
+            cookie_dir = template.lower()
+
+        cookiecutter.main.cookiecutter(
+            selected_template,
+            extra_context={
+                "author_name": os.getlogin(),
+                "project_name": project_dir,
+                "cellpy_version": cellpy_version,
+                "session_id": session_id,
+            },
+            no_input=no_input,
+            directory=cookie_dir,
+        )
+    except cookiecutter.exceptions.OutputDirExistsException as e:
+        click.echo("Sorry. This did not work as expected!")
+        click.echo(" - cookiecutter refused to create the project")
+        click.echo(e)
+
+    if serve_:
+        os.chdir(directory)
+        _serve(server)
+
+    if run_:
+        try:
+            import papermill as pm
+        except ImportError:
+            click.echo(
+                "[cellpy]: You need to install papermill for automatically execute the notebooks."
+            )
+            click.echo("[cellpy]: You can install it using pip like this:")
+            click.echo(" >> pip install papermill")
+            return
+        new_existing_projects = os.listdir(selected_project_dir)
+        our_new_projects = list(set(new_existing_projects) - set(existing_projects))
+
+        if not len(our_new_projects):
+            click.echo(
+                "[cellpy]: Sorry, could not deiced what is the new project "
+                "- so I don't dare to try to execute automatically."
+            )
+            return
+        our_new_project = selected_project_dir / our_new_projects[0]
+
+        _run_project(our_new_project)
+
+
+def _serve(server):
+    click.echo(f"serving with jupyter {server}")
+    subprocess.run(["jupyter", server], check=True)
+    click.echo("Finished serving.")
+
+
+# ----------------------- serve ---------------------------------------
+@click.command()
+@click.option("--lab", "-l", is_flag=True, help="Use Jupyter Lab instead of Notebook")
+@click.option("--directory", "-d", default=None, help="Start in custom directory DIR")
+def serve(lab, directory):
+    """Start a Jupyter server."""
+
+    from cellpy.parameters import prms
+
+    if directory is None:
+        directory = prms.Paths.notebookdir
+    elif directory == "home":
+        directory = Path().home()
+    elif directory == "here":
+        directory = Path(os.getcwd())
+
+    if not os.path.isdir(directory):
+        click.echo("Sorry. This did not work as expected!")
+        click.echo(f" - {directory} does not exist")
+        return
+
+    if lab:
+        server = "lab"
+    else:
+        server = "notebook"
+
+    os.chdir(directory)
+    _serve(server)
+
+
+cli.add_command(setup)
+cli.add_command(info)
+cli.add_command(edit)
+cli.add_command(pull)
+cli.add_command(run)
+cli.add_command(new)
+cli.add_command(serve)
+
+
+# tests etc
+def _main_pull():
+    if sys.platform == "win32":
+        rootpath = pathlib.Path(r"C:\Temp\cellpy_user")
+    else:
+        rootpath = pathlib.Path("/Users/jepe/scripting/tmp/cellpy_test_user")
+    _pull_examples(rootpath, pw="env")
+    _pull_tests(rootpath, pw="env")
+    # _pull(gdirpath="examples", rootpath=rootpath, u="ask", pw="ask")
+    # _pull(gdirpath="tests", rootpath=rootpath, u="ask", pw="ask")
+    # _pull(gdirpath="testdata", rootpath=rootpath, u="ask", pw="ask")
+
+
+def _main():
+    file_name = prmreader.create_custom_init_filename()
+    click.echo(file_name)
+    user_directory, destination_file_name = prmreader.get_user_dir_and_dst(file_name)
+    click.echo(user_directory)
+    click.echo(destination_file_name)
+    click.echo("trying to save it")
+    save_prm_file(destination_file_name + "_dummy")
+
+    click.echo(" Testing setup ".center(80, "="))
+    setup(["--interactive", "--reset"])
+
+
+def _cli_setup_interactive():
+    from click.testing import CliRunner
+
+    if sys.platform == "win32":
+        root_dir = r"C:\Temp\cellpy_user"
+    else:
+        root_dir = "/Users/jepe/scripting/tmp/cellpy_test_user"
+    testuser = "tester"
+    init_filename = prmreader.create_custom_init_filename(testuser)
+    dst_file = get_dst_file(root_dir, init_filename)
+    init_file = pathlib.Path(dst_file)
+    opts = list()
+    opts.append("setup")
+    opts.append("-i")
+    # opts.append("-nr")
+    opts.append("-r")
+    opts.extend(["-d", root_dir])
+    opts.extend(["-t", testuser])
+
+    input_str = "\n"  # out
+    input_str += "\n"  # rawdatadir
+    input_str += "\n"  # cellpyfiles
+    input_str += "\n"  # log
+    input_str += "\n"  # examples
+    input_str += "\n"  # dbfolder
+    input_str += "\n"  # dbfile
+    runner = CliRunner()
+    result = runner.invoke(cli, opts, input=input_str)
+
+    click.echo(" out ".center(80, "."))
+    click.echo(result.output)
+    from pprint import pprint
+
+    pprint(prmreader.prms.Paths)
+    click.echo(" conf-file ".center(80, "."))
+    click.echo(init_file)
+    click.echo()
+    with init_file.open() as f:
+        for line in f.readlines():
+            click.echo(line.strip())
+
+
+def check_it(var=None):
+    import pathlib
+    import sys
+
+    p_env = pathlib.Path(sys.prefix)
+    print(p_env.name)
+    new(list_=True)
+
+
+if __name__ == "__main__":
+    u1 = os.getlogin()
+    u2 = os.path.expanduser("~")
+    u3 = os.environ.get("USERNAME")
+
+    print(u1)
+    print(u2)
+    print(u3)
+    # check_it()
+    # click.echo("\n\n", " RUNNING MAIN PULL ".center(80, "*"), "\n")
+    # _main_pull()
+    # click.echo("ok")
```

### Comparing `cellpy-1.0.0a0/cellpy/exceptions.py` & `cellpy-1.0.0a3/cellpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/cellpy/internals/core.py` & `cellpy-1.0.0a3/cellpy/internals/core.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,618 +1,687 @@
-"""This module contains div classes etc that are not really connected to cellpy."""
-
-from dataclasses import dataclass
-import fnmatch
-import logging
-import os
-import pathlib
-import shutil
-import stat
-import tempfile
-import time
-import warnings
-from typing import (
-    Any,
-    Tuple,
-    Dict,
-    List,
-    Union,
-    TypeVar,
-    Generator,
-    Optional,
-    Iterable,
-    Callable,
-    Type,
-    cast,
-)
-
-import fabric
-
-from cellpy.exceptions import UnderDefined
-
-S = TypeVar("S", bound="OtherPath")
-URI_PREFIXES = ["ssh:", "sftp:", "scp:", "http:", "https:", "ftp:", "ftps:", "smb:"]
-IMPLEMENTED_PROTOCOLS = ["ssh:", "sftp:", "scp:"]
-# name of environment variable that holds the key file and password:
-ENV_VAR_CELLPY_KEY_FILENAME = "CELLPY_KEY_FILENAME"
-ENV_VAR_CELLPY_PASSWORD = "CELLPY_PASSWORD"
-
-
-@dataclass
-class ExternalStatResult:
-    """Mock of os.stat_result."""
-
-    # st_mode: int = 0
-    # st_ino: int = 0
-    # st_dev: int = 0
-    # st_nlink: int = 0
-    # st_uid: int = 0
-    # st_gid: int = 0
-    st_size: int = 0
-    st_mtime: int = 0
-    st_atime: int = 0
-    st_ctime: Optional[int] = None
-
-
-def _clean_up_original_path_string(path_string):
-    logging.debug(f"cleaning up path: {path_string}")
-    if not isinstance(path_string, str):
-        logging.debug(f"path is not a string: {path_string}")
-        logging.debug(f"path is of type: {type(path_string)}")
-
-        if isinstance(path_string, OtherPath):
-            logging.debug(f"path is an OtherPath object")
-            if hasattr(path_string, "original"):
-                logging.debug(f"path has an original attribute")
-                path_string = path_string.original
-            else:
-                logging.debug(f"path does not have an original attribute")
-                path_string = str(path_string)
-
-        elif isinstance(path_string, pathlib.PosixPath):
-            path_string = "/".join(path_string.parts)
-        elif isinstance(path_string, pathlib.WindowsPath):
-            parts = list(path_string.parts)
-            if not parts:
-                parts = [""]
-            parts[0] = parts[0].replace("\\", "")
-            path_string = "/".join(parts)
-        else:
-            path_string = str(path_string)
-    else:
-        logging.debug(f"path is a string: {path_string}")
-    return path_string
-
-
-def _check_external(path_string: str) -> Tuple[str, bool, str, str]:
-    # path_sep = "\\" if os.name == "nt" else "/"
-    _is_external = False
-    _location = ""
-    _uri_prefix = ""
-    for prefix in URI_PREFIXES:
-        if path_string.startswith(prefix):
-            path_string = path_string.replace(prefix, "")
-            path_string = path_string.lstrip("/")
-            _is_external = True
-            _uri_prefix = prefix + "//"
-            _location, *rest = path_string.split("/")
-            path_string = "/" + "/".join(rest)
-            break
-    path_string = path_string or "."
-    # fix for windows paths:
-    path_string = path_string.replace("\\", "/")
-    # fix for posix paths:
-    path_string = path_string.replace("//", "/")
-    return path_string, _is_external, _uri_prefix, _location
-
-
-class OtherPath(pathlib.Path):
-    """A pathlib.Path subclass that can handle external paths.
-
-    Additional attributes:
-        is_external (bool): is True if the path is external.
-        location (str): the location of the external path (e.g. a server name).
-        uri_prefix (str): the prefix of the external path (e.g. scp:// or sftp://).
-        raw_path (str): the path without any uri_prefix or location.
-        original (str): the original path string.
-        full_path (str): the full path (including uri_prefix and location).
-    Additional methods:
-        copy (method): a method for copying the file to a local path.
-    Overrides (only if is_external is True):
-        glob (method): a method for globbing external paths.
-        rglob (method): a method for 'recursive' globbing external paths (max one extra level deep).
-    """
-
-    _flavour = (
-        pathlib._windows_flavour if os.name == "nt" else pathlib._posix_flavour
-    )  # noqa
-
-    def __new__(cls, *args, **kwargs):
-        logging.debug("Running __new__ for OtherPath")
-        logging.debug(f"args: {args}")
-        logging.debug(f"kwargs: {kwargs}")
-        if args:
-            path, *args = args
-        else:
-            path = "."
-            logging.debug("initiating OtherPath without any arguments")
-        if not path:
-            logging.debug("initiating OtherPath with empty path")
-            path = "."
-        logging.debug(f"path: {path}")
-        if isinstance(path, OtherPath) and hasattr(path, "_original"):
-            logging.debug(f"path is OtherPath")
-            path = path._original
-        logging.debug(f"checked if path is OtherPath")
-        path = _clean_up_original_path_string(path)
-        cls.__original = path
-        cls._pathlib_doc = super().__doc__
-        path = _check_external(path)[0]
-        return super().__new__(cls, path, *args, **kwargs)
-
-    def __init__(self, *args, **kwargs):
-        logging.debug("Running __init__ for OtherPath")
-        _path_string, *args = args
-        if not _path_string:
-            path_string = "."
-        else:
-            path_string = self.__original
-        self._original = self.__original
-        self._check_external(path_string)
-        # pathlib.PurePath and Path for Python 3.12 seems to have an __init__ method
-        # where it sets self._raw_path from the input argument, but this is not the case
-        # for Python 3.11, 10, and 9. Those do not have their own __init__ method (and
-        # does not have a self._raw_path attribute).
-        # Instead of running e.g. super().__init__(self._raw_other_path) we do this
-        # instead (which is what the __init__ method does in Python 3.12):
-        self._raw_path = self._raw_other_path
-        self.__doc__ += f"\nOriginal documentation:\n\n{self._pathlib_doc}"
-        self._wrap_methods()  # dynamically wrapping methods - should gradually be replaced by hard-coded methods.
-
-    def _wrap_methods(self):
-        logging.debug("Running _wrap_methods for OtherPath")
-        existing_methods = self.__class__.__dict__.keys()
-        parent_methods_that_works_also_on_external_paths = []  # "parents", "parts"
-        parent_methods_that_returns_other_paths = []
-
-        for m in sorted(dir(pathlib.Path)):
-            if m.startswith("_"):
-                continue
-            if (
-                m in existing_methods
-                or m in parent_methods_that_works_also_on_external_paths
-            ):
-                continue
-            method = getattr(pathlib.Path, m)
-            if m in parent_methods_that_returns_other_paths:
-                setattr(self.__class__, m, self._wrap_and_morph_method(method))
-            if callable(method):
-                setattr(self.__class__, m, self._wrap_callable_method(method))
-            else:
-                setattr(self.__class__, m, self._wrap_non_callable(method))
-
-    def _wrap_and_morph_method(self, method):
-        if self.is_external:
-            print(f"Cannot run {method.__name__} for external paths!")
-            return lambda *args, **kwargs: self
-        else:
-            return lambda *args, **kwargs: OtherPath(*args, **kwargs)
-
-    def _wrap_callable_method(self, method, default_return_value=True):
-        if self.is_external:
-            print(f"Cannot run {method.__name__} for external paths!")
-            return lambda *args, **kwargs: default_return_value
-        else:
-            return method
-
-    def _wrap_non_callable(self, attr, default_return_value=None):
-        if self.is_external:
-            print(f"Cannot get {attr} for external paths!")
-            return default_return_value
-        else:
-            return attr
-
-    def _check_external(self, path_string):
-        logging.debug("Running _check_external for OtherPath")
-        (
-            path_string,
-            self._is_external,
-            self._uri_prefix,
-            self._location,
-        ) = _check_external(path_string)
-        logging.debug(f"self._is_external: {self._is_external}")
-        logging.debug(f"self._uri_prefix: {self._uri_prefix}")
-        logging.debug(f"self._location: {self._location}")
-        logging.debug(f"path_string: {path_string}")
-        self._raw_other_path = path_string
-
-    def __div__(self, other: Union[str, S]) -> S:
-        if self.is_external:
-            path = self._original + "/" + other
-            return OtherPath(path)
-        path = pathlib.Path(self._original).__truediv__(other)
-        return OtherPath(path)
-
-    def __truediv__(self, other: Union[str, S]) -> S:
-        if self.is_external:
-            path = self._original + "/" + other
-            return OtherPath(path)
-        path = pathlib.Path(self._original).__truediv__(other)
-        return OtherPath(path)
-
-    def __rtruediv__(self: S, key: Union[str, S]) -> S:
-        if self.is_external:
-            raise TypeError(f"Cannot use rtruediv on external paths.")
-        path = pathlib.Path(self._original).__rtruediv__(key)
-        return OtherPath(path)
-
-    def __str__(self: S) -> str:
-        if hasattr(self, "_original") and self.is_external:
-            return self._original
-        else:
-            return super().__str__()
-
-    def _glob(self, glob_str: str, **kwargs) -> Generator:
-        testing = kwargs.pop("testing", False)
-        search_in_sub_dirs = kwargs.pop("search_in_sub_dirs", False)
-        if self.is_external:
-            connect_kwargs, host = self._get_connection_info(testing)
-            paths = self._glob_with_fabric(
-                host, connect_kwargs, glob_str, search_in_sub_dirs=search_in_sub_dirs
-            )
-            return (OtherPath(f"{self._original.rstrip('/')}/{p}") for p in paths)
-        paths = pathlib.Path(self._original).glob(glob_str)
-        return (OtherPath(p) for p in paths)
-
-    def glob(self, glob_str: str, *args, **kwargs) -> Generator:
-        return self._glob(glob_str, search_in_sub_dirs=False, **kwargs)
-
-    def rglob(self, glob_str: str, *args, **kwargs) -> Generator:
-        return self._glob(glob_str, search_in_sub_dirs=True, **kwargs)
-
-    def resolve(self: S, *args, **kwargs) -> S:
-        if self.is_external:
-            # logging.warning(f"Cannot resolve external paths. Returning self. ({self})")
-            return self
-        resolved_path = pathlib.Path(self._original).resolve(*args, **kwargs)
-        return OtherPath(resolved_path)
-
-    def is_dir(self: S, *args, **kwargs) -> bool:
-        """Check if path is a directory."""
-        if self.is_external:
-            logging.warning(
-                f"Cannot check if dir exists for external paths! Assuming it exists."
-            )
-            return True
-        return super().is_dir()
-
-    def is_file(self: S, *args, **kwargs) -> bool:
-        """Check if path is a file."""
-        if self.is_external:
-            logging.warning(
-                f"Cannot check if file exists for external paths! Assuming it exists."
-            )
-            return True
-        return super().is_file()
-
-    def exists(self: S, *args, **kwargs) -> bool:
-        """Check if path exists."""
-        if self.is_external:
-            logging.warning(
-                f"Cannot check if path exists for external paths! Assuming it exists."
-            )
-            return True
-        return super().exists()
-
-    @property
-    def parent(self: S) -> S:
-        """Return the parent directory of the path."""
-        if self.is_external:
-            return OtherPath(self._original.rsplit("/", 1)[0])
-        return OtherPath(super().parent)
-
-    @property
-    def name(self: S):
-        """Return the parent directory of the path."""
-        return super().name
-
-    @property
-    def suffix(self) -> str:
-        """Return the suffix of the path."""
-        return super().suffix
-
-    @property
-    def suffixes(self) -> List[str]:
-        """Return the suffixes of the path."""
-        return super().suffixes
-
-    @property
-    def stem(self) -> str:
-        """Return the stem of the path."""
-        return super().stem
-
-    def with_suffix(self: S, suffix: str) -> S:
-        """Return a new path with the suffix changed."""
-        if self.is_external:
-            logging.warning(
-                "This is method (`with_suffix`) not tested for external paths!"
-            )
-            return OtherPath(self._original.rsplit(".", 1)[0] + suffix)
-        return OtherPath(super().with_suffix(suffix))
-
-    def with_name(self: S, name: str) -> S:
-        """Return a new path with the name changed."""
-        if self.is_external:
-            logging.warning(
-                "This method (`with_name`) is not tested for external paths!"
-            )
-            return OtherPath(self._original.rsplit("/", 1)[0] + "/" + name)
-        return OtherPath(super().with_name(name))
-
-    def with_stem(self: S, stem: str) -> S:
-        """Return a new path with the stem changed."""
-        if self.is_external:
-            logging.warning(
-                "This method (`with_stem`) is not tested for external paths!"
-            )
-            return OtherPath(self._original.rsplit("/", 1)[0] + "/" + stem)
-        return OtherPath(super().with_stem(stem))
-
-    def absolute(self: S) -> S:
-        if self.is_external:
-            logging.warning(
-                "This method (`absolute`) is not implemented yet for external paths! Returning self."
-            )
-            return self
-        return OtherPath(super().absolute())
-
-    def samefile(self: S, other_path: Union[str, pathlib.Path, S]) -> bool:
-        if self.is_external:
-            logging.warning(
-                "This method (`absolute`) is not implemented yet for external paths! Returning True."
-            )
-            return True
-        return super().samefile(other_path)
-
-    def iterdir(self, *args, **kwargs):
-        if self.is_external:
-            logging.warning(
-                f"Cannot run `iterdir` yet for external paths! Returning None."
-            )
-            return
-        else:
-            return (OtherPath(p) for p in super().iterdir())
-
-    @property
-    def parents(self, *args, **kwargs):
-        if self.is_external:
-            logging.warning(
-                f"Cannot run `parents` yet for external paths! Returning None."
-            )
-            return
-        return super().parents
-
-    def stat(self, *args, **kwargs):
-        testing = kwargs.pop("testing", False)
-        if self.is_external:
-            # logging.warning(f"Cannot run `stat` for external paths! Returning stat_result object with only zeros.")
-            try:
-                connect_kwargs, host = self._get_connection_info(testing)
-            except UnderDefined as e:
-                logging.debug(f"UnderDefined error: {e}")
-                logging.debug("Returning stat_result object with only zeros.")
-                return ExternalStatResult()
-            try:
-                return self._stat_with_fabric(host, connect_kwargs)
-            except FileNotFoundError:
-                logging.debug(
-                    "File not found! Returning stat_result object with only zeros."
-                )
-                return ExternalStatResult()
-
-        return super().stat()
-
-    def joinpath(self, *args, **kwargs):
-        logging.warning(f"Cannot run 'joinpath' for OtherPath!")
-        return self
-
-    def readlink(self, *args, **kwargs):
-        logging.warning(f"Cannot run 'readlink' for OtherPath!")
-        return
-
-    def match(self, *args, **kwargs):
-        logging.warning(f"Cannot run 'match' for OtherPath!")
-        return
-
-    def cwd(self):
-        logging.warning(f"Cannot run 'match' for OtherPath!")
-        return
-
-    def group(self):
-        logging.warning(f"Cannot run 'group' for OtherPath!")
-        return
-
-    @property
-    def owner(self, *args, **kwargs):
-        logging.warning(f"Cannot get 'owner' for OtherPath!")
-        return
-
-    def lchmod(self, *args, **kwargs):
-        logging.warning(f"Cannot run 'lchmod' for OtherPath!")
-        return self
-
-    @property
-    def original(self: S) -> str:
-        return self._original
-
-    @property
-    def raw_path(self: S) -> str:
-        # this will return a leading slash for some edge cases
-        return self._raw_other_path
-
-    @property
-    def full_path(self: S) -> str:
-        if self.is_external:
-            return f"{self._uri_prefix}{self._location}{self._raw_other_path}"
-        return self._original
-
-    @property
-    def is_external(self: S) -> bool:
-        if not hasattr(self, "_is_external"):
-            logging.warning("OBS! OtherPath object missing _is_external attribute!")
-            logging.warning("This should not happen. Please report this bug!")
-            logging.warning(
-                "(most likely means that pathlib.Path has changed and that it now has "
-                "another attribute or method that returns a new pathlib.Path object or "
-                "that you have used a method that is not supported yet)"
-            )
-            # return False
-        return self._is_external
-
-    @property
-    def uri_prefix(self) -> str:
-        """Return the uri prefix for the external path (e.g ``ssh://``)."""
-        return self._uri_prefix
-
-    @property
-    def location(self) -> str:
-        """Return the location of the external path (e.g ``user@server.com``)."""
-        return self._location
-
-    def as_uri(self) -> str:
-        """Return the path as a uri (e.g. ``scp://user@server.com/home/data/my_file.txt``)."""
-        if self._is_external:
-            return f"{self._uri_prefix}{self._location}/{'/'.join(list(super().parts)[1:])}"
-        return super().as_uri()
-
-    def copy(
-        self, destination: Optional[pathlib.Path] = None, testing=False
-    ) -> pathlib.Path:
-        """Copy the file to a destination."""
-        if destination is None:
-            destination = pathlib.Path(tempfile.gettempdir())
-        else:
-            destination = pathlib.Path(destination)
-        print(80 * "=")
-        print(f"Copying {self} to {destination}...")
-        print(f"Is external: {self.is_external}")
-        print(f"URI prefix: {self.uri_prefix}")
-        print(f"Location: {self.location}")
-        print(f"Raw path: {self.raw_path}")
-        print(f"Full path: {self.full_path}")
-        print(f"Original: {self.original}")
-        print(f"Is absolute: {self.is_absolute()}")
-        print(f"{self.name=}")
-        print(80 * "=")
-        path_of_copied_file = destination / self.name
-
-        if not self.is_external:
-            shutil.copy2(self, destination)
-        else:
-            connect_kwargs, host = self._get_connection_info(testing)
-            self._copy_with_fabric(host, connect_kwargs, destination)
-
-        return path_of_copied_file
-
-    def _get_connection_info(self, testing: bool = False) -> Tuple[Dict, str]:
-        host = self.location
-        uri_prefix = self.uri_prefix.replace("//", "")
-        if uri_prefix not in URI_PREFIXES:
-            raise ValueError(f"uri_prefix {uri_prefix} not recognized")
-        if uri_prefix not in IMPLEMENTED_PROTOCOLS:
-            raise ValueError(
-                f"uri_prefix {uri_prefix.replace(':', '')} not implemented yet"
-            )
-        password = os.getenv(ENV_VAR_CELLPY_PASSWORD, None)
-        key_filename = os.getenv(ENV_VAR_CELLPY_KEY_FILENAME, None)
-        if password is None and key_filename is None:
-            raise UnderDefined(
-                f"You must define either {ENV_VAR_CELLPY_PASSWORD} "
-                f"or {ENV_VAR_CELLPY_KEY_FILENAME} environment variables."
-            )
-        if key_filename is not None:
-            connect_kwargs = {"key_filename": key_filename}
-            logging.debug(f"got key_filename")
-            if not testing:
-                if not pathlib.Path(key_filename).is_file():
-                    raise FileNotFoundError(f"Could not find key file {key_filename}")
-        else:
-            connect_kwargs = {"password": password}
-        return connect_kwargs, host
-
-    def _copy_with_fabric(
-        self, host: str, connect_kwargs: dict, destination: Union[str, S, pathlib.Path]
-    ):
-        with fabric.Connection(host, connect_kwargs=connect_kwargs) as conn:
-            try:
-                t1 = time.time()
-                conn.get(self.raw_path, str(destination / self.name))
-                logging.debug(f"copying took {time.time() - t1:.2f} seconds")
-            except FileNotFoundError as e:
-                raise FileNotFoundError(
-                    f"Could not find file {self.raw_path} on {host}"
-                ) from e
-
-    def _stat_with_fabric(self, host: str, connect_kwargs: dict) -> ExternalStatResult:
-        with fabric.Connection(host, connect_kwargs=connect_kwargs) as conn:
-            try:
-                t1 = time.time()
-                sftp_conn = conn.sftp()
-                stat_result = sftp_conn.stat(self.raw_path)
-                logging.debug(f"stat took {time.time() - t1:.2f} seconds")
-                return ExternalStatResult(
-                    st_size=stat_result.st_size,
-                    st_atime=stat_result.st_atime,
-                    st_mtime=stat_result.st_mtime,
-                )
-            except FileNotFoundError as e:
-                raise FileNotFoundError(
-                    f"Could not find file {self.raw_path} on {host}"
-                ) from e
-
-    def _glob_with_fabric(
-        self: S,
-        host: str,
-        connect_kwargs: dict,
-        glob_str: str,
-        search_in_sub_dirs: bool = False,
-    ) -> List[str]:
-        path_separator = "/"
-        with fabric.Connection(host, connect_kwargs=connect_kwargs) as conn:
-            try:
-                t1 = time.time()
-                sftp_conn = conn.sftp()
-                sftp_conn.chdir(self.raw_path)
-                if search_in_sub_dirs:  # recursive globbing one level down
-                    sub_dirs = [
-                        f
-                        for f in sftp_conn.listdir()
-                        if stat.S_ISDIR(sftp_conn.stat(f).st_mode)
-                    ]
-                    files = [
-                        f
-                        for f in sftp_conn.listdir()
-                        if not stat.S_ISDIR(sftp_conn.stat(f).st_mode)
-                    ]
-                    filtered_files = fnmatch.filter(files, glob_str)
-                    for sub_dir in sub_dirs:
-                        sftp_conn.chdir(sub_dir)
-                        new_files = [
-                            f
-                            for f in sftp_conn.listdir()
-                            if not stat.S_ISDIR(sftp_conn.stat(f).st_mode)
-                        ]
-                        new_filtered_files = fnmatch.filter(new_files, glob_str)
-                        new_filtered_files = [
-                            f"{sub_dir}{path_separator}{f}" for f in new_filtered_files
-                        ]
-                        filtered_files += new_filtered_files
-                        sftp_conn.chdir("..")
-                else:
-                    files = sftp_conn.listdir()
-                    filtered_files = fnmatch.filter(files, glob_str)
-                logging.debug(f"globbing took {time.time() - t1:.2f} seconds")
-                return filtered_files
-            except FileNotFoundError as e:
-                raise FileNotFoundError(
-                    f"Could not find file {self.raw_path} on {host}"
-                ) from e
+"""This module contains div classes etc that are not really connected to cellpy."""
+
+from dataclasses import dataclass
+import fnmatch
+import logging
+import os
+import pathlib
+import shutil
+import stat
+import tempfile
+import time
+import warnings
+from typing import (
+    Any,
+    Tuple,
+    Dict,
+    List,
+    Union,
+    TypeVar,
+    Generator,
+    Optional,
+    Iterable,
+    Callable,
+    Type,
+    cast,
+)
+
+import fabric
+
+from cellpy.exceptions import UnderDefined
+
+S = TypeVar("S", bound="OtherPath")
+URI_PREFIXES = ["ssh:", "sftp:", "scp:", "http:", "https:", "ftp:", "ftps:", "smb:"]
+IMPLEMENTED_PROTOCOLS = ["ssh:", "sftp:", "scp:"]
+# name of environment variable that holds the key file and password:
+ENV_VAR_CELLPY_KEY_FILENAME = "CELLPY_KEY_FILENAME"
+ENV_VAR_CELLPY_PASSWORD = "CELLPY_PASSWORD"
+
+
+@dataclass
+class ExternalStatResult:
+    """Mock of os.stat_result."""
+
+    # st_mode: int = 0
+    # st_ino: int = 0
+    # st_dev: int = 0
+    # st_nlink: int = 0
+    # st_uid: int = 0
+    # st_gid: int = 0
+    st_size: int = 0
+    st_mtime: int = 0
+    st_atime: int = 0
+    st_ctime: Optional[int] = None
+
+
+def _clean_up_original_path_string(path_string):
+    if not isinstance(path_string, str):
+        if isinstance(path_string, OtherPath):
+            logging.debug(f"path is an OtherPath object")
+            if hasattr(path_string, "original"):
+                logging.debug(f"path has an original attribute")
+                path_string = path_string.original
+            else:
+                logging.debug(f"path does not have an original attribute")
+                path_string = str(path_string)
+
+        elif isinstance(path_string, pathlib.PosixPath):
+            path_string = "/".join(path_string.parts)
+        elif isinstance(path_string, pathlib.WindowsPath):
+            parts = list(path_string.parts)
+            if not parts:
+                parts = [""]
+            parts[0] = parts[0].replace("\\", "")
+            path_string = "/".join(parts)
+        else:
+            logging.debug(f"unknown path type: {type(path_string)}")
+            path_string = str(path_string)
+    return path_string
+
+
+def _check_external(path_string: str) -> Tuple[str, bool, str, str]:
+    # path_sep = "\\" if os.name == "nt" else "/"
+    _is_external = False
+    _location = ""
+    _uri_prefix = ""
+    for prefix in URI_PREFIXES:
+        if path_string.startswith(prefix):
+            path_string = path_string.replace(prefix, "")
+            path_string = path_string.lstrip("/")
+            _is_external = True
+            _uri_prefix = prefix + "//"
+            _location, *rest = path_string.split("/")
+            path_string = "/" + "/".join(rest)
+            break
+    path_string = path_string or "."
+    # fix for windows paths:
+    path_string = path_string.replace("\\", "/")
+    # fix for posix paths:
+    path_string = path_string.replace("//", "/")
+    return path_string, _is_external, _uri_prefix, _location
+
+
+class OtherPath(pathlib.Path):
+    """A pathlib.Path subclass that can handle external paths.
+
+    Additional attributes:
+        is_external (bool): is True if the path is external.
+        location (str): the location of the external path (e.g. a server name).
+        uri_prefix (str): the prefix of the external path (e.g. scp:// or sftp://).
+        raw_path (str): the path without any uri_prefix or location.
+        original (str): the original path string.
+        full_path (str): the full path (including uri_prefix and location).
+    Additional methods:
+        copy (method): a method for copying the file to a local path.
+    Overrides (only if is_external is True):
+        glob (method): a method for globbing external paths.
+        rglob (method): a method for 'recursive' globbing external paths (max one extra level deep).
+    """
+
+    _flavour = (
+        pathlib._windows_flavour if os.name == "nt" else pathlib._posix_flavour
+    )  # noqa
+
+    def __new__(cls, *args, **kwargs):
+        if args:
+            path, *args = args
+        else:
+            path = "."
+            logging.debug("initiating OtherPath without any arguments")
+        if not path:
+            logging.debug("initiating OtherPath with empty path")
+            path = "."
+        if isinstance(path, OtherPath) and hasattr(path, "_original"):
+            logging.debug(f"path is OtherPath")
+            path = path._original
+        logging.debug(f"checked if path is OtherPath")
+
+        path = _clean_up_original_path_string(path)
+        assert isinstance(path, str), "path must be a string"
+        cls.__original = path
+        cls._pathlib_doc = super().__doc__
+        path = _check_external(path)[0]
+        return super().__new__(cls, path, *args, **kwargs)
+
+    def __init__(self, *args, **kwargs):
+        logging.debug("Running __init__ for OtherPath")
+        _path_string, *args = args
+        if not _path_string:
+            path_string = "."
+        else:
+            path_string = self.__original
+        self._original = self.__original
+        self._check_external(path_string)
+        # pathlib.PurePath and Path for Python 3.12 seems to have an __init__ method
+        # where it sets self._raw_path from the input argument, but this is not the case
+        # for Python 3.11, 10, and 9. Those do not have their own __init__ method (and
+        # does not have a self._raw_path attribute).
+        # Instead of running e.g. super().__init__(self._raw_other_path) we do this
+        # instead (which is what the __init__ method does in Python 3.12):
+        self._raw_path = self._raw_other_path
+        self.__doc__ += f"\nOriginal documentation:\n\n{self._pathlib_doc}"
+        self._wrap_methods()  # dynamically wrapping methods - should gradually be replaced by hard-coded methods.
+
+    def _wrap_methods(self):
+        logging.debug("Running _wrap_methods for OtherPath")
+        existing_methods = self.__class__.__dict__.keys()
+        parent_methods_that_works_also_on_external_paths = []  # "parents", "parts"
+        parent_methods_that_returns_other_paths = []
+
+        for m in sorted(dir(pathlib.Path)):
+            if m.startswith("_"):
+                continue
+            if (
+                m in existing_methods
+                or m in parent_methods_that_works_also_on_external_paths
+            ):
+                continue
+            method = getattr(pathlib.Path, m)
+            if m in parent_methods_that_returns_other_paths:
+                setattr(self.__class__, m, self._wrap_and_morph_method(method))
+            if callable(method):
+                setattr(self.__class__, m, self._wrap_callable_method(method))
+            else:
+                setattr(self.__class__, m, self._wrap_non_callable(method))
+
+    def _wrap_and_morph_method(self, method):
+        if self.is_external:
+            return lambda *args, **kwargs: self
+        else:
+            return lambda *args, **kwargs: OtherPath(*args, **kwargs)
+
+    def _wrap_callable_method(self, method, default_return_value=True):
+        if self.is_external:
+            return lambda *args, **kwargs: default_return_value
+        else:
+            return method
+
+    def _wrap_non_callable(self, attr, default_return_value=None):
+        if self.is_external:
+            return default_return_value
+        else:
+            return attr
+
+    def _check_external(self, path_string):
+        logging.debug("Running _check_external for OtherPath")
+        (
+            path_string,
+            self._is_external,
+            self._uri_prefix,
+            self._location,
+        ) = _check_external(path_string)
+        logging.debug(f"self._is_external: {self._is_external}")
+        logging.debug(f"self._uri_prefix: {self._uri_prefix}")
+        logging.debug(f"self._location: {self._location}")
+        logging.debug(f"path_string: {path_string}")
+        self._raw_other_path = path_string
+
+    def __div__(self, other: Union[str, S]) -> S:
+        if self.is_external:
+            path = f"{self._original}/{other}"
+            return OtherPath(path)
+        path = pathlib.Path(self._original).__truediv__(other)
+        return OtherPath(path)
+
+    def __truediv__(self, other: Union[str, S]) -> S:
+        if self.is_external:
+            path = f"{self._original}/{other}"
+            return OtherPath(path)
+        path = pathlib.Path(self._original).__truediv__(other)
+        return OtherPath(path)
+
+    def __rtruediv__(self: S, key: Union[str, S]) -> S:
+        if self.is_external:
+            raise TypeError(f"Cannot use rtruediv on external paths.")
+        path = pathlib.Path(self._original).__rtruediv__(key)
+        return OtherPath(path)
+
+    def __str__(self: S) -> str:
+        if hasattr(self, "_original") and self.is_external:
+            logging.debug("external path, returning _original")
+            return self._original
+        return super().__str__()
+
+    def __repr__(self: S) -> str:
+        if hasattr(self, "_original"):
+            if self.is_external:
+                logging.debug("external path, returning _original")
+            return f"OtherPath('{self._original}')"
+        else:
+            return super().__repr__()
+
+    def _glob(self, glob_str: str, **kwargs) -> Generator:
+        testing = kwargs.pop("testing", False)
+        search_in_sub_dirs = kwargs.pop("search_in_sub_dirs", False)
+        if self.is_external:
+            connect_kwargs, host = self._get_connection_info(testing)
+            paths = self._glob_with_fabric(
+                host, connect_kwargs, glob_str, search_in_sub_dirs=search_in_sub_dirs
+            )
+            return (OtherPath(f"{self._original.rstrip('/')}/{p}") for p in paths)
+        paths = pathlib.Path(self._original).glob(glob_str)
+        return (OtherPath(p) for p in paths)
+
+    def glob(self, glob_str: str, *args, **kwargs) -> Generator:
+        return self._glob(glob_str, search_in_sub_dirs=False, **kwargs)
+
+    def rglob(self, glob_str: str, *args, **kwargs) -> Generator:
+        return self._glob(glob_str, search_in_sub_dirs=True, **kwargs)
+
+    def _listdir(self, levels: int, **kwargs) -> Generator:
+        if self.is_external:
+            testing = kwargs.pop("testing", False)
+            connect_kwargs, host = self._get_connection_info(testing)
+            paths = self._listdir_with_fabric(host, connect_kwargs, levels)
+            return (OtherPath(p) for p in paths)
+
+        if self.is_dir():
+            return (OtherPath(f"{self.full_path}/{p}") for p in os.listdir(self._original))
+
+    def listdir(self: S, levels: int = 1, **kwargs) -> Generator:
+        """List the contents of the directory.
+
+        Args:
+            levels (int, optional): How many sublevels to list. Defaults to 1.
+                If you want to list all sublevels, use `listdir(levels=-1)`.
+                If you want to list only the current level (no subdirectories),
+                use `listdir(levels=0)`.
+
+        Returns:
+            Generator: Generator of OtherPath objects.
+
+        """
+        return self._listdir(levels, **kwargs)
+
+    def resolve(self: S, *args, **kwargs) -> S:
+        """Resolve the path."""
+        if self.is_external:
+            logging.debug(f"Cannot resolve external paths. Returning self. ({self})")
+            return OtherPath(self._original)
+        resolved_path = pathlib.Path(self._original).resolve(*args, **kwargs)
+        return OtherPath(resolved_path)
+
+    def is_dir(self: S, *args, **kwargs) -> bool:
+        """Check if path is a directory."""
+        if self.is_external:
+            logging.warning(
+                f"Cannot check if dir exists for external paths! Assuming it exists."
+            )
+            return True
+        return super().is_dir()
+
+    def is_file(self: S, *args, **kwargs) -> bool:
+        """Check if path is a file."""
+        if self.is_external:
+            logging.warning(
+                f"Cannot check if file exists for external paths! Assuming it exists."
+            )
+            return True
+        return super().is_file()
+
+    def exists(self: S, *args, **kwargs) -> bool:
+        """Check if path exists."""
+        if self.is_external:
+            logging.warning(
+                f"Cannot check if path exists for external paths! Assuming it exists."
+            )
+            return True
+        return super().exists()
+
+    @property
+    def parent(self: S) -> S:
+        """Return the parent directory of the path."""
+        if self.is_external:
+            return OtherPath(self._original.rsplit("/", 1)[0])
+        return OtherPath(super().parent)
+
+    @property
+    def name(self: S):
+        """Return the parent directory of the path."""
+        return super().name
+
+    @property
+    def suffix(self) -> str:
+        """Return the suffix of the path."""
+        return super().suffix
+
+    @property
+    def suffixes(self) -> List[str]:
+        """Return the suffixes of the path."""
+        return super().suffixes
+
+    @property
+    def stem(self) -> str:
+        """Return the stem of the path."""
+        return super().stem
+
+    def with_suffix(self: S, suffix: str) -> S:
+        """Return a new path with the suffix changed."""
+        if self.is_external:
+            logging.warning(
+                "This is method (`with_suffix`) not tested for external paths!"
+            )
+            return OtherPath(self._original.rsplit(".", 1)[0] + suffix)
+        return OtherPath(super().with_suffix(suffix))
+
+    def with_name(self: S, name: str) -> S:
+        """Return a new path with the name changed."""
+        if self.is_external:
+            logging.warning(
+                "This method (`with_name`) is not tested for external paths!"
+            )
+            return OtherPath(self._original.rsplit("/", 1)[0] + "/" + name)
+        return OtherPath(super().with_name(name))
+
+    def with_stem(self: S, stem: str) -> S:
+        """Return a new path with the stem changed."""
+        if self.is_external:
+            logging.warning(
+                "This method (`with_stem`) is not tested for external paths!"
+            )
+            return OtherPath(self._original.rsplit("/", 1)[0] + "/" + stem)
+        return OtherPath(super().with_stem(stem))
+
+    def absolute(self: S) -> S:
+        if self.is_external:
+            logging.warning(
+                "This method (`absolute`) is not implemented yet for external paths! Returning self."
+            )
+            return OtherPath(self._original)
+        return OtherPath(super().absolute())
+
+    def samefile(self: S, other_path: Union[str, pathlib.Path, S]) -> bool:
+        if self.is_external:
+            logging.warning(
+                "This method (`absolute`) is not implemented yet for external paths! Returning True."
+            )
+            return True
+        return super().samefile(other_path)
+
+    def iterdir(self, *args, **kwargs):
+        if self.is_external:
+            logging.warning(
+                f"Cannot run `iterdir` yet for external paths! Returning None."
+            )
+            return
+        else:
+            return (OtherPath(p) for p in super().iterdir())
+
+    @property
+    def parents(self, *args, **kwargs):
+        if self.is_external:
+            logging.warning(
+                f"Cannot run `parents` yet for external paths! Returning None."
+            )
+            return
+        return super().parents
+
+    def stat(self, *args, **kwargs):
+        testing = kwargs.pop("testing", False)
+        if self.is_external:
+            # logging.warning(f"Cannot run `stat` for external paths! Returning stat_result object with only zeros.")
+            try:
+                connect_kwargs, host = self._get_connection_info(testing)
+            except UnderDefined as e:
+                logging.debug(f"UnderDefined error: {e}")
+                logging.debug("Returning stat_result object with only zeros.")
+                return ExternalStatResult()
+            try:
+                return self._stat_with_fabric(host, connect_kwargs)
+            except FileNotFoundError:
+                logging.debug(
+                    "File not found! Returning stat_result object with only zeros."
+                )
+                return ExternalStatResult()
+
+        return super().stat()
+
+    def joinpath(self, *args, **kwargs):
+        logging.warning(f"Cannot run 'joinpath' for OtherPath!")
+        return OtherPath(self._original)
+
+    def readlink(self, *args, **kwargs):
+        logging.warning(f"Cannot run 'readlink' for OtherPath!")
+        return
+
+    def match(self, *args, **kwargs):
+        logging.warning(f"Cannot run 'match' for OtherPath!")
+        return
+
+    def cwd(self):
+        logging.warning(f"Cannot run 'match' for OtherPath!")
+        return
+
+    def group(self):
+        logging.warning(f"Cannot run 'group' for OtherPath!")
+        return
+
+    @property
+    def owner(self, *args, **kwargs):
+        logging.warning(f"Cannot get 'owner' for OtherPath!")
+        return
+
+    def lchmod(self, *args, **kwargs):
+        logging.warning(f"Cannot run 'lchmod' for OtherPath!")
+        return OtherPath(self._original)
+
+    @property
+    def original(self: S) -> str:
+        return self._original
+
+    @property
+    def raw_path(self: S) -> str:
+        # this will return a leading slash for some edge cases
+        return self._raw_other_path
+
+    @property
+    def full_path(self: S) -> str:
+        if self.is_external:
+            return f"{self._uri_prefix}{self._location}{self._raw_other_path}"
+        return self._original
+
+    @property
+    def pathlike_location(self: S) -> S:
+        """Return the location of the external path as a pathlike object."""
+
+        if self.is_external:
+            return OtherPath(f"{self._uri_prefix}{self._location}")
+        return OtherPath(super().drive)
+
+    @property
+    def is_external(self: S) -> bool:
+        if not hasattr(self, "_is_external"):
+            logging.warning("OBS! OtherPath object missing _is_external attribute!")
+            logging.warning("This should not happen. Please report this bug!")
+            logging.warning(
+                "(most likely means that pathlib.Path has changed and that it now has "
+                "another attribute or method that returns a new pathlib.Path object or "
+                "that you have used a method that is not supported yet)"
+            )
+            # return False
+        return self._is_external
+
+    @property
+    def uri_prefix(self) -> str:
+        """Return the uri prefix for the external path (e.g ``ssh://``)."""
+        return self._uri_prefix
+
+    @property
+    def location(self) -> str:
+        """Return the location of the external path (e.g ``user@server.com``)."""
+        return self._location
+
+    def as_uri(self) -> str:
+        """Return the path as a uri (e.g. ``scp://user@server.com/home/data/my_file.txt``)."""
+        if self._is_external:
+            return f"{self._uri_prefix}{self._location}/{'/'.join(list(super().parts)[1:])}"
+        return super().as_uri()
+
+    def copy(
+        self, destination: Optional[pathlib.Path] = None, testing=False
+    ) -> pathlib.Path:
+        """Copy the file to a destination."""
+        if destination is None:
+            destination = pathlib.Path(tempfile.gettempdir())
+        else:
+            destination = pathlib.Path(destination)
+        path_of_copied_file = destination / self.name
+
+        if not self.is_external:
+            shutil.copy2(self, destination)
+        else:
+            connect_kwargs, host = self._get_connection_info(testing)
+            self._copy_with_fabric(host, connect_kwargs, destination)
+
+        return path_of_copied_file
+
+    def _get_connection_info(self, testing: bool = False) -> Tuple[Dict, str]:
+        host = self.location
+        uri_prefix = self.uri_prefix.replace("//", "")
+        if uri_prefix not in URI_PREFIXES:
+            raise ValueError(f"uri_prefix {uri_prefix} not recognized")
+        if uri_prefix not in IMPLEMENTED_PROTOCOLS:
+            raise ValueError(
+                f"uri_prefix {uri_prefix.replace(':', '')} not implemented yet"
+            )
+        password = os.getenv(ENV_VAR_CELLPY_PASSWORD, None)
+        key_filename = os.getenv(ENV_VAR_CELLPY_KEY_FILENAME, None)
+        if password is None and key_filename is None:
+            raise UnderDefined(
+                f"You must define either {ENV_VAR_CELLPY_PASSWORD} "
+                f"or {ENV_VAR_CELLPY_KEY_FILENAME} environment variables."
+            )
+        if key_filename is not None:
+            key_filename = pathlib.Path(key_filename).expanduser().resolve()
+            connect_kwargs = {"key_filename": str(key_filename)}
+            logging.debug(f"got key_filename")
+            if not testing:
+                if not pathlib.Path(key_filename).is_file():
+                    raise FileNotFoundError(f"Could not find key file {key_filename}")
+        else:
+            connect_kwargs = {"password": password}
+        return connect_kwargs, host
+
+    def _copy_with_fabric(
+        self, host: str, connect_kwargs: dict, destination: Union[str, S, pathlib.Path]
+    ):
+        with fabric.Connection(host, connect_kwargs=connect_kwargs) as conn:
+            try:
+                t1 = time.time()
+                conn.get(self.raw_path, str(destination / self.name))
+                logging.debug(f"copying took {time.time() - t1:.2f} seconds")
+            except FileNotFoundError as e:
+                raise FileNotFoundError(
+                    f"Could not find file {self.raw_path} on {host}"
+                ) from e
+
+    def _stat_with_fabric(self, host: str, connect_kwargs: dict) -> ExternalStatResult:
+        with fabric.Connection(host, connect_kwargs=connect_kwargs) as conn:
+            try:
+                t1 = time.time()
+                sftp_conn = conn.sftp()
+                stat_result = sftp_conn.stat(self.raw_path)
+                logging.debug(f"stat took {time.time() - t1:.2f} seconds")
+                return ExternalStatResult(
+                    st_size=stat_result.st_size,
+                    st_atime=stat_result.st_atime,
+                    st_mtime=stat_result.st_mtime,
+                )
+            except FileNotFoundError as e:
+                raise FileNotFoundError(
+                    f"Could not find file {self.raw_path} on {host}"
+                ) from e
+
+    def _listdir_with_fabric(
+        self: S,
+        host: str,
+        connect_kwargs: dict,
+        levels: int = 1,
+    ) -> List[str]:
+        """List the contents of a directory through sftp."""
+
+        path_separator = "/"  # only supports unix-like systems
+        t1 = time.time()
+        with fabric.Connection(host, connect_kwargs=connect_kwargs) as conn:
+            try:
+                t1 = time.time()
+                sftp_conn = conn.sftp()
+                sftp_conn.chdir(self.raw_path)
+                sub_dirs = [f"{self.raw_path}{path_separator}{f}" for f in sftp_conn.listdir() if stat.S_ISDIR(sftp_conn.stat(f).st_mode)]
+                files = [f"{self.raw_path}{path_separator}{f}" for f in sftp_conn.listdir() if not stat.S_ISDIR(sftp_conn.stat(f).st_mode)]
+                while levels != 0:
+                    new_sub_dirs = []
+                    for sub_dir in sub_dirs:
+                        try:
+                            sftp_conn.chdir(sub_dir)
+                            _new_sub_dirs = [f"{sub_dir}{path_separator}{f}" for f in sftp_conn.listdir() if stat.S_ISDIR(sftp_conn.stat(f).st_mode)]
+                            new_files = [f"{sub_dir}{path_separator}{f}" for f in sftp_conn.listdir() if not stat.S_ISDIR(sftp_conn.stat(f).st_mode)]
+                            files += new_files
+                            new_sub_dirs += _new_sub_dirs
+                            sftp_conn.chdir(self.raw_path)
+                        except FileNotFoundError:
+                            logging.debug(f"Could not look in {sub_dir}: FileNotFoundError")
+                        pass
+                    sub_dirs = new_sub_dirs
+                    if len(sub_dirs) == 0:
+                        break
+                    levels -= 1
+
+                logging.debug(f"globbing took {time.time() - t1:.2f} seconds")
+                return files
+            except FileNotFoundError as e:
+                raise FileNotFoundError(
+                    f"Could not find file {self.raw_path} on {host}"
+                ) from e
+
+    def _glob_with_fabric(
+        self: S,
+        host: str,
+        connect_kwargs: dict,
+        glob_str: str,
+        search_in_sub_dirs: bool = False,
+    ) -> List[str]:
+        # TODO: update this so that it works faster (need some linux magic)
+        path_separator = "/"
+        with fabric.Connection(host, connect_kwargs=connect_kwargs) as conn:
+            try:
+                t1 = time.time()
+                sftp_conn = conn.sftp()
+                sftp_conn.chdir(self.raw_path)
+                if search_in_sub_dirs:  # recursive globbing one level down
+                    sub_dirs = [
+                        f
+                        for f in sftp_conn.listdir()
+                        if stat.S_ISDIR(sftp_conn.stat(f).st_mode)
+                    ]
+                    files = [
+                        f
+                        for f in sftp_conn.listdir()
+                        if not stat.S_ISDIR(sftp_conn.stat(f).st_mode)
+                    ]
+                    filtered_files = fnmatch.filter(files, glob_str)
+                    for sub_dir in sub_dirs:
+                        try:
+                            sftp_conn.chdir(sub_dir)
+                            new_files = [
+                                f
+                                for f in sftp_conn.listdir()
+                                if not stat.S_ISDIR(sftp_conn.stat(f).st_mode)
+                            ]
+                            new_filtered_files = fnmatch.filter(new_files, glob_str)
+                            new_filtered_files = [
+                                f"{sub_dir}{path_separator}{f}" for f in new_filtered_files
+                            ]
+                            filtered_files += new_filtered_files
+                            sftp_conn.chdir("..")
+                        except FileNotFoundError:
+                            logging.debug(f"Could not look in {sub_dir}: FileNotFoundError")
+                            pass
+                else:
+                    files = sftp_conn.listdir()
+                    filtered_files = fnmatch.filter(files, glob_str)
+                logging.debug(f"globbing took {time.time() - t1:.2f} seconds")
+                return filtered_files
+            except FileNotFoundError as e:
+                raise FileNotFoundError(
+                    f"Could not find file {self.raw_path} on {host}"
+                ) from e
```

### Comparing `cellpy-1.0.0a0/cellpy/log.py` & `cellpy-1.0.0a3/cellpy/log.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/cellpy/logging.json` & `cellpy-1.0.0a3/cellpy/logging.json`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/cellpy/parameters/internal_settings.py` & `cellpy-1.0.0a3/cellpy/parameters/internal_settings.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/cellpy/parameters/legacy/update_headers.py` & `cellpy-1.0.0a3/cellpy/parameters/legacy/update_headers.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/cellpy/parameters/prmreader.py` & `cellpy-1.0.0a3/cellpy/parameters/prmreader.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,380 +1,387 @@
-# -*- coding: utf-8 -*-
-import getpass
-import glob
-import logging
-import os
-import pathlib
-import sys
-import warnings
-from collections import OrderedDict
-from dataclasses import asdict, dataclass
-from pprint import pprint
-
-import box
-import dotenv
-import ruamel
-from ruamel.yaml import YAML
-from ruamel.yaml.error import YAMLError
-
-from cellpy.exceptions import ConfigFileNotRead, ConfigFileNotWritten
-from cellpy.parameters import prms
-from cellpy.parameters.internal_settings import OTHERPATHS
-from cellpy.internals.core import OtherPath
-
-DEFAULT_FILENAME_START = ".cellpy_prms_"
-DEFAULT_FILENAME_END = ".conf"
-USE_MY_DOCUMENTS = False
-
-DEFAULT_FILENAME = DEFAULT_FILENAME_START + "default" + DEFAULT_FILENAME_END
-
-# logger = logging.getLogger(__name__)
-
-yaml = YAML()
-
-
-def initialize():
-    """initializes cellpy by reading the config file and the environment file"""
-    try:
-        _read_prm_file(_get_prm_file())
-        _load_env_file()
-    except FileNotFoundError:
-        warnings.warn("Could not find the config-file")
-    except UserWarning:
-        warnings.warn("Could not read the config-file")
-
-
-def _load_env_file():
-    """loads the environment file"""
-    env_file = pathlib.Path(prms.Paths.env_file)
-    env_file_in_user_dir = pathlib.Path.home() / prms.Paths.env_file
-    if env_file.is_file():
-        dotenv.load_dotenv(env_file)
-    elif env_file_in_user_dir.is_file():
-        dotenv.load_dotenv(env_file_in_user_dir)
-    else:
-        logging.debug("No .env file found")
-
-
-def get_user_name():
-    """get the username of the current user (cross-platform)"""
-    return getpass.getuser()
-
-
-def create_custom_init_filename(user_name=None):
-    """creates a custom prms filename"""
-    if user_name is None:
-        return DEFAULT_FILENAME_START + get_user_name() + DEFAULT_FILENAME_END
-    else:
-        return DEFAULT_FILENAME_START + user_name + DEFAULT_FILENAME_END
-
-
-def get_user_dir_and_dst(init_filename=None):
-    """gets the name of the user directory and full prm filepath"""
-    if init_filename is None:
-        init_filename = create_custom_init_filename()
-    user_dir = get_user_dir()
-    dst_file = user_dir / init_filename
-    return user_dir, dst_file
-
-
-def get_user_dir():
-    """gets the name of the user directory"""
-    # user_dir = pathlib.Path(os.path.abspath(os.path.expanduser("~")))
-    user_dir = pathlib.Path().home().resolve()
-    if os.name == "nt" and USE_MY_DOCUMENTS:
-        _user_dir = user_dir / "documents"
-        if _user_dir.is_dir():
-            user_dir = _user_dir
-    return user_dir
-
-
-def _write_prm_file(file_name=None):
-    logging.debug("saving configuration to %s" % file_name)
-    config_dict = _pack_prms()
-
-    try:
-        with open(file_name, "w") as config_file:
-            yaml.allow_unicode = True
-            yaml.default_flow_style = False
-            yaml.explicit_start = True
-            yaml.explicit_end = True
-            yaml.dump(config_dict, config_file)
-    except YAMLError:
-        raise ConfigFileNotWritten
-
-
-def _update_prms(config_dict):
-    """updates the prms with the values in the config_dict"""
-    # config_dict is your current config
-    # _config_attr is the attribute in the prms module (i.e. the defaults)
-    logging.debug("updating parameters")
-    logging.debug(f"new prms: {config_dict}")
-    for key in config_dict:
-        if config_dict[key] is None:
-            logging.debug(f"{config_dict[key]} is None")
-            continue
-        if hasattr(prms, key):
-            _config_attr = getattr(prms, key)
-            is_path = isinstance(_config_attr, prms.PathsClass)
-            if _config_attr is None:
-                logging.debug(f"{_config_attr} is None")
-                continue
-            for k in config_dict[key]:
-                z = config_dict[key][k]
-                if is_path:
-                    _txt = f"{k}: {z}"
-                    if k.lower() == "db_filename":
-                        # special hack because it is a filename and not a path
-                        pass
-                    elif k.lower() in OTHERPATHS:
-                        # special hack because it is possibly an external location
-                        z = OtherPath(
-                            str(z)
-                        ).resolve()  # v1.0.0: this is only resolving local paths
-                    else:
-                        z = pathlib.Path(z).resolve()
-                    _txt += f" -> {z}"
-                    logging.debug("converting to pathlib.Path")
-                    logging.debug(_txt)
-
-                if isinstance(z, dict):
-                    y = getattr(_config_attr, k)
-                    z = box.Box({**y, **z})
-                if isinstance(z, ruamel.yaml.comments.CommentedMap):
-                    z = box.Box(z)
-                setattr(_config_attr, k, z)
-        else:
-            logging.info("\n  not-supported prm: %s" % key)
-
-
-def _convert_instruments_to_dict(x):
-    # Converting instruments to dictionary (since it contains box.Box objects)
-    d = asdict(x)
-    for k, v in d.items():
-        try:
-            d[k] = v.to_dict()
-        except AttributeError:
-            pass
-
-    return d
-
-
-def _convert_to_dict(x):
-    try:
-        dictionary = x.to_dict()
-    except AttributeError:
-        dictionary = asdict(x)
-    return dictionary
-
-
-def _convert_paths_to_dict(x):
-    dictionary = {}
-    for k in x.keys():
-        # hack to get around the leading underscore (since they are properties):
-        if len(k) > 1 and k[0] == "_" and k.lower()[1:] in OTHERPATHS:
-            t = getattr(x, k).full_path
-            k = k[1:]
-        else:
-            t = str(getattr(x, k))
-        dictionary[k] = t
-    return dictionary
-
-
-def _update_and_convert_to_dict(parameter_name):
-    """check that all the parameters are correct in the prm-file"""
-    # update from old prm-file (before v1.0.0):
-    if parameter_name == "DbCols":
-        if hasattr(prms, "DbCols"):
-            db_cols = _convert_to_dict(prms.DbCols)
-            if db_cols is None:
-                return prms.DbColsClass()
-
-            for k in db_cols:
-                if isinstance(db_cols[k], (list, tuple)):
-                    db_cols[k] = db_cols[k][0]
-            return db_cols
-        else:
-            return prms.DbColsClass()
-
-
-def _pack_prms():
-    """if you introduce new 'save-able' parameter dictionaries, then you have
-    to include them here"""
-
-    config_dict = {
-        "Paths": _convert_paths_to_dict(prms.Paths),
-        "FileNames": _convert_to_dict(prms.FileNames),
-        "Db": _convert_to_dict(prms.Db),
-        "DbCols": _update_and_convert_to_dict("DbCols"),
-        "CellInfo": _convert_to_dict(prms.CellInfo),
-        "Reader": _convert_to_dict(prms.Reader),
-        "Materials": _convert_to_dict(prms.Materials),
-        "Instruments": _convert_instruments_to_dict(prms.Instruments),
-        "Batch": _convert_to_dict(prms.Batch),
-    }
-    return config_dict
-
-
-def _read_prm_file(prm_filename):
-    """read the prm file"""
-    logging.debug("Reading config-file: %s" % prm_filename)
-    try:
-        with open(prm_filename, "r") as config_file:
-            prm_dict = yaml.load(config_file)
-
-    except YAMLError as e:
-        raise ConfigFileNotRead from e
-    else:
-        if isinstance(prm_dict, dict):
-            _update_prms(prm_dict)
-        else:
-            print(type(prm_dict))
-
-
-def _read_prm_file_without_updating(prm_filename):
-    """read the prm file but do not update the params"""
-    logging.debug("Reading config-file: %s" % prm_filename)
-    try:
-        with open(prm_filename, "r") as config_file:
-            prm_dict = yaml.load(config_file)
-
-    except YAMLError as e:
-        raise ConfigFileNotRead from e
-    return prm_dict
-
-
-def __look_at(file_name):
-    with open(file_name, "r") as config_file:
-        t = yaml.load(config_file)
-    print(t)
-
-
-def _get_prm_file(file_name=None, search_order=None):
-    """returns name of the prm file"""
-    if file_name is not None:
-        if os.path.isfile(file_name):
-            return file_name
-        else:
-            logging.info("Could not find the prm-file")
-
-    default_name = prms._prm_default_name  # NOQA
-    prm_globtxt = prms._prm_globtxt  # NOQA
-
-    script_dir = os.path.abspath(os.path.dirname(__file__))
-
-    search_path = dict()
-    search_path["curdir"] = os.path.abspath(os.path.dirname(sys.argv[0]))
-    search_path["filedir"] = script_dir
-    search_path["user_dir"] = get_user_dir()
-
-    if search_order is None:
-        search_order = ["user_dir"]  # ["curdir","filedir", "user_dir",]
-    else:
-        search_order = search_order
-
-    # The default name for the prm file is at the moment in the script-dir,@
-    # while default searching is in the user_dir (yes, I know):
-    prm_default = os.path.join(script_dir, default_name)
-
-    # -searching-----------------------
-    search_dict: OrderedDict[Any] = OrderedDict()
-
-    for key in search_order:
-        search_dict[key] = [None, None]
-        prm_directory = search_path[key]
-        default_file = os.path.join(prm_directory, default_name)
-
-        if os.path.isfile(default_file):
-            # noinspection PyTypeChecker
-            search_dict[key][0] = default_file
-
-        prm_globtxt_full = os.path.join(prm_directory, prm_globtxt)
-
-        user_files = glob.glob(prm_globtxt_full)
-
-        for f in user_files:
-            if os.path.basename(f) != os.path.basename(default_file):
-                search_dict[key][1] = f
-                break
-
-    # -selecting----------------------
-    prm_file = None
-    for key, file_list in search_dict.items():
-        if file_list[-1]:
-            prm_file = file_list[-1]
-            break
-        else:
-            if not prm_file:
-                prm_file = file_list[0]
-
-    if prm_file:
-        prm_filename = prm_file
-    else:
-        prm_filename = prm_default
-    return prm_filename
-
-
-def _save_current_prms_to_user_dir():
-    # This should be put into the cellpy setup script
-    file_name = os.path.join(prms.user_dir, prms._prm_default_name)  # NOQA
-    _write_prm_file(file_name)
-
-
-def info():
-    """this function will show only the 'box'-type
-    attributes and their content in the cellpy.prms module"""
-    print("Convenience function for listing prms")
-    print(prms.__name__)
-    print(f"prm file (for current user): {_get_prm_file()}")
-    print()
-
-    for key, current_object in prms.__dict__.items():
-        if key.startswith("_") and not key.startswith("__") and prms._debug:  # NOQA
-            print(f"Internal: {key} (type={type(current_object)}): {current_object}")
-
-        elif isinstance(current_object, box.Box):
-            print()
-            print(" OLD-TYPE PRM ".center(80, "="))
-            print(f"prms.{key}:")
-            print(80 * "-")
-            for subkey in current_object:
-                print(f"prms.{key}.{subkey} = ", f"{current_object[subkey]}")
-            print()
-
-        elif key == "Paths":
-            print(" NEW-TYPE PRM WITH OTHERPATHS ".center(80, "*"))
-            attributes = {
-                k: v for k, v in vars(current_object).items() if not k.startswith("_")
-            }
-            for attr in OTHERPATHS:
-                attributes[attr] = getattr(current_object, attr)
-            pprint(attributes, width=1)
-
-        elif isinstance(current_object, (prms.CellPyConfig, prms.CellPyDataConfig)):
-            print(" NEW-TYPE PRM ".center(80, "="))
-            attributes = {
-                k: v for k, v in vars(current_object).items() if not k.startswith("_")
-            }
-            print(f" {key} ".center(80, "="))
-            pprint(attributes, width=1)
-            print()
-
-
-def main():
-    print(" STARTING THE ACTUAL SCRIPT ".center(80, "-"))
-    print("PRM FILE:")
-    f = _get_prm_file()
-    print(f)
-    print("READING:")
-    _read_prm_file(f)
-    print("PACKING:")
-    pprint(_pack_prms())
-    print("INFO:")
-    info()
-    # print(prms)
-    # pprint(str(prms.Batch), width=1)
-    # print(prms.Batch.summary_plot_height_fractions)
-
-
-if __name__ == "__main__":
-    main()
+# -*- coding: utf-8 -*-
+import getpass
+import glob
+import logging
+import os
+import pathlib
+import sys
+import warnings
+from collections import OrderedDict
+from dataclasses import asdict, dataclass
+from pprint import pprint
+
+import box
+import dotenv
+import ruamel
+from ruamel.yaml import YAML
+from ruamel.yaml.error import YAMLError
+
+from cellpy.exceptions import ConfigFileNotRead, ConfigFileNotWritten
+from cellpy.parameters import prms
+from cellpy.parameters.internal_settings import OTHERPATHS
+from cellpy.internals.core import OtherPath
+
+DEFAULT_FILENAME_START = ".cellpy_prms_"
+DEFAULT_FILENAME_END = ".conf"
+USE_MY_DOCUMENTS = False
+
+DEFAULT_FILENAME = DEFAULT_FILENAME_START + "default" + DEFAULT_FILENAME_END
+
+# logger = logging.getLogger(__name__)
+
+yaml = YAML()
+
+
+def initialize():
+    """initializes cellpy by reading the config file and the environment file"""
+    try:
+        _read_prm_file(_get_prm_file())
+        _load_env_file()
+    except FileNotFoundError:
+        warnings.warn("Could not find the config-file")
+    except UserWarning:
+        warnings.warn("Could not read the config-file")
+
+
+def _load_env_file():
+    """loads the environment file"""
+    env_file = pathlib.Path(prms.Paths.env_file)
+    env_file_in_user_dir = pathlib.Path.home() / prms.Paths.env_file
+    if env_file.is_file():
+        dotenv.load_dotenv(env_file)
+    elif env_file_in_user_dir.is_file():
+        dotenv.load_dotenv(env_file_in_user_dir)
+    else:
+        logging.debug("No .env file found")
+
+
+def get_user_name():
+    """get the username of the current user (cross-platform)"""
+    return getpass.getuser()
+
+
+def create_custom_init_filename(user_name=None):
+    """creates a custom prms filename"""
+    if user_name is None:
+        return DEFAULT_FILENAME_START + get_user_name() + DEFAULT_FILENAME_END
+    else:
+        return DEFAULT_FILENAME_START + user_name + DEFAULT_FILENAME_END
+
+
+def get_user_dir_and_dst(init_filename=None):
+    """gets the name of the user directory and full prm filepath"""
+    if init_filename is None:
+        init_filename = create_custom_init_filename()
+    user_dir = get_user_dir()
+    dst_file = user_dir / init_filename
+    return user_dir, dst_file
+
+
+def get_user_dir():
+    """gets the name of the user directory"""
+    # user_dir = pathlib.Path(os.path.abspath(os.path.expanduser("~")))
+    user_dir = pathlib.Path().home().resolve()
+    if os.name == "nt" and USE_MY_DOCUMENTS:
+        _user_dir = user_dir / "documents"
+        if _user_dir.is_dir():
+            user_dir = _user_dir
+    return user_dir
+
+
+def _write_prm_file(file_name=None):
+    logging.debug("saving configuration to %s" % file_name)
+    config_dict = _pack_prms()
+
+    try:
+        with open(file_name, "w") as config_file:
+            yaml.allow_unicode = True
+            yaml.default_flow_style = False
+            yaml.explicit_start = True
+            yaml.explicit_end = True
+            yaml.dump(config_dict, config_file)
+    except YAMLError:
+        raise ConfigFileNotWritten
+
+
+def _update_prms(config_dict):
+    """updates the prms with the values in the config_dict"""
+    # config_dict is your current config
+    # _config_attr is the attribute in the prms module (i.e. the defaults)
+
+    logging.debug("updating parameters")
+    logging.debug(f"new prms: {config_dict}")
+    for key in config_dict:
+        if config_dict[key] is None:
+            logging.debug(f"{config_dict[key]} is None")
+            continue
+        if key == "Paths":
+            _config_attr = getattr(prms, key)
+            for k in config_dict[key]:
+                z = config_dict[key][k]
+
+                _txt = f"{k}: {z}"
+                if k.lower() == "db_filename":
+                    # special hack because it is a filename and not a path
+                    pass
+                elif k.lower() in OTHERPATHS:
+                    logging.debug("converting to OtherPath")
+                    # special hack because it is possibly an external location
+                    z = OtherPath(
+                        str(z)
+                    ).resolve()  # v1.0.0: this is only resolving local paths
+                else:
+                    logging.debug("converting to pathlib.Path")
+                    z = pathlib.Path(z).resolve()
+                _txt += f" -> {z}"
+
+                logging.debug(_txt)
+                setattr(_config_attr, k, z)
+
+        elif hasattr(prms, key):
+            _config_attr = getattr(prms, key)
+            if _config_attr is None:
+                logging.debug(f"{_config_attr} is None")
+                continue
+            for k in config_dict[key]:
+                z = config_dict[key][k]
+                if isinstance(z, dict):
+                    y = getattr(_config_attr, k)
+                    z = box.Box({**y, **z})
+                if isinstance(z, ruamel.yaml.comments.CommentedMap):
+                    z = box.Box(z)
+                setattr(_config_attr, k, z)
+        else:
+            logging.info("\n  not-supported prm: %s" % key)
+
+
+def _convert_instruments_to_dict(x):
+    # Converting instruments to dictionary (since it contains box.Box objects)
+    d = asdict(x)
+    for k, v in d.items():
+        try:
+            d[k] = v.to_dict()
+        except AttributeError:
+            pass
+
+    return d
+
+
+def _convert_to_dict(x):
+    try:
+        dictionary = x.to_dict()
+    except AttributeError:
+        dictionary = asdict(x)
+    return dictionary
+
+
+def _convert_paths_to_dict(x):
+    dictionary = {}
+    for k in x.keys():
+        # hack to get around the leading underscore (since they are properties):
+        if len(k) > 1 and k[0] == "_" and k.lower()[1:] in OTHERPATHS:
+            t = getattr(x, k).full_path
+            k = k[1:]
+        else:
+            t = str(getattr(x, k))
+        dictionary[k] = t
+    return dictionary
+
+
+def _update_and_convert_to_dict(parameter_name):
+    """check that all the parameters are correct in the prm-file"""
+    # update from old prm-file (before v1.0.0):
+    if parameter_name == "DbCols":
+        if hasattr(prms, "DbCols"):
+            db_cols = _convert_to_dict(prms.DbCols)
+            if db_cols is None:
+                return prms.DbColsClass()
+
+            for k in db_cols:
+                if isinstance(db_cols[k], (list, tuple)):
+                    db_cols[k] = db_cols[k][0]
+            return db_cols
+        else:
+            return prms.DbColsClass()
+
+
+def _pack_prms():
+    """if you introduce new 'save-able' parameter dictionaries, then you have
+    to include them here"""
+
+    config_dict = {
+        "Paths": _convert_paths_to_dict(prms.Paths),
+        "FileNames": _convert_to_dict(prms.FileNames),
+        "Db": _convert_to_dict(prms.Db),
+        "DbCols": _update_and_convert_to_dict("DbCols"),
+        "CellInfo": _convert_to_dict(prms.CellInfo),
+        "Reader": _convert_to_dict(prms.Reader),
+        "Materials": _convert_to_dict(prms.Materials),
+        "Instruments": _convert_instruments_to_dict(prms.Instruments),
+        "Batch": _convert_to_dict(prms.Batch),
+    }
+    return config_dict
+
+
+def _read_prm_file(prm_filename):
+    """read the prm file"""
+    logging.debug("Reading config-file: %s" % prm_filename)
+    try:
+        with open(prm_filename, "r") as config_file:
+            prm_dict = yaml.load(config_file)
+
+    except YAMLError as e:
+        raise ConfigFileNotRead from e
+    else:
+        if isinstance(prm_dict, dict):
+            _update_prms(prm_dict)
+        else:
+            print(type(prm_dict))
+
+
+def _read_prm_file_without_updating(prm_filename):
+    """read the prm file but do not update the params"""
+    logging.debug("Reading config-file: %s" % prm_filename)
+    try:
+        with open(prm_filename, "r") as config_file:
+            prm_dict = yaml.load(config_file)
+
+    except YAMLError as e:
+        raise ConfigFileNotRead from e
+    return prm_dict
+
+
+def __look_at(file_name):
+    with open(file_name, "r") as config_file:
+        t = yaml.load(config_file)
+    print(t)
+
+
+def _get_prm_file(file_name=None, search_order=None):
+    """returns name of the prm file"""
+    if file_name is not None:
+        if os.path.isfile(file_name):
+            return file_name
+        else:
+            logging.info("Could not find the prm-file")
+
+    default_name = prms._prm_default_name  # NOQA
+    prm_globtxt = prms._prm_globtxt  # NOQA
+
+    script_dir = os.path.abspath(os.path.dirname(__file__))
+
+    search_path = dict()
+    search_path["curdir"] = os.path.abspath(os.path.dirname(sys.argv[0]))
+    search_path["filedir"] = script_dir
+    search_path["user_dir"] = get_user_dir()
+
+    if search_order is None:
+        search_order = ["user_dir"]  # ["curdir","filedir", "user_dir",]
+    else:
+        search_order = search_order
+
+    # The default name for the prm file is at the moment in the script-dir,@
+    # while default searching is in the user_dir (yes, I know):
+    prm_default = os.path.join(script_dir, default_name)
+
+    # -searching-----------------------
+    search_dict: OrderedDict[Any] = OrderedDict()
+
+    for key in search_order:
+        search_dict[key] = [None, None]
+        prm_directory = search_path[key]
+        default_file = os.path.join(prm_directory, default_name)
+
+        if os.path.isfile(default_file):
+            # noinspection PyTypeChecker
+            search_dict[key][0] = default_file
+
+        prm_globtxt_full = os.path.join(prm_directory, prm_globtxt)
+
+        user_files = glob.glob(prm_globtxt_full)
+
+        for f in user_files:
+            if os.path.basename(f) != os.path.basename(default_file):
+                search_dict[key][1] = f
+                break
+
+    # -selecting----------------------
+    prm_file = None
+    for key, file_list in search_dict.items():
+        if file_list[-1]:
+            prm_file = file_list[-1]
+            break
+        else:
+            if not prm_file:
+                prm_file = file_list[0]
+
+    if prm_file:
+        prm_filename = prm_file
+    else:
+        prm_filename = prm_default
+    return prm_filename
+
+
+def _save_current_prms_to_user_dir():
+    # This should be put into the cellpy setup script
+    file_name = os.path.join(prms.user_dir, prms._prm_default_name)  # NOQA
+    _write_prm_file(file_name)
+
+
+def info():
+    """this function will show only the 'box'-type
+    attributes and their content in the cellpy.prms module"""
+    print("Convenience function for listing prms")
+    print(prms.__name__)
+    print(f"prm file (for current user): {_get_prm_file()}")
+    print()
+
+    for key, current_object in prms.__dict__.items():
+        if key.startswith("_") and not key.startswith("__") and prms._debug:  # NOQA
+            print(f"Internal: {key} (type={type(current_object)}): {current_object}")
+
+        elif isinstance(current_object, box.Box):
+            print()
+            print(" OLD-TYPE PRM ".center(80, "="))
+            print(f"prms.{key}:")
+            print(80 * "-")
+            for subkey in current_object:
+                print(f"prms.{key}.{subkey} = ", f"{current_object[subkey]}")
+            print()
+
+        elif key == "Paths":
+            print(" NEW-TYPE PRM WITH OTHERPATHS ".center(80, "*"))
+            attributes = {
+                k: v for k, v in vars(current_object).items() if not k.startswith("_")
+            }
+            for attr in OTHERPATHS:
+                attributes[attr] = getattr(current_object, attr)
+            pprint(attributes, width=1)
+
+        elif isinstance(current_object, (prms.CellPyConfig, prms.CellPyDataConfig)):
+            print(" NEW-TYPE PRM ".center(80, "="))
+            attributes = {
+                k: v for k, v in vars(current_object).items() if not k.startswith("_")
+            }
+            print(f" {key} ".center(80, "="))
+            pprint(attributes, width=1)
+            print()
+
+
+def main():
+    print(" STARTING THE ACTUAL SCRIPT ".center(80, "-"))
+    print("PRM FILE:")
+    f = _get_prm_file()
+    print(f)
+    print("READING:")
+    _read_prm_file(f)
+    print("PACKING:")
+    pprint(_pack_prms())
+    print("INFO:")
+    info()
+    print(prms)
+    pprint(str(prms.Batch), width=1)
+    print(prms.Batch.summary_plot_height_fractions)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `cellpy-1.0.0a0/cellpy/parameters/prms.py` & `cellpy-1.0.0a3/cellpy/parameters/prms.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,402 +1,403 @@
-"""cellpy parameters"""
-from __future__ import annotations
-import os
-import sys
-from dataclasses import dataclass, field
-from pathlib import Path
-from typing import List, Tuple, Union, Optional, TYPE_CHECKING
-
-# Using TYPE_CHECKING to avoid circular imports
-# (this will only work without from __future__ import annotations for python 3.11 and above)
-from cellpy.internals.core import OtherPath
-
-import box
-
-# When adding prms, please
-#   1) check / update the internal_settings.py file as well to
-#      ensure that copying / splitting cellpy objects
-#      behaves properly.
-#   2) check / update the .cellpy_prms_default.conf file
-
-# locations etc. for reading custom parameters
-script_dir = os.path.abspath(os.path.dirname(__file__))
-cur_dir = os.path.abspath(os.path.dirname(sys.argv[0]))
-user_dir = Path.home()
-wdir = Path(cur_dir)
-op_wdir = str(wdir)
-
-
-@dataclass
-class CellPyDataConfig:
-    """Settings that can be unique for each CellpyCell instance."""
-
-    ...
-
-
-@dataclass
-class CellPyConfig:
-    """Session settings (global)."""
-
-    def keys(self):
-        return self.__dataclass_fields__.keys()
-
-
-# If updating this, you will have to do a lot of tweaks.
-#   .cellpy_prms_default.conf
-#   cli.py (_update_paths)
-#   test_cli_setup_interactive (NUMBER_OF_DIRS)
-#   test_prms.py (config_file_txt)
-#   _convert_paths_to_dict
-
-
-# This can stay global:
-@dataclass
-class PathsClass(CellPyConfig):
-    outdatadir: Union[Path, str] = wdir
-    _rawdatadir: Union[OtherPath, str] = op_wdir
-    _cellpydatadir: Union[OtherPath, str] = op_wdir
-    db_path: Union[Path, str] = wdir  # used for simple excel db reader
-    filelogdir: Union[Path, str] = wdir
-    examplesdir: Union[Path, str] = wdir
-    notebookdir: Union[Path, str] = wdir
-    templatedir: Union[Path, str] = wdir
-    batchfiledir: Union[Path, str] = wdir
-    instrumentdir: Union[Path, str] = wdir
-    db_filename: str = "cellpy_db.xlsx"  # used for simple excel db reader
-    env_file: Union[Path, str] = user_dir / ".env_cellpy"
-
-    @property
-    def rawdatadir(self) -> OtherPath:
-        return OtherPath(self._rawdatadir)
-
-    @rawdatadir.setter
-    def rawdatadir(self, value: Union[OtherPath, Path, str]):
-        self._rawdatadir = OtherPath(value)
-
-    @property
-    def cellpydatadir(self) -> OtherPath:
-        return OtherPath(self._cellpydatadir)
-
-    @cellpydatadir.setter
-    def cellpydatadir(self, value: Union[OtherPath, Path, str]):
-        self._cellpydatadir = OtherPath(value)
-
-
-@dataclass
-class BatchClass(CellPyConfig):
-    template: str = "standard"
-    fig_extension: str = "png"
-    backend: str = "bokeh"
-    notebook: bool = True
-    dpi: int = 300
-    markersize: int = 4
-    symbol_label: str = "simple"
-    color_style_label: str = "seaborn-deep"
-    figure_type: str = "unlimited"
-    summary_plot_width: int = 900
-    summary_plot_height: int = 800
-    summary_plot_height_fractions: List[float] = field(
-        default_factory=lambda: [0.2, 0.5, 0.3]
-    )
-
-
-@dataclass
-class FileNamesClass(CellPyConfig):
-    file_name_format: str = "YYYYMMDD_[NAME]EEE_CC_TT_RR"
-    raw_extension: str = "res"
-    reg_exp: str = None
-    file_list_location: str = None
-    file_list_type: str = None
-    file_list_name: str = None
-    cellpy_file_extension: str = "h5"
-
-
-@dataclass
-class ReaderClass(CellPyConfig):
-    diagnostics: bool = False
-    filestatuschecker: str = "size"
-    force_step_table_creation: bool = True
-    force_all: bool = False  # not used yet - should be used when saving
-    sep: str = ";"
-    cycle_mode: str = "anode"
-    sorted_data: bool = True  # finding step-types assumes sorted data
-    select_minimal: bool = False
-    limit_loaded_cycles: Optional[
-        int
-    ] = None  # limit loading cycles to given cycle number
-    ensure_step_table: bool = False
-    ensure_summary_table: bool = False
-    voltage_interpolation_step: float = 0.01
-    time_interpolation_step: float = 10.0
-    capacity_interpolation_step: float = 2.0
-    use_cellpy_stat_file: bool = False
-    auto_dirs: bool = True  # search in prm-file for res and hdf5 dirs in cellpy.get()
-
-
-@dataclass
-class DbClass(CellPyConfig):
-    db_type: str = "simple_excel_reader"
-    db_table_name: str = "db_table"  # used for simple excel db reader
-    db_header_row: int = 0  # used for simple excel db reader
-    db_unit_row: int = 1  # used for simple excel db reader
-    db_data_start_row: int = 2  # used for simple excel db reader
-    db_search_start_row: int = 2  # used for simple excel db reader
-    db_search_end_row: int = -1  # used for simple excel db reader
-    db_file_sqlite: str = "excel.db"  # used when converting from Excel to sqlite
-    # database connection string - used for more advanced db readers:
-    db_connection: Optional[str] = None
-
-
-@dataclass
-class DbColsClass(CellPyConfig):  # used for simple excel db reader
-    # Note to developers:
-    #  1) This is ONLY for the excel-reader (dbreader.py)! More advanced
-    #     readers should get their own way of handling the db-columns.
-    #  2) If you would like to change the names of the attributes,
-    #     you will have to change the names in the
-    #        a .cellpy_prms_default.conf
-    #        b. dbreader.py
-    #        c. test_dbreader.py
-    #        d. internal_settings.py (renaming when making sqlite from Excel)
-    #     As well as the DbColsTypeClass below.
-
-    id: str = "id"
-    exists: str = "exists"
-    project: str = "project"
-    label: str = "label"
-    group: str = "group"
-    selected: str = "selected"
-    cell_name: str = "cell"
-    cell_type: str = "cell_type"
-    experiment_type: str = "experiment_type"
-    mass_active: str = "mass_active_material"
-    area: str = "area"
-    mass_total: str = "mass_total"
-    loading: str = "loading_active_material"
-    nom_cap: str = "nominal_capacity"
-    file_name_indicator: str = "file_name_indicator"
-    instrument: str = "instrument"
-    raw_file_names: str = "raw_file_names"
-    cellpy_file_name: str = "cellpy_file_name"
-    comment_slurry: str = "comment_slurry"
-    comment_cell: str = "comment_cell"
-    comment_general: str = "comment_general"
-    freeze: str = "freeze"
-    argument: str = "argument"
-
-    batch: str = "batch"
-    sub_batch_01: str = "b01"
-    sub_batch_02: str = "b02"
-    sub_batch_03: str = "b03"
-    sub_batch_04: str = "b04"
-    sub_batch_05: str = "b05"
-    sub_batch_06: str = "b06"
-    sub_batch_07: str = "b07"
-
-
-@dataclass
-class DbColsUnitClass(CellPyConfig):
-    # Note to developers:
-    #  1) This is ONLY for the excel-reader (dbreader.py)! More advanced
-    #     readers should get their own way of handling the db-columns.
-
-    id: str = "str"
-    exists: str = "int"
-    project: str = "str"
-    label: str = "str"
-    group: str = "str"
-    selected: str = "int"
-    cell_name: str = "str"
-    cell_type: str = "str"
-    experiment_type: str = "str"
-    mass_active: str = "float"
-    area: str = "float"
-    mass_total: str = "float"
-    loading: str = "float"
-    nom_cap: str = "float"
-    file_name_indicator: str = "str"
-    instrument: str = "str"
-    raw_file_names: str = "str"
-    cellpy_file_name: str = "str"
-    comment_slurry: str = "str"
-    comment_cell: str = "str"
-    comment_general: str = "str"
-    freeze: str = "int"
-    argument: str = "str"
-
-    batch: str = "str"
-    sub_batch_01: str = "str"
-    sub_batch_02: str = "str"
-    sub_batch_03: str = "str"
-    sub_batch_04: str = "str"
-    sub_batch_05: str = "str"
-    sub_batch_06: str = "str"
-    sub_batch_07: str = "str"
-
-
-@dataclass
-class CellInfoClass(CellPyDataConfig):
-    """Values used for setting the parameters related to the cell and the cycling"""
-
-    voltage_lim_low: float = 0.0
-    voltage_lim_high: float = 1.0
-    active_electrode_area: float = 1.0
-    active_electrode_thickness: float = 1.0
-    electrolyte_volume: float = 1.0
-
-    electrolyte_type: str = "standard"
-    active_electrode_type: str = "standard"
-    counter_electrode_type: str = "standard"
-    reference_electrode_type: str = "standard"
-    experiment_type: str = "cycling"
-    cell_type: str = "standard"
-    separator_type: str = "standard"
-    active_electrode_current_collector: str = "standard"
-    reference_electrode_current_collector: str = "standard"
-    comment: str = ""
-
-
-@dataclass
-class MaterialsClass(CellPyDataConfig):
-    """Default material-specific values used in processing the data."""
-
-    cell_class: str = "Li-Ion"
-    default_material: str = "silicon"
-    default_mass: float = 1.0
-    default_nom_cap: float = 1.0
-    default_nom_cap_specifics: str = "gravimetric"
-
-
-Paths = PathsClass()
-FileNames = FileNamesClass()
-Reader = ReaderClass()
-Db = DbClass()
-DbCols = DbColsClass()
-CellInfo = CellInfoClass()
-Materials = MaterialsClass()
-Batch = BatchClass(summary_plot_height_fractions=[0.2, 0.5, 0.3])
-
-
-# ------------------------------------------------------------------------------
-# Instruments
-#
-#  This should be updated - currently using dicts instead of subclasses of
-#  dataclasses. I guess I could update this but is a bit challenging
-#  so maybe replace later  using e.g. pydantic
-# ------------------------------------------------------------------------------
-
-
-# This can stay global:
-# remark! using box.Box for each instrument
-@dataclass
-class InstrumentsClass(CellPyConfig):
-    tester: Union[str, None]
-    custom_instrument_definitions_file: Union[str, None]
-    Arbin: box.Box
-    Maccor: box.Box
-    Neware: box.Box
-
-
-# Pre-defined instruments:
-# These can stay global:
-Arbin = {
-    "max_res_filesize": 150_000_000,
-    "chunk_size": None,
-    "max_chunks": None,
-    "use_subprocess": False,
-    "detect_subprocess_need": False,
-    "sub_process_path": None,
-    "office_version": "64bit",
-    "SQL_server": r"localhost\SQLEXPRESS",
-    "SQL_UID": "sa",
-    "SQL_PWD": "ChangeMe123",
-    "SQL_Driver": "SQL Server",
-}
-
-Arbin = box.Box(Arbin)
-
-Maccor = {"default_model": "one"}
-Maccor = box.Box(Maccor)
-
-Neware = {"default_model": "one"}
-Neware = box.Box(Neware)
-
-Instruments = InstrumentsClass(
-    tester=None,  # TODO: moving this to DataSetClass (deprecate)
-    custom_instrument_definitions_file=None,
-    Arbin=Arbin,
-    Maccor=Maccor,
-    Neware=Neware,
-)
-
-
-# ------------------------------------------------------------------------------
-# Other secret- or non-config (only for developers)
-# ------------------------------------------------------------------------------
-
-_db_cols_unit = DbColsUnitClass()
-_debug = False
-_variable_that_is_not_saved_to_config = "Hei"
-_prm_default_name = ".cellpy_prms_default.conf"
-_prm_globtxt = ".cellpy_prms*.conf"
-_odbcs = ["pyodbc", "ado", "pypyodbc"]
-_odbc = "pyodbc"
-_search_for_odbc_driver = True
-_allow_multi_test_file = False
-_use_filename_cache = True
-_sub_process_path = Path(__file__) / "../../../bin/mdbtools-win/mdb-export"
-_sub_process_path = _sub_process_path.resolve()
-_sort_if_subprocess = True
-
-_cellpyfile_root = "CellpyData"
-_cellpyfile_raw = "/raw"
-_cellpyfile_step = "/steps"
-_cellpyfile_summary = "/summary"
-_cellpyfile_fid = "/fid"
-_cellpyfile_common_meta = "/info"
-_cellpyfile_test_dependent_meta = "/info_test_dependent"
-
-_cellpyfile_raw_unit_pre_id = "raw_unit_"
-_cellpyfile_raw_limit_pre_id = ""
-
-_cellpyfile_complevel = 1
-_cellpyfile_complib = None  # currently, defaults to "zlib"
-_cellpyfile_raw_format = "table"
-_cellpyfile_summary_format = "table"
-_cellpyfile_stepdata_format = "table"
-_cellpyfile_infotable_format = "fixed"
-_cellpyfile_fidtable_format = "fixed"
-
-# templates
-_standard_template_uri = "https://github.com/jepegit/cellpy_cookies.git"
-
-_registered_templates = {
-    "standard": (_standard_template_uri, "standard"),  # (repository, name-of-folder)
-    "ife": (_standard_template_uri, "ife"),
-}
-
-# used as global variables
-_globals_status = ""
-_globals_errors = []
-_globals_message = []
-
-
-# general settings for loaders
-_minimum_columns_to_keep_for_raw_if_exists = [
-    "data_point_txt",
-    "datetime_txt",
-    "test_time_txt",
-    "step_time_txt",
-    "cycle_index_txt",
-    "step_time_txt",
-    "step_index_txt",
-    "current_txt",
-    "voltage_txt",
-    "charge_capacity_txt",
-    "discharge_capacity_txt",
-    "power_txt",
-]
-
-# used during development for testing new features
-
-_res_chunk = 0
+"""cellpy parameters"""
+from __future__ import annotations
+import os
+import sys
+from dataclasses import dataclass, field
+from pathlib import Path
+from typing import List, Tuple, Union, Optional, TYPE_CHECKING
+
+# Using TYPE_CHECKING to avoid circular imports
+# (this will only work without from __future__ import annotations for python 3.11 and above)
+from cellpy.internals.core import OtherPath
+
+import box
+
+# When adding prms, please
+#   1) check / update the internal_settings.py file as well to
+#      ensure that copying / splitting cellpy objects
+#      behaves properly.
+#   2) check / update the .cellpy_prms_default.conf file
+
+# locations etc. for reading custom parameters
+script_dir = os.path.abspath(os.path.dirname(__file__))
+cur_dir = os.path.abspath(os.path.dirname(sys.argv[0]))
+user_dir = Path.home()
+wdir = Path(cur_dir)
+op_wdir = str(wdir)
+
+
+@dataclass
+class CellPyDataConfig:
+    """Settings that can be unique for each CellpyCell instance."""
+
+    ...
+
+
+@dataclass
+class CellPyConfig:
+    """Session settings (global)."""
+
+    def keys(self):
+        return self.__dataclass_fields__.keys()
+
+
+# If updating this, you will have to do a lot of tweaks.
+#   .cellpy_prms_default.conf
+#   cli.py (_update_paths)
+#   test_cli_setup_interactive (NUMBER_OF_DIRS)
+#   test_prms.py (config_file_txt)
+#   _convert_paths_to_dict
+
+
+# This can stay global:
+@dataclass
+class PathsClass(CellPyConfig):
+    outdatadir: Union[Path, str] = wdir
+    _rawdatadir: Union[OtherPath, str] = op_wdir
+    _cellpydatadir: Union[OtherPath, str] = op_wdir
+    db_path: Union[Path, str] = wdir  # used for simple excel db reader
+    filelogdir: Union[Path, str] = wdir
+    examplesdir: Union[Path, str] = wdir
+    notebookdir: Union[Path, str] = wdir
+    templatedir: Union[Path, str] = wdir
+    batchfiledir: Union[Path, str] = wdir
+    instrumentdir: Union[Path, str] = wdir
+    db_filename: str = "cellpy_db.xlsx"  # used for simple excel db reader
+    env_file: Union[Path, str] = user_dir / ".env_cellpy"
+
+    @property
+    def rawdatadir(self) -> OtherPath:
+        return OtherPath(self._rawdatadir)
+
+    @rawdatadir.setter
+    def rawdatadir(self, value: Union[OtherPath, Path, str]):
+        self._rawdatadir = OtherPath(value)
+
+    @property
+    def cellpydatadir(self) -> OtherPath:
+        return OtherPath(self._cellpydatadir)
+
+    @cellpydatadir.setter
+    def cellpydatadir(self, value: Union[OtherPath, Path, str]):
+        self._cellpydatadir = OtherPath(value)
+
+
+@dataclass
+class BatchClass(CellPyConfig):
+    template: str = "standard"
+    fig_extension: str = "png"
+    backend: str = "bokeh"
+    notebook: bool = True
+    dpi: int = 300
+    markersize: int = 4
+    symbol_label: str = "simple"
+    color_style_label: str = "seaborn-deep"
+    figure_type: str = "unlimited"
+    summary_plot_width: int = 900
+    summary_plot_height: int = 800
+    summary_plot_height_fractions: List[float] = field(
+        default_factory=lambda: [0.2, 0.5, 0.3]
+    )
+
+
+@dataclass
+class FileNamesClass(CellPyConfig):
+    file_name_format: str = "YYYYMMDD_[NAME]EEE_CC_TT_RR"
+    raw_extension: str = "res"
+    reg_exp: str = None
+    sub_folders: bool = True
+    file_list_location: str = None
+    file_list_type: str = None
+    file_list_name: str = None
+    cellpy_file_extension: str = "h5"
+
+
+@dataclass
+class ReaderClass(CellPyConfig):
+    diagnostics: bool = False
+    filestatuschecker: str = "size"
+    force_step_table_creation: bool = True
+    force_all: bool = False  # not used yet - should be used when saving
+    sep: str = ";"
+    cycle_mode: str = "anode"
+    sorted_data: bool = True  # finding step-types assumes sorted data
+    select_minimal: bool = False
+    limit_loaded_cycles: Optional[
+        int
+    ] = None  # limit loading cycles to given cycle number
+    ensure_step_table: bool = False
+    ensure_summary_table: bool = False
+    voltage_interpolation_step: float = 0.01
+    time_interpolation_step: float = 10.0
+    capacity_interpolation_step: float = 2.0
+    use_cellpy_stat_file: bool = False
+    auto_dirs: bool = True  # search in prm-file for res and hdf5 dirs in cellpy.get()
+
+
+@dataclass
+class DbClass(CellPyConfig):
+    db_type: str = "simple_excel_reader"
+    db_table_name: str = "db_table"  # used for simple excel db reader
+    db_header_row: int = 0  # used for simple excel db reader
+    db_unit_row: int = 1  # used for simple excel db reader
+    db_data_start_row: int = 2  # used for simple excel db reader
+    db_search_start_row: int = 2  # used for simple excel db reader
+    db_search_end_row: int = -1  # used for simple excel db reader
+    db_file_sqlite: str = "excel.db"  # used when converting from Excel to sqlite
+    # database connection string - used for more advanced db readers:
+    db_connection: Optional[str] = None
+
+
+@dataclass
+class DbColsClass(CellPyConfig):  # used for simple excel db reader
+    # Note to developers:
+    #  1) This is ONLY for the excel-reader (dbreader.py)! More advanced
+    #     readers should get their own way of handling the db-columns.
+    #  2) If you would like to change the names of the attributes,
+    #     you will have to change the names in the
+    #        a .cellpy_prms_default.conf
+    #        b. dbreader.py
+    #        c. test_dbreader.py
+    #        d. internal_settings.py (renaming when making sqlite from Excel)
+    #     As well as the DbColsTypeClass below.
+
+    id: str = "id"
+    exists: str = "exists"
+    project: str = "project"
+    label: str = "label"
+    group: str = "group"
+    selected: str = "selected"
+    cell_name: str = "cell"
+    cell_type: str = "cell_type"
+    experiment_type: str = "experiment_type"
+    mass_active: str = "mass_active_material"
+    area: str = "area"
+    mass_total: str = "mass_total"
+    loading: str = "loading_active_material"
+    nom_cap: str = "nominal_capacity"
+    file_name_indicator: str = "file_name_indicator"
+    instrument: str = "instrument"
+    raw_file_names: str = "raw_file_names"
+    cellpy_file_name: str = "cellpy_file_name"
+    comment_slurry: str = "comment_slurry"
+    comment_cell: str = "comment_cell"
+    comment_general: str = "comment_general"
+    freeze: str = "freeze"
+    argument: str = "argument"
+
+    batch: str = "batch"
+    sub_batch_01: str = "b01"
+    sub_batch_02: str = "b02"
+    sub_batch_03: str = "b03"
+    sub_batch_04: str = "b04"
+    sub_batch_05: str = "b05"
+    sub_batch_06: str = "b06"
+    sub_batch_07: str = "b07"
+
+
+@dataclass
+class DbColsUnitClass(CellPyConfig):
+    # Note to developers:
+    #  1) This is ONLY for the excel-reader (dbreader.py)! More advanced
+    #     readers should get their own way of handling the db-columns.
+
+    id: str = "str"
+    exists: str = "int"
+    project: str = "str"
+    label: str = "str"
+    group: str = "str"
+    selected: str = "int"
+    cell_name: str = "str"
+    cell_type: str = "str"
+    experiment_type: str = "str"
+    mass_active: str = "float"
+    area: str = "float"
+    mass_total: str = "float"
+    loading: str = "float"
+    nom_cap: str = "float"
+    file_name_indicator: str = "str"
+    instrument: str = "str"
+    raw_file_names: str = "str"
+    cellpy_file_name: str = "str"
+    comment_slurry: str = "str"
+    comment_cell: str = "str"
+    comment_general: str = "str"
+    freeze: str = "int"
+    argument: str = "str"
+
+    batch: str = "str"
+    sub_batch_01: str = "str"
+    sub_batch_02: str = "str"
+    sub_batch_03: str = "str"
+    sub_batch_04: str = "str"
+    sub_batch_05: str = "str"
+    sub_batch_06: str = "str"
+    sub_batch_07: str = "str"
+
+
+@dataclass
+class CellInfoClass(CellPyDataConfig):
+    """Values used for setting the parameters related to the cell and the cycling"""
+
+    voltage_lim_low: float = 0.0
+    voltage_lim_high: float = 1.0
+    active_electrode_area: float = 1.0
+    active_electrode_thickness: float = 1.0
+    electrolyte_volume: float = 1.0
+
+    electrolyte_type: str = "standard"
+    active_electrode_type: str = "standard"
+    counter_electrode_type: str = "standard"
+    reference_electrode_type: str = "standard"
+    experiment_type: str = "cycling"
+    cell_type: str = "standard"
+    separator_type: str = "standard"
+    active_electrode_current_collector: str = "standard"
+    reference_electrode_current_collector: str = "standard"
+    comment: str = ""
+
+
+@dataclass
+class MaterialsClass(CellPyDataConfig):
+    """Default material-specific values used in processing the data."""
+
+    cell_class: str = "Li-Ion"
+    default_material: str = "silicon"
+    default_mass: float = 1.0
+    default_nom_cap: float = 1.0
+    default_nom_cap_specifics: str = "gravimetric"
+
+
+Paths = PathsClass()
+FileNames = FileNamesClass()
+Reader = ReaderClass()
+Db = DbClass()
+DbCols = DbColsClass()
+CellInfo = CellInfoClass()
+Materials = MaterialsClass()
+Batch = BatchClass(summary_plot_height_fractions=[0.2, 0.5, 0.3])
+
+
+# ------------------------------------------------------------------------------
+# Instruments
+#
+#  This should be updated - currently using dicts instead of subclasses of
+#  dataclasses. I guess I could update this but is a bit challenging
+#  so maybe replace later  using e.g. pydantic
+# ------------------------------------------------------------------------------
+
+
+# This can stay global:
+# remark! using box.Box for each instrument
+@dataclass
+class InstrumentsClass(CellPyConfig):
+    tester: Union[str, None]
+    custom_instrument_definitions_file: Union[str, None]
+    Arbin: box.Box
+    Maccor: box.Box
+    Neware: box.Box
+
+
+# Pre-defined instruments:
+# These can stay global:
+Arbin = {
+    "max_res_filesize": 150_000_000,
+    "chunk_size": None,
+    "max_chunks": None,
+    "use_subprocess": False,
+    "detect_subprocess_need": False,
+    "sub_process_path": None,
+    "office_version": "64bit",
+    "SQL_server": r"localhost\SQLEXPRESS",
+    "SQL_UID": "sa",
+    "SQL_PWD": "ChangeMe123",
+    "SQL_Driver": "SQL Server",
+}
+
+Arbin = box.Box(Arbin)
+
+Maccor = {"default_model": "one"}
+Maccor = box.Box(Maccor)
+
+Neware = {"default_model": "one"}
+Neware = box.Box(Neware)
+
+Instruments = InstrumentsClass(
+    tester=None,  # TODO: moving this to DataSetClass (deprecate)
+    custom_instrument_definitions_file=None,
+    Arbin=Arbin,
+    Maccor=Maccor,
+    Neware=Neware,
+)
+
+
+# ------------------------------------------------------------------------------
+# Other secret- or non-config (only for developers)
+# ------------------------------------------------------------------------------
+
+_db_cols_unit = DbColsUnitClass()
+_debug = False
+_variable_that_is_not_saved_to_config = "Hei"
+_prm_default_name = ".cellpy_prms_default.conf"
+_prm_globtxt = ".cellpy_prms*.conf"
+_odbcs = ["pyodbc", "ado", "pypyodbc"]
+_odbc = "pyodbc"
+_search_for_odbc_driver = True
+_allow_multi_test_file = False
+_use_filename_cache = True
+_sub_process_path = Path(__file__) / "../../../bin/mdbtools-win/mdb-export"
+_sub_process_path = _sub_process_path.resolve()
+_sort_if_subprocess = True
+
+_cellpyfile_root = "CellpyData"
+_cellpyfile_raw = "/raw"
+_cellpyfile_step = "/steps"
+_cellpyfile_summary = "/summary"
+_cellpyfile_fid = "/fid"
+_cellpyfile_common_meta = "/info"
+_cellpyfile_test_dependent_meta = "/info_test_dependent"
+
+_cellpyfile_raw_unit_pre_id = "raw_unit_"
+_cellpyfile_raw_limit_pre_id = ""
+
+_cellpyfile_complevel = 1
+_cellpyfile_complib = None  # currently, defaults to "zlib"
+_cellpyfile_raw_format = "table"
+_cellpyfile_summary_format = "table"
+_cellpyfile_stepdata_format = "table"
+_cellpyfile_infotable_format = "fixed"
+_cellpyfile_fidtable_format = "fixed"
+
+# templates
+_standard_template_uri = "https://github.com/jepegit/cellpy_cookies.git"
+
+_registered_templates = {
+    "standard": (_standard_template_uri, "standard"),  # (repository, name-of-folder)
+    "ife": (_standard_template_uri, "ife"),
+}
+
+# used as global variables
+_globals_status = ""
+_globals_errors = []
+_globals_message = []
+
+
+# general settings for loaders
+_minimum_columns_to_keep_for_raw_if_exists = [
+    "data_point_txt",
+    "datetime_txt",
+    "test_time_txt",
+    "step_time_txt",
+    "cycle_index_txt",
+    "step_time_txt",
+    "step_index_txt",
+    "current_txt",
+    "voltage_txt",
+    "charge_capacity_txt",
+    "discharge_capacity_txt",
+    "power_txt",
+]
+
+# used during development for testing new features
+
+_res_chunk = 0
```

### Comparing `cellpy-1.0.0a0/cellpy/readers/cellreader.py` & `cellpy-1.0.0a3/cellpy/readers/cellreader.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/cellpy/readers/core.py` & `cellpy-1.0.0a3/cellpy/readers/core.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/cellpy/readers/dbreader.py` & `cellpy-1.0.0a3/cellpy/readers/dbreader.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/cellpy/readers/filefinder.py` & `cellpy-1.0.0a3/cellpy/readers/instruments/custom.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,253 +1,289 @@
-# -*- coding: utf-8 -*-
+"""This module is used for loading data using the `instrument="custom"` method.
+If no `instrument_file` is given (either directly or through the use
+of the :: separator), the default instrument file (yaml) will be used."""
+
+# This module works, but is by no means finished. The module is meant to
+# be developed further allowing for example
+# to provide custom parsers. At the moment, we anticipate that it only should
+# work with txt-files (so the class is called CustomTxtLoader), however, it is
+# possible to extend the scope to allow for providing parsers that also can read
+# binary files. The future will show.
 
-import fnmatch
-import glob
 import logging
-import os
-import pathlib
-import time
-from typing import Optional, Union, List, Tuple
-import warnings
-
-import cellpy.exceptions
-from cellpy.parameters import prms
-from cellpy.internals.core import OtherPath
-
-
-def search_for_files(
-    run_name: str,
-    raw_extension: Optional[str] = None,
-    cellpy_file_extension: Optional[str] = None,
-    raw_file_dir: Union[OtherPath, pathlib.Path, str, None] = None,
-    cellpy_file_dir: Union[OtherPath, pathlib.Path, str, None] = None,
-    prm_filename: Union[pathlib.Path, str, None] = None,
-    file_name_format: Optional[str] = None,
-    reg_exp: Optional[str] = None,
-    sub_folders: bool = False,
-    file_list: Optional[List[str]] = None,
-    pre_path: Union[OtherPath, pathlib.Path, str, None] = None,
-) -> Tuple[List[str], str]:
-    """Searches for files (raw-data files and cellpy-files).
-
-
-    Args:
-        run_name(str): run-file identification.
-        raw_extension(str): optional, extension of run-files (without the '.').
-        cellpy_file_extension(str): optional, extension for cellpy files
-            (without the '.').
-        raw_file_dir(path): optional, directory where to look for run-files
-            (default: read prm-file)
-        cellpy_file_dir(path): optional, directory where to look for
-            cellpy-files (default: read prm-file)
-        prm_filename(path): optional parameter file can be given.
-        file_name_format(str): format of raw-file names or a glob pattern
-            (default: YYYYMMDD_[name]EEE_CC_TT_RR).
-        reg_exp(str): use regular expression instead (defaults to None).
-        sub_folders (bool): perform search also in sub-folders.
-        file_list (list of str): perform the search within a given list
-            of filenames instead of searching the folder(s). The list should
-            not contain the full filepath (only the actual file names). If
-            you want to provide the full path, you will have to modify the
-            file_name_format or reg_exp accordingly.
-        pre_path (path or str): path to prepend the list of files selected
-             from the file_list.
-
-
-    Returns:
-        run-file names (list of strings) and cellpy-file-name (str of full path).
-    """
-
-    # TODO: @jepe - use reg_exp
-    # TODO: @jepe - allow for searching in cloud
-    # TODO: @jepe - how to implement searching in db?
-    # TODO: update prms and conf file to allow for setting if search should be done in
-    #  sub-folders, several folders, db, cloud etc
-    # TODO: @jepe - find a way to implement automatic file_list creation in a top level func.
-
-    version = 0.3
-    t0 = time.time()
-
-    if reg_exp is None:
-        reg_exp = prms.FileNames.reg_exp
-
-    if raw_extension is None:
-        raw_extension = prms.FileNames.raw_extension
-
-    if raw_extension is None:
-        raw_extension = prms.FileNames.raw_extension
-
-    if cellpy_file_extension is None:
-        cellpy_file_extension = prms.FileNames.cellpy_file_extension
-
-    # backward compatibility check
-    if cellpy_file_extension.startswith("."):
-        warnings.warn(
-            "Deprecation warning: cellpy_file_extension should not include the '.'"
+import sys
+from abc import ABC
+from pathlib import Path
+
+import pandas as pd
+
+from cellpy import prms
+from cellpy.readers.instruments.base import find_delimiter_and_start, AutoLoader
+from cellpy.readers.instruments.configurations import (
+    register_local_configuration_from_yaml_file,
+)
+
+
+class DataLoader(AutoLoader, ABC):
+    """Class for loading data from txt files."""
+
+    instrument_name = "custom"
+    raw_ext = "*"
+
+    def __init__(self, instrument_file=None, **kwargs):
+        if instrument_file is None:
+            logging.debug("No instrument_file provided - checking default")
+            instrument_file = prms.Instruments.custom_instrument_definitions_file
+        if not instrument_file:
+            raise FileExistsError(
+                "Missing instrument definition file "
+                "(not given and not defined in config)"
+            )
+        if not Path(instrument_file).is_file():
+            # searching in the Instruments folder:
+            instrument_dir = Path(prms.Paths.instrumentdir)
+            logging.debug(f"Looking for file in {instrument_dir}")
+            instrument_file_in_instrument_dir = instrument_dir / instrument_file
+            if not instrument_file_in_instrument_dir.is_file():
+                logging.debug(f"Could not find {instrument_file_in_instrument_dir}")
+                raise FileExistsError(
+                    "Instrument definition file not found! " f"({instrument_file})"
+                )
+            instrument_file = instrument_file_in_instrument_dir
+
+        logging.debug(f"Instrument definition file: {instrument_file}")
+        self.local_instrument_file = instrument_file
+        super().__init__()
+
+    default_model = None
+    supported_models = None
+
+    def pre_init(self):
+        self.auto_register_config = False
+        self.config_params = register_local_configuration_from_yaml_file(
+            self.local_instrument_file
         )
-        cellpy_file_extension = cellpy_file_extension[1:]
-        warnings.warn(f"Removing it -> {cellpy_file_extension}")
 
-    if raw_file_dir is None:
-        raw_file_dir = prms.Paths.rawdatadir
+    # TODO: rewrite this:
+    def parse_loader_parameters(self, **kwargs):
+        auto_format = kwargs.get("auto_format", False)
+        if auto_format:
+            self._auto_formatter()
+
+    def _config_sub_parser(self, key_label, default_value=None, **kwargs):
+        return kwargs.pop(
+            key_label, self.config_params.formatters.get(key_label, default_value)
+        )
 
-    if file_name_format is None:
-        file_name_format = prms.FileNames.file_name_format
+    # TODO: rewrite this:
+    def parse_formatter_parameters(self, **kwargs):
+        self.file_format = self._config_sub_parser(
+            "file_format", default_value="csv", **kwargs
+        )
+        # print("FORMATTERS".center(80, "="))
+        # print(self.config_params.formatters)
 
-    if not isinstance(raw_file_dir, (list, tuple)):
-        raw_file_dir = [OtherPath(raw_file_dir)]
-    else:
-        raw_file_dir = [OtherPath(d) for d in raw_file_dir]
+        # rewrite this on a later stage to use functions and dict lookup instead of if - else
+        if self.file_format == "csv":
+            self.sep = self._config_sub_parser("sep", default_value=None, **kwargs)
+            self.skiprows = self._config_sub_parser(
+                "skiprows", default_value=0, **kwargs
+            )
+            self.header = self._config_sub_parser("header", default_value=0, **kwargs)
+            self.encoding = self._config_sub_parser(
+                "encoding", default_value="utf-8", **kwargs
+            )
+            self.decimal = self._config_sub_parser(
+                "decimal", default_value=".", **kwargs
+            )
+            self.thousands = self._config_sub_parser(
+                "thousands", default_value=None, **kwargs
+            )
+
+        elif self.file_format == "xlsx":
+            self.table_name = self._config_sub_parser(
+                "table_name", default_value="sheet 1", **kwargs
+            )
 
-    if reg_exp:
-        logging.warning(f"Got reg_exp: {reg_exp}")
-        logging.warning("Sorry, but using reg exp is not implemented yet.")
+        elif self.file_format == "xls":
+            self.table_name = self._config_sub_parser(
+                "table_name", default_value="sheet 1", **kwargs
+            )
 
-    if prm_filename is not None:
-        logging.debug("Sorry, reading prm file is not implemented yet.")
+        elif self.file_format == "json":
+            print("json not implemented yet")
+            sys.exit()
+
+        else:
+            print(f"{self.file_format} not implemented yet")
+            sys.exit()
+
+    # TODO: consider rewriting this:
+    def _auto_formatter(self):
+        separator, first_index = find_delimiter_and_start(
+            self.name,
+            separators=None,
+            checking_length_header=100,
+            checking_length_whole=200,
+        )
+        self.encoding = "UTF-8"  # consider adding a find_encoding function
+        self.sep = separator
+        self.skiprows = first_index - 1  # consider adding a find_rows_to_skip function
+        self.header = 0  # consider adding a find_header function
 
-    if cellpy_file_dir is None:
-        cellpy_file_dir = OtherPath(prms.Paths.cellpydatadir)
-    else:
-        cellpy_file_dir = OtherPath(cellpy_file_dir)
+        logging.critical(
+            f"auto-formatting:\n  {self.sep=}\n  {self.skiprows=}\n  {self.header=}\n  {self.encoding=}\n"
+        )
+
+    def query_file(self, name):
+        # rewrite this on a later stage to use functions and dict lookup instead of if - else
+        if self.file_format == "csv":
+            logging.debug(f"parsing with pandas.read_csv: {name}")
+            logging.critical(
+                f"{self.sep=}, {self.skiprows=}, {self.header=}, {self.encoding=}, {self.decimal=}"
+            )
+            data_df = pd.read_csv(
+                name,
+                sep=self.sep,
+                skiprows=self.skiprows,
+                header=self.header,
+                encoding=self.encoding,
+                decimal=self.decimal,
+                thousands=self.thousands,
+            )
+        elif self.file_format == "xls":
+            logging.debug(
+                f"parsing with pandas.read_excel using xlrd (old format): {name}"
+            )
+            sheet_name = self.table_name
+
+            raw_frame = pd.read_excel(name, engine="xlrd", sheet_name=None)
+            matching = [s for s in raw_frame.keys() if s.startswith(sheet_name)]
+            if matching:
+                return raw_frame[matching[0]]
+            raise IOError(f"Could not find the sheet {sheet_name} in {name}")
+
+        elif self.file_format == "xlsx":
+            logging.debug(f"parsing with pandas.read_excel: {name}")
+            sheet_name = self.table_name
+            raw_frame = pd.read_excel(
+                name, engine="openpyxl", sheet_name=None
+            )  # TODO: replace this with pd.ExcelReader
+            matching = [s for s in raw_frame.keys() if s.startswith(sheet_name)]
+            if matching:
+                logging.debug(f"read sheet: {sheet_name}")
+                return raw_frame[matching[0]]
+            raise IOError(f"Could not find the sheet {sheet_name} in {name}")
+
+        elif self.file_format == "json":
+            raise IOError(
+                f"Could not read {name}, {self.file_format} not supported yet"
+            )
+        else:
+            raise IOError(
+                f"Could not read {name}, {self.file_format} not supported yet"
+            )
+
+        return data_df
+
+
+def check_loader_from_outside_with_get():
+    import pathlib
+
+    import cellpy
 
-    if file_name_format is None and reg_exp is None:
-        try:
-            # To be implemented in version 0.5:
-            file_name_format = prms.FileNames.file_name_format
-        except AttributeError:
-            file_name_format = "YYYYMMDD_[name]EEE_CC_TT_RR"
-
-    if file_name_format.upper() == "YYYYMMDD_[NAME]EEE_CC_TT_RR":
-        # backward compatibility check
-        if raw_extension.startswith("."):
-            warnings.warn(
-                "Deprecation warning: raw_extension should not include the '.'"
-            )
-            raw_extension = raw_extension[1:]
-            warnings.warn(f"Removing it -> {raw_extension}")
-        # TODO: give warning/error-message if run_name contains more than one file (due to duplicate in db)
-        glob_text_raw = f"{run_name}*.{raw_extension}"
+    pd.options.display.max_columns = 100
+
+    base_path_win = pathlib.Path("C:/scripting")
+    base_path_mac = pathlib.Path("/Users/jepe/scripting")
+
+    if sys.platform == "win32":
+        base_path = base_path_win
+        out = pathlib.Path(r"C:\scripting\trash")
     else:
-        glob_text_raw = file_name_format
+        base_path = base_path_mac
+        out = pathlib.Path("/Users/jepe/tmp")
+
+    instrument = "custom"
 
-    logging.debug(f"searching for raw files in: {raw_file_dir}")
-    logging.debug(f"searching for {run_name}")
-    logging.debug(f"using glob {glob_text_raw}")
-
-    cellpy_file = f"{run_name}.{cellpy_file_extension}"
-    cellpy_file = cellpy_file_dir / cellpy_file
-    # Not sure if for example pandas can handle OtherPath objects:
-    cellpy_file = cellpy_file.full_path
-
-    logging.debug(f"generated cellpy filename {cellpy_file}")
-
-    if file_list is not None:
-        if len(raw_file_dir) > 1:
-            logging.info("you provided several raw file directories")
-        logging.debug("searching within provided list of files")
-        run_files = fnmatch.filter(file_list, glob_text_raw)
-        if pre_path is not None:
-            pre_path = OtherPath(pre_path)
-            run_files = list(map(lambda x: pre_path / x, run_files))
+    file_number = 3
+
+    if file_number == 1:
+        filename = "custom_data_001.csv"
+        instrument_file = "cellpy/testdata/data/custom_instrument_001.yml"
+    elif file_number == 2:
+        filename = "custom_data_002.xlsx"
+        instrument_file = "cellpy/testdata/instruments/custom_002.yml"
+    elif file_number == 3:
+        filename = "custom_data_003.xls"
+        instrument_file = "cellpy/testdata/instruments/custom_003.yml"
     else:
-        run_files = []
-        for d in raw_file_dir:
-            if d.is_external:
-                logging.debug("external file")
-            if not d.is_dir():
-                warnings.warn("your raw file directory cannot be accessed!")
-                # raise cellpy.exceptions.IOError("your raw file directory cannot be accessed!")
-                _run_files = []
-            else:
-                logging.debug(f"checking in folder {d}")
-
-                if sub_folders:
-                    _run_files = d.rglob(glob_text_raw)
-
-                else:
-                    _run_files = d.glob(glob_text_raw)
-
-                _run_files = [str(_f.resolve()) for _f in _run_files]
-                _run_files.sort()
-            run_files.extend(_run_files)
-
-    return run_files, cellpy_file
-
-
-def check_01():
-    import dotenv
-    from cellpy import log
-
-    log.setup_logging(default_level="DEBUG")
-    dotenv.load_dotenv(r"C:\scripting\cellpy\local\.env_cellpy_local")
-    print("searching for files")
-    my_run_name = "20160805_test001_45_cc"
-    # my_run_name = "20210218_Seam08_02_01_cc"
-    my_raw_file_dir = OtherPath(
-        f"scp://{os.getenv('CELLPY_HOST')}/home/{os.getenv('CELLPY_USER')}/tmp/"
+        print("not implemented")
+        return
+
+    # NEXT: test hooks and make tests
+
+    instrument_file = base_path / instrument_file
+    data_dir = base_path / "cellpy/testdata/data"
+    name = data_dir / filename
+
+    print(f"File exists? {name.is_file()}")
+    if not name.is_file():
+        print(f"could not find {name} ")
+        return
+
+    print(" RUNNING CELLPY GET ".center(80, "="))
+    print(f"{instrument=}")
+
+    c = cellpy.get(
+        filename=name,
+        instrument=instrument,
+        instrument_file=instrument_file,
+        mass=1.0,
+        auto_summary=False,
     )
-    # my_raw_file_dir = OtherPath(r"C:\scripting\processing_cellpy\raw")
-    my_cellpy_file_dir = OtherPath("C:/scripting/processing_cellpy/data/")
-    f = search_for_files(
-        my_run_name, raw_file_dir=my_raw_file_dir, cellpy_file_dir=my_cellpy_file_dir
+    _process_cellpy_object(name, c, out)
+
+
+def _process_cellpy_object(name, c, out):
+    import matplotlib.pyplot as plt
+
+    pd.options.display.max_columns = 100
+
+    print(f"loaded the file - now lets see what we got")
+    raw = c.data.raw
+    raw.to_clipboard()
+    print(raw.head())
+    c.make_step_table()
+
+    steps = c.data.steps
+    summary = c.data.summary
+
+    raw.to_csv(out / "raw.csv", sep=";")
+    steps.to_csv(out / "steps.csv", sep=";")
+    summary.to_csv(out / "summary.csv", sep=";")
+
+    fig_1, (ax1, ax2, ax3, ax4) = plt.subplots(
+        4,
+        1,
+        figsize=(6, 10),
+        constrained_layout=True,
+        sharex=True,
     )
-    print(f)
-    #
-    # print(my_raw_file_dir)
-    # print(my_raw_file_dir.is_dir())
-    # print(my_raw_file_dir.raw_path)
-
-
-def check_02():
-    import dotenv
-    import fabric
-    import stat
-
-    dotenv.load_dotenv(r"C:\scripting\cellpy\local\.env_cellpy_local")
-    host = os.getenv("CELLPY_HOST")
-    user = os.getenv("CELLPY_USER")
-    key_file = os.getenv("CELLPY_KEY_FILENAME")
-    print(f"host: {host}")
-    print(f"user: {user}")
-    connect_kwargs = {"key_filename": key_file}
-
-    with fabric.Connection(host, connect_kwargs=connect_kwargs) as conn:
-        sftp_conn = conn.sftp()
-        sftp_conn.chdir("tmp")
-        print("===================")
-        for fileattr in sftp_conn.listdir_attr():
-            if stat.S_ISDIR(fileattr.st_mode):
-                print(f"dir: {fileattr.filename}")
-            else:
-                print(f"file: {fileattr.filename}")
-        print("===================")
-        glob_str = "20*.res"
-        sub_dirs = [
-            f for f in sftp_conn.listdir() if stat.S_ISDIR(sftp_conn.stat(f).st_mode)
-        ]
-        files = [
-            f
-            for f in sftp_conn.listdir()
-            if not stat.S_ISDIR(sftp_conn.stat(f).st_mode)
-        ]
-        filtered_files = fnmatch.filter(files, glob_str)
-        for sub_dir in sub_dirs:
-            sftp_conn.chdir(sub_dir)
-            new_files = [
-                f
-                for f in sftp_conn.listdir()
-                if not stat.S_ISDIR(sftp_conn.stat(f).st_mode)
-            ]
-            new_filtered_files = fnmatch.filter(new_files, glob_str)
-            new_filtered_files = [
-                f"{sub_dir}{path_separator}{f}" for f in new_filtered_files
-            ]
-            filtered_files += new_filtered_files
-            sftp_conn.chdir("..")
+    raw.plot(x="test_time", y="voltage", ax=ax1)
+    raw.plot(x="test_time", y="current", ax=ax2)
+    raw.plot(x="test_time", y=["charge_capacity", "discharge_capacity"], ax=ax3)
+    raw.plot(x="test_time", y="cycle_index", ax=ax4)
+    fig_1.suptitle(f"{name.name}", fontsize=16)
+
+    n = c.get_number_of_cycles()
+    print(f"Number of cycles: {n}")
+
+    plt.legend()
+    plt.show()
 
-        for f in filtered_files:
-            print(f"file: {f} of type {type(f)}")
+    outfile = out / "test_out"
+    c.save(outfile)
 
 
 if __name__ == "__main__":
-    check_01()
+    check_loader_from_outside_with_get()
```

### Comparing `cellpy-1.0.0a0/cellpy/readers/instruments/arbin_res.py` & `cellpy-1.0.0a3/cellpy/readers/instruments/arbin_res.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/cellpy/readers/instruments/arbin_sql.py` & `cellpy-1.0.0a3/cellpy/readers/instruments/arbin_sql.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/cellpy/readers/instruments/arbin_sql_7.py` & `cellpy-1.0.0a3/cellpy/readers/instruments/arbin_sql_7.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/cellpy/readers/instruments/arbin_sql_csv.py` & `cellpy-1.0.0a3/cellpy/readers/instruments/arbin_sql_csv.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/cellpy/readers/instruments/arbin_sql_h5.py` & `cellpy-1.0.0a3/cellpy/readers/instruments/arbin_sql_h5.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/cellpy/readers/instruments/arbin_sql_xlsx.py` & `cellpy-1.0.0a3/cellpy/readers/instruments/arbin_sql_xlsx.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/cellpy/readers/instruments/base.py` & `cellpy-1.0.0a3/cellpy/readers/instruments/base.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/cellpy/readers/instruments/biologics_mpr.py` & `cellpy-1.0.0a3/cellpy/readers/instruments/biologics_mpr.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/cellpy/readers/instruments/configurations/__init__.py` & `cellpy-1.0.0a3/cellpy/readers/instruments/configurations/__init__.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/cellpy/readers/instruments/configurations/maccor_txt_four.py` & `cellpy-1.0.0a3/cellpy/readers/instruments/configurations/maccor_txt_four.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/cellpy/readers/instruments/configurations/maccor_txt_one.py` & `cellpy-1.0.0a3/cellpy/readers/instruments/configurations/maccor_txt_one.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/cellpy/readers/instruments/configurations/maccor_txt_three.py` & `cellpy-1.0.0a3/cellpy/readers/instruments/configurations/maccor_txt_three.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/cellpy/readers/instruments/configurations/maccor_txt_two.py` & `cellpy-1.0.0a3/cellpy/readers/instruments/configurations/maccor_txt_two.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/cellpy/readers/instruments/configurations/maccor_txt_zero.py` & `cellpy-1.0.0a3/cellpy/readers/instruments/configurations/maccor_txt_zero.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/cellpy/readers/instruments/configurations/neware_txt_zero.py` & `cellpy-1.0.0a3/cellpy/readers/instruments/configurations/neware_txt_zero.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/cellpy/readers/instruments/ext_nda_reader.py` & `cellpy-1.0.0a3/cellpy/readers/instruments/ext_nda_reader.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/cellpy/readers/instruments/loader_specific_modules/biologic_file_format.py` & `cellpy-1.0.0a3/cellpy/readers/instruments/loader_specific_modules/biologic_file_format.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/cellpy/readers/instruments/local_instrument.py` & `cellpy-1.0.0a3/cellpy/readers/instruments/local_instrument.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/cellpy/readers/instruments/maccor_txt.py` & `cellpy-1.0.0a3/cellpy/readers/instruments/maccor_txt.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/cellpy/readers/instruments/neware_txt.py` & `cellpy-1.0.0a3/cellpy/readers/instruments/neware_txt.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/cellpy/readers/instruments/pec_csv.py` & `cellpy-1.0.0a3/cellpy/readers/instruments/pec_csv.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/cellpy/readers/instruments/processors/post_processors.py` & `cellpy-1.0.0a3/cellpy/readers/instruments/processors/post_processors.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/cellpy/readers/instruments/processors/pre_processors.py` & `cellpy-1.0.0a3/cellpy/readers/instruments/processors/pre_processors.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/cellpy/readers/sql_dbreader.py` & `cellpy-1.0.0a3/cellpy/readers/sql_dbreader.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/cellpy/utils/batch.py` & `cellpy-1.0.0a3/cellpy/utils/batch.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,1249 +1,1252 @@
-"""Routines for batch processing of cells (v2)."""
-
-import logging
-import os
-import pathlib
-import shutil
-import sys
-import warnings
-
-import pandas as pd
-from pandas import Index
-from tqdm.auto import tqdm
-
-import cellpy.exceptions
-from cellpy import log, prms
-from cellpy.parameters.internal_settings import (
-    headers_journal,
-    headers_step_table,
-    headers_summary,
-)
-from cellpy.internals.core import OtherPath
-from cellpy.utils.batch_tools.batch_analyzers import (
-    BaseSummaryAnalyzer,
-    OCVRelaxationAnalyzer,
-)
-from cellpy.utils.batch_tools.batch_core import Data
-from cellpy.utils.batch_tools.batch_experiments import CyclingExperiment
-from cellpy.utils.batch_tools.batch_exporters import CSVExporter
-from cellpy.utils.batch_tools.batch_journals import LabJournal
-from cellpy.utils.batch_tools.batch_plotters import CyclingSummaryPlotter
-from cellpy.utils.batch_tools.dumpers import ram_dumper
-
-# logger = logging.getLogger(__name__)
-logging.captureWarnings(True)
-
-COLUMNS_SELECTED_FOR_VIEW = [
-    headers_journal.mass,
-    headers_journal.total_mass,
-    headers_journal.loading,
-    headers_journal.nom_cap,
-]
-
-
-class Batch:
-    """A convenient class for running batch procedures.
-
-    The Batch class contains among other things:
-        - iterator protocol
-        - a journal with info about the different cells where the
-        main information is accessible as a pandas.DataFrame through the `.pages` attribute
-        - a data lookup accessor `.data` that behaves similarly as a dict.
-    """
-
-    def __init__(self, *args, **kwargs):
-        """Initialize the Batch class.
-
-        The initialization accepts arbitrary arguments and keyword arguments.
-        It first looks for the file_name and db_reader keyword arguments.
-
-        Usage:
-            b = Batch((name, (project)), **kwargs)
-
-        Examples:
-            >>> b = Batch("experiment001", "main_project")
-            >>> b = Batch("experiment001", "main_project", batch_col="b02")
-            >>> b = Batch(name="experiment001", project="main_project", batch_col="b02")
-            >>> b = Batch(file_name="cellpydata/batchfiles/cellpy_batch_experiment001.json")
-
-        Keyword Args (priority):
-            file_name (str or pathlib.Path): journal file name to load.
-            db_reader (str): data-base reader to use (defaults to "default" as given
-                in the config-file or prm-class).
-            frame (pandas.DataFrame): load from given dataframe.
-        Args:
-            *args: name (str) (project (str))
-
-        Keyword Args (other):
-            default_log_level (str): custom log-level (defaults to None (i.e. default log-level in cellpy)).
-            custom_log_dir (str or pathlib.Path): custom folder for putting the log-files.
-            force_raw_file (bool): load from raw regardless (defaults to False).
-            force_cellpy (bool): load cellpy-files regardless (defaults to False).
-            force_recalc (bool): Always recalculate (defaults to False).
-            export_cycles (bool): Extract and export individual cycles to csv (defaults to True).
-            export_raw (bool): Extract and export raw-data to csv (defaults to True).
-            export_ica (bool): Extract and export individual dQ/dV data to csv (defaults to True).
-            accept_errors (bool): Continue automatically to next file if error is raised (defaults to False).
-            nom_cap (float): give a nominal capacity if you want to use another value than
-                the one given in the config-file or prm-class.
-        """
-        # TODO: add option for setting max cycle number
-        #   use self.experiment.last_cycle = xxx
-        default_log_level = kwargs.pop("log_level", None)
-        custom_log_dir = kwargs.pop("custom_log_dir", None)
-        if default_log_level is not None or custom_log_dir is not None:
-            log.setup_logging(
-                custom_log_dir=custom_log_dir,
-                default_level=default_log_level,
-                reset_big_log=True,
-            )
-
-        db_reader = kwargs.pop("db_reader", "default")
-
-        file_name = kwargs.pop("file_name", None)
-        frame = kwargs.pop("frame", None)
-
-        logging.debug("creating CyclingExperiment")
-        self.experiment = CyclingExperiment(db_reader=db_reader)
-        logging.info("created CyclingExperiment")
-
-        self.experiment.force_cellpy = kwargs.pop("force_cellpy", False)
-        self.experiment.force_raw = kwargs.pop("force_raw_file", False)
-        self.experiment.force_recalc = kwargs.pop("force_recalc", False)
-        self.experiment.export_cycles = kwargs.pop("export_cycles", True)
-        self.experiment.export_raw = kwargs.pop("export_raw", True)
-        self.experiment.export_ica = kwargs.pop("export_ica", False)
-        self.experiment.accept_errors = kwargs.pop("accept_errors", False)
-        self.experiment.nom_cap = kwargs.pop("nom_cap", None)
-
-        if not file_name:
-            if frame is not None:
-                self.experiment.journal.from_frame(frame, **kwargs)
-            else:
-                if len(args) > 0:
-                    self.experiment.journal.name = args[0]
-
-                if len(args) > 1:
-                    self.experiment.journal.project = args[1]
-
-                for key in kwargs:
-                    if key == "name":
-                        self.experiment.journal.name = kwargs[key]
-                    elif key == "project":
-                        self.experiment.journal.project = kwargs[key]
-                    elif key == "batch_col":
-                        self.experiment.journal.batch_col = kwargs[key]
-        else:
-            self.experiment.journal.from_file(file_name=file_name, **kwargs)
-
-        self.exporter = CSVExporter()
-        self.exporter._assign_dumper(ram_dumper)
-        self.exporter.assign(self.experiment)
-
-        self.summary_collector = BaseSummaryAnalyzer()
-        self.summary_collector.assign(self.experiment)
-
-        self.plotter = CyclingSummaryPlotter()
-        self.plotter.assign(self.experiment)
-        self._journal_name = self.journal_name
-        self.headers_step_table = headers_step_table
-
-    def __str__(self):
-        return str(self.experiment)
-
-    def _repr_html_(self):
-        txt = f"<h2>Batch-object</h2> id={hex(id(self))}"
-        txt += f"<h3>batch.journal</h3>"
-        txt += f"<blockquote>{self.journal._repr_html_()}</blockquote>"
-        txt += f"<h3>batch.experiment</h3>"
-        txt += f"<blockquote>{self.experiment._repr_html_()}</blockquote>"
-
-        return txt
-
-    def __len__(self):
-        return len(self.experiment)
-
-    def __iter__(self):
-        return self.experiment.__iter__()
-
-    def show_pages(self, number_of_rows=5):
-        warnings.warn("Deprecated - use pages.head() instead", DeprecationWarning)
-        return self.experiment.journal.pages.head(number_of_rows)
-
-    @property
-    def view(self):
-        warnings.warn("Deprecated - use report instead", DeprecationWarning)
-        pages = self.experiment.journal.pages
-        pages = pages[COLUMNS_SELECTED_FOR_VIEW]
-        return pages
-
-    @property
-    def name(self):
-        return self.experiment.journal.name
-
-    def _check_cell_raw(self, cell_id):
-        try:
-            c = self.experiment.data[cell_id]
-            return len(c.data.raw)
-        except Exception as e:
-            logging.debug(f"Exception ignored: {e}")
-            return None
-
-    def _check_cell_steps(self, cell_id):
-        try:
-            c = self.experiment.data[cell_id]
-            return len(c.data.steps)
-        except Exception as e:
-            logging.debug(f"Exception ignored: {e}")
-            return None
-
-    def _check_cell_summary(self, cell_id):
-        try:
-            c = self.experiment.data[cell_id]
-            return len(c.data.summary)
-        except Exception as e:
-            logging.debug(f"Exception ignored: {e}")
-            return None
-
-    def _check_cell_max_cap(self, cell_id):
-        try:
-            c = self.experiment.data[cell_id]
-            s = c.data.summary
-            return s[headers_summary["charge_capacity_gravimetric"]].max()
-
-        except Exception as e:
-            logging.debug(f"Exception ignored: {e}")
-            return None
-
-    def _check_cell_min_cap(self, cell_id):
-        try:
-            c = self.experiment.data[cell_id]
-            s = c.data.summary
-            return s[headers_summary["charge_capacity_gravimetric"]].min()
-
-        except Exception as e:
-            logging.debug(f"Exception ignored: {e}")
-            return None
-
-    def _check_cell_avg_cap(self, cell_id):
-        try:
-            c = self.experiment.data[cell_id]
-            s = c.data.summary
-            return s[headers_summary["charge_capacity_gravimetric"]].mean()
-
-        except Exception as e:
-            logging.debug(f"Exception ignored: {e}")
-            return None
-
-    def _check_cell_std_cap(self, cell_id):
-        try:
-            c = self.experiment.data[cell_id]
-            s = c.data.summary
-            return s[headers_summary["charge_capacity_gravimetric"]].std()
-
-        except Exception as e:
-            logging.debug(f"Exception ignored: {e}")
-            return None
-
-    def _check_cell_empty(self, cell_id):
-        try:
-            c = self.experiment.data[cell_id]
-            return c.empty
-        except Exception as e:
-            logging.debug(f"Exception ignored: {e}")
-            return None
-
-    def _check_cell_cycles(self, cell_id):
-        try:
-            c = self.experiment.data[cell_id]
-            return c.data.steps[self.headers_step_table.cycle].max()
-        except Exception as e:
-            logging.debug(f"Exception ignored: {e}")
-            return None
-
-    def drop(self, cell_label=None):
-        """Drop cells from the journal.
-
-        If ``cell_label`` is not given, ``cellpy`` will look into the journal for session
-        info about bad cells, and if it finds it, it will remove those from the
-        journal.
-
-        Note! remember to save your journal again after modifying it.
-
-        Note! this method has not been properly tested yet.
-
-        Args:
-            cell_label (str): the cell label of the cell you would like to remove.
-
-        Returns:
-            ``cellpy.utils.batch`` object (returns a copy if `keep_old` is ``True``).
-
-        """
-        if cell_label is None:
-            try:
-                cell_labels = self.journal.session["bad_cells"]
-            except AttributeError:
-                logging.critical(
-                    "session info about bad cells is missing - cannot drop"
-                )
-                return
-        else:
-            cell_labels = [cell_label]
-
-        for cell_label in cell_labels:
-            if cell_label not in self.pages.index:
-                logging.critical(f"could not find {cell_label}")
-            else:
-                self.pages = self.pages.drop(cell_label)
-
-    def report(self, stylize=True):
-        """Create a report on all the cells in the batch object.
-
-        Remark! To perform a reporting, cellpy needs to access all the data (and it might take some time).
-
-        Returns:
-            ``pandas.DataFrame``
-        """
-        pages = self.experiment.journal.pages
-        pages = pages[COLUMNS_SELECTED_FOR_VIEW].copy()
-        # pages["empty"] = pages.index.map(self._check_cell_empty)
-        pages["raw_rows"] = pages.index.map(self._check_cell_raw)
-        pages["steps_rows"] = pages.index.map(self._check_cell_steps)
-        pages["summary_rows"] = pages.index.map(self._check_cell_summary)
-        pages["last_cycle"] = pages.index.map(self._check_cell_cycles)
-        pages["average_capacity"] = pages.index.map(self._check_cell_avg_cap)
-        pages["max_capacity"] = pages.index.map(self._check_cell_max_cap)
-        pages["min_capacity"] = pages.index.map(self._check_cell_min_cap)
-        pages["std_capacity"] = pages.index.map(self._check_cell_std_cap)
-
-        avg_last_cycle = pages.last_cycle.mean()
-        avg_max_capacity = pages.max_capacity.mean()
-
-        if stylize:
-
-            def highlight_outlier(s):
-                average = s.mean()
-                outlier = (s < average / 2) | (s > 2 * average)
-                return ["background-color: #f09223" if v else "" for v in outlier]
-
-            def highlight_small(s):
-                average = s.mean()
-                outlier = s < average / 4
-                return ["background-color: #41A1D8" if v else "" for v in outlier]
-
-            def highlight_very_small(s):
-                outlier = s <= 3
-                return ["background-color: #416CD8" if v else "" for v in outlier]
-
-            def highlight_big(s):
-                average = s.mean()
-                outlier = s > 2 * average
-                return ["background-color: #D85F41" if v else "" for v in outlier]
-
-            styled_pages = (
-                pages.style.apply(highlight_small, subset=["last_cycle"])
-                .apply(
-                    highlight_outlier,
-                    subset=["min_capacity", "max_capacity", "average_capacity"],
-                )
-                .apply(
-                    highlight_big,
-                    subset=["min_capacity", "max_capacity", "average_capacity"],
-                )
-                .apply(
-                    highlight_very_small,
-                    subset=["max_capacity", "average_capacity", "last_cycle"],
-                )
-                # .format({'min_capacity': "{:.2f}",
-                #        'max_capacity': "{:.2f}",
-                #        'average_capacity': "{:.2f}",
-                #        'std_capacity': '{:.2f}'})
-            )
-            pages = styled_pages
-
-        return pages
-
-    @property
-    def info_file(self):
-        # renamed to journal_name
-        warnings.warn("Deprecated - use journal_name instead", DeprecationWarning)
-        return self.experiment.journal.file_name
-
-    @property
-    def journal_name(self):
-        return self.experiment.journal.file_name
-
-    def _concat_memory_dumped(self, engine_name):
-        keys = [df.name for df in self.experiment.memory_dumped[engine_name]]
-        return pd.concat(self.experiment.memory_dumped[engine_name], keys=keys, axis=1)
-
-    @property
-    def summaries(self):
-        """Concatenated summaries from all cells (multiindex dataframe)."""
-        try:
-            return self._concat_memory_dumped("summary_engine")
-        except KeyError:
-            logging.critical("no summaries exists (dumping to ram first)")
-            self.summary_collector.do()
-            return self._concat_memory_dumped("summary_engine")
-
-    @property
-    def summary_headers(self):
-        """The column names of the concatenated summaries"""
-        try:
-            return self.summaries.columns.get_level_values(0)
-        except AttributeError:
-            logging.info("can't get any columns")
-
-    @property
-    def cell_names(self) -> list:
-        return self.experiment.cell_names
-
-    @property
-    def labels(self):
-        # Plan: allow cells to both have a label and a cell_name, where that latter should be a unique
-        # identifier. Consider also to allow for a group-name.
-        # The label and cell name can be the same. Consider allowing several cells to share the same label
-        # thus returning several cellpy cell objects. Our use "group" for this purpose.
-        print(
-            "Label-based look-up is not supported yet. Performing cell-name based look-up instead."
-        )
-        return self.experiment.cell_names
-
-    @property
-    def cells(self) -> Data:
-        """Access cells as a Data object (attribute lookup and automatic loading)
-
-        Usage (at least in jupyter notebook):
-            Write `b.cells.x` and press <TAB>. Then a pop-up will appear, and you can choose the
-            cell you would like to retrieve.
-        """
-        return self.experiment.data
-
-    @property
-    def cell_summary_headers(self) -> Index:
-        return self.experiment.data[self.experiment.cell_names[0]].data.summary.columns
-
-    @property
-    def cell_raw_headers(self) -> Index:
-        return self.experiment.data[self.experiment.cell_names[0]].data.raw.columns
-
-    @property
-    def cell_step_headers(self) -> Index:
-        return self.experiment.data[self.experiment.cell_names[0]].data.steps.columns
-
-    @property
-    def pages(self) -> pd.DataFrame:
-        return self.experiment.journal.pages
-
-    @pages.setter
-    def pages(self, df: pd.DataFrame):
-        self.experiment.journal.pages = df
-        all_cell_labels = set(self.experiment.cell_data_frames.keys())
-        cell_labels_to_keep = set(self.journal.pages.index)
-        cell_labels_to_remove = all_cell_labels - cell_labels_to_keep
-        for cell_label in cell_labels_to_remove:
-            del self.experiment.cell_data_frames[cell_label]
-
-    @property
-    def journal(self) -> LabJournal:
-        return self.experiment.journal
-
-    @journal.setter
-    def journal(self, new):
-        # self.experiment.journal = new
-        raise NotImplementedError(
-            "Setting a new journal object directly on a "
-            "batch object is not allowed at the moment. Try modifying "
-            "the journal.pages instead."
-        )
-
-    def old_duplicate_journal(self, folder=None) -> None:
-        """Copy the journal to folder.
-
-        Args:
-            folder (str or pathlib.Path): folder to copy to (defaults to the
-            current folder).
-        """
-
-        logging.debug(f"duplicating journal to folder {folder}")
-        journal_name = pathlib.Path(self.experiment.journal.file_name)
-        if not journal_name.is_file():
-            logging.info("No journal saved")
-            return
-        new_journal_name = journal_name.name
-        if folder is not None:
-            new_journal_name = pathlib.Path(folder) / new_journal_name
-        try:
-            shutil.copy(journal_name, new_journal_name)
-        except shutil.SameFileError:
-            logging.debug("same file exception encountered")
-
-    def duplicate_journal(self, folder=None) -> None:
-        """Copy the journal to folder.
-
-        Args:
-            folder (str or pathlib.Path): folder to copy to (defaults to the
-            current folder).
-        """
-        self.experiment.journal.duplicate_journal(folder)
-        #
-        # logging.debug(f"duplicating journal to folder {folder}")
-        # journal_name = pathlib.Path(self.experiment.journal.file_name)
-        # if not journal_name.is_file():
-        #     logging.info("No journal saved")
-        #     return
-        # new_journal_name = journal_name.name
-        # if folder is not None:
-        #     new_journal_name = pathlib.Path(folder) / new_journal_name
-        # try:
-        #     shutil.copy(journal_name, new_journal_name)
-        # except shutil.SameFileError:
-        #     logging.debug("same file exception encountered")
-
-    def create_journal(self, description=None, from_db=True, **kwargs):
-        """Create journal pages.
-
-            This method is a wrapper for the different Journal methods for making
-            journal pages (Batch.experiment.journal.xxx). It is under development. If you
-            want to use 'advanced' options (i.e. not loading from a db), please consider
-            using the methods available in Journal for now.
-
-            Args:
-                description: the information and meta-data needed to generate the journal pages ('empty': create an
-                    empty journal; ``dict``: create journal pages from a dictionary; ``pd.DataFrame``: create journal pages
-                    from a ``pandas.DataFrame``: 'filename.json': load cellpy batch file; 'filename.xlsx': create journal
-                    pages from an Excel file).
-                from_db (bool): Deprecation Warning: this parameter will be removed as it is
-                    the default anyway. Generate the pages from a db (the default option).
-                    This will be over-ridden if description is given.
-
-                **kwargs: sent to sub-function(s) (*e.g.* from_db -> simple_db_reader -> find_files ->
-                    filefinder.search_for_files).
-
-            kwargs -> from_db:
-                project=None, name=None, batch_col=None
-
-
-            kwargs -> simple_db_reader:
-                reader: a reader object (defaults to dbreader.Reader)
-                cell_ids: keys (cell IDs)
-                file_list: file list to send to filefinder (instead of searching in folders for files).
-                pre_path: prepended path to send to filefinder.
-                include_key: include the key col in the pages (the cell IDs).
-                include_individual_arguments: include the argument column in the pages.
-                additional_column_names: list of additional column names to include in the pages.
-
-            kwargs -> filefinder.search_for_files:
-                run_name(str): run-file identification.
-                raw_extension(str): optional, extension of run-files (without the '.').
-                cellpy_file_extension(str): optional, extension for cellpy files
-                    (without the '.').
-                raw_file_dir(path): optional, directory where to look for run-files
-                    (default: read prm-file)
-                cellpy_file_dir(path): optional, directory where to look for
-                    cellpy-files (default: read prm-file)
-                prm_filename(path): optional parameter file can be given.
-                file_name_format(str): format of raw-file names or a glob pattern
-                    (default: YYYYMMDD_[name]EEE_CC_TT_RR).
-                reg_exp(str): use regular expression instead (defaults to None).
-                sub_folders (bool): perform search also in sub-folders.
-                file_list (list of str): perform the search within a given list
-                    of filenames instead of searching the folder(s). The list should
-                    not contain the full filepath (only the actual file names). If
-                    you want to provide the full path, you will have to modify the
-                    file_name_format or reg_exp accordingly.
-                pre_path (path or str): path to prepend the list of files selected
-                     from the file_list.
-            kwargs -> journal.to_file:
-                duplicate_to_local_folder (bool): default True.
-
-
-        Returns:
-            info_dict
-
-        """
-
-        # TODO (jepe): create option to update journal without looking for files
-
-        logging.debug("Creating a journal")
-        logging.debug(f"description: {description}")
-        logging.debug(f"from_db: {from_db}")
-        logging.info(f"name: {self.experiment.journal.name}")
-        logging.info(f"project: {self.experiment.journal.project}")
-        to_project_folder = kwargs.pop("to_project_folder", True)
-        duplicate_to_local_folder = kwargs.pop("duplicate_to_local_folder", True)
-
-        if description is not None:
-            from_db = False
-        else:
-            if self.experiment.journal.pages is not None:
-                warnings.warn(
-                    "You created a journal - but you already have a "
-                    "journal. Hope you know what you are doing!"
-                )
-
-        if from_db:
-            self.experiment.journal.from_db(**kwargs)
-            self.experiment.journal.to_file(
-                duplicate_to_local_folder=duplicate_to_local_folder
-            )
-
-            # TODO: remove these:
-            if duplicate_to_local_folder:
-                self.experiment.journal.duplicate_journal()
-            if to_project_folder:
-                self.duplicate_journal(prms.Paths.batchfiledir)
-
-        else:
-            is_str = isinstance(description, str)
-            is_file = False
-
-            if is_str and pathlib.Path(description).is_file():
-                description = pathlib.Path(description)
-                is_file = True
-
-            if isinstance(description, pathlib.Path):
-                logging.debug("pathlib.Path object given")
-                is_file = True
-
-            if is_file:
-                logging.info(f"loading file {description}")
-                if description.suffix in [".json", ".xlsx"]:
-                    self.experiment.journal.from_file(description)
-                else:
-                    warnings.warn("unknown file extension")
-
-            else:
-                if is_str and description.lower() == "empty":
-                    logging.debug("creating empty journal pages")
-
-                    self.experiment.journal.pages = (
-                        self.experiment.journal.create_empty_pages()
-                    )
-
-                elif isinstance(description, pd.DataFrame):
-                    logging.debug("pandas DataFrame given")
-
-                    p = self.experiment.journal.create_empty_pages()
-                    columns = p.columns
-
-                    for column in columns:
-                        try:
-                            p[column] = description[column]
-                        except KeyError:
-                            logging.debug(f"missing key: {column}")
-
-                    # checking if filenames is a column
-                    if "filenames" in description.columns:
-                        indexes = description["filenames"]
-                    else:
-                        indexes = description.index
-
-                    p.index = indexes
-                    self.experiment.journal.pages = p
-
-                elif isinstance(description, dict):
-                    logging.debug("dictionary given")
-                    self.experiment.journal.pages = (
-                        self.experiment.journal.create_empty_pages()
-                    )
-                    for k in self.experiment.journal.pages.columns:
-                        try:
-                            value = description[k]
-                        except KeyError:
-                            warnings.warn(f"missing key: {k}")
-                        else:
-                            if not isinstance(value, list):
-                                warnings.warn("encountered item that is not a list")
-                                logging.debug(f"converting '{k}' to list-type")
-                                value = [value]
-                            if k == "raw_file_names":
-                                if not isinstance(value[0], list):
-                                    warnings.warn(
-                                        "encountered raw file description"
-                                        "that is not of list-type"
-                                    )
-                                    logging.debug(
-                                        "converting raw file description to a"
-                                        "list of lists"
-                                    )
-                                    value = [value]
-                            self.experiment.journal.pages[k] = value
-
-                    try:
-                        value = description["filenames"]
-                        if not isinstance(value, list):
-                            warnings.warn("encountered item that is not a list")
-                            logging.debug(f"converting '{k}' to list-type")
-                            value = [value]
-                        self.experiment.journal.pages.index = value
-                    except KeyError:
-                        logging.debug("could not interpret the index")
-
-                else:
-                    logging.debug(
-                        "the option you provided seems to be either of "
-                        "an unknown type or a file not found"
-                    )
-                    logging.info(
-                        "did not understand the option - creating empty journal pages"
-                    )
-
-            # finally
-            self.experiment.journal.to_file(
-                duplicate_to_local_folder=duplicate_to_local_folder
-            )
-            self.experiment.journal.generate_folder_names()
-            self.experiment.journal.paginate()
-            self.duplicate_journal(prms.Paths.batchfiledir)
-
-    def create_folder_structure(self) -> None:
-        warnings.warn("Deprecated - use paginate instead.", DeprecationWarning)
-        self.experiment.journal.paginate()
-        logging.info("created folders")
-
-    def paginate(self) -> None:
-        """Create the folders where cellpy will put its output."""
-
-        self.experiment.journal.paginate()
-        logging.info("created folders")
-
-    def save_journal(self) -> None:
-        """Save the journal (json-format).
-
-        The journal file will be saved in the project directory and in the
-        batch-file-directory (prms.Paths.batchfiledir). The latter is useful
-        for processing several batches using the iterate_batches functionality.
-        """
-
-        # Remark! Got an recursive error when running on mac.
-        self.experiment.journal.to_file(to_project_folder=True, paginate=False)
-        logging.info("saved journal pages to project folder")
-        self.duplicate_journal(prms.Paths.batchfiledir)
-        logging.info("duplicated journal pages to batch dir")
-        self.duplicate_journal()
-        logging.info("duplicated journal pages to current dir")
-
-    def export_journal(self, filename=None) -> None:
-        """Export the journal to xlsx."""
-        if filename is None:
-            filename = self.experiment.journal.file_name
-        filename = pathlib.Path(filename).with_suffix(".xlsx")
-        self.experiment.journal.to_file(
-            file_name=filename, to_project_folder=False, paginate=False
-        )
-
-    def duplicate_cellpy_files(
-        self, location: str = "standard", selector: dict = None, **kwargs
-    ) -> None:
-        """Copy the cellpy files and make a journal with the new names available in
-        the current folder.
-
-        Args:
-            location: where to copy the files. Either choose among the following
-                options:
-                "standard": data/interim folder
-                "here": current directory
-                "cellpydatadir": the stated cellpy data dir in your settings (prms)
-            or if the location is not one of the above, use the actual value of the
-                location argument.
-            selector (dict): if given, the cellpy files are reloaded after duplicating and
-                modified based on the given selector(s).
-
-            kwargs: sent to update if selector is provided
-
-        Returns:
-            The updated journal pages.
-        """
-
-        pages = self.experiment.journal.pages
-        cellpy_file_dir = OtherPath(prms.Paths.cellpydatadir)
-
-        if location == "standard":
-            batch_data_dir = pathlib.Path("data") / "interim"
-
-        elif location == "here":
-            batch_data_dir = pathlib.Path(".")
-
-        elif location == "cellpydatadir":
-            batch_data_dir = cellpy_file_dir
-
-        else:
-            batch_data_dir = location
-
-        def _new_file_path(x):
-            return str(batch_data_dir / pathlib.Path(x).name)
-
-        # update the journal pages
-        columns = pages.columns
-        pages["new_cellpy_file_name"] = pages.cellpy_file_name.apply(_new_file_path)
-
-        # copy the cellpy files
-        for n, row in pages.iterrows():
-            logging.info(f"{row.cellpy_file_name} -> {row.new_cellpy_file_name}")
-            try:
-                from_file = row.cellpy_file_name
-                to_file = row.new_cellpy_file_name
-                os.makedirs(os.path.dirname(to_file), exist_ok=True)
-                shutil.copy(from_file, to_file)
-            except shutil.SameFileError:
-                logging.info("Same file! No point in copying")
-            except FileNotFoundError:
-                logging.info("File not found! Cannot copy it!")
-
-        # save the journal pages
-        pages["cellpy_file_name"] = pages["new_cellpy_file_name"]
-        self.experiment.journal.pages = pages[columns]
-        journal_file_name = pathlib.Path(self.experiment.journal.file_name).name
-        self.experiment.journal.to_file(
-            journal_file_name, paginate=False, to_project_folder=False
-        )
-        if selector is not None:
-            logging.info("Modifying the cellpy-files.")
-            logging.info(f"selector: {selector}")
-            self.experiment.force_cellpy = True
-            self.update(selector=selector, **kwargs)
-
-    # TODO: list_journals?
-
-    def link(self, max_cycle=None, force_combine_summaries=False) -> None:
-        """Link journal content to the cellpy-files and load the step information.
-
-        Args:
-            max_cycle (int): set maximum cycle number to link to.
-            force_combine_summaries (bool): automatically run combine_summaries (set this to True
-                if you are re-linking without max_cycle for a batch that previously were linked
-                with max_cycle)
-
-        """
-
-        self.experiment.link(max_cycle=max_cycle)
-        if force_combine_summaries or max_cycle:
-            self.summary_collector.do(reset=True)
-
-    def load(self) -> None:
-        # does the same as update
-        warnings.warn("Deprecated - use update instead.", DeprecationWarning)
-        self.experiment.update()
-
-    def update(self, pool=False, **kwargs) -> None:
-        """Updates the selected datasets.
-
-        Keyword Args (to experiment-instance):
-            all_in_memory (bool): store the `cellpydata` in memory (default
-                False)
-            cell_specs (dict of dicts): individual arguments pr. cell. The `cellspecs` key-word argument
-                dictionary will override the **kwargs and the parameters from the journal pages
-                for the indicated cell.
-
-        Additional kwargs:
-            transferred all the way to the instrument loader, if not
-            picked up earlier. Remark that you can obtain the same pr. cell by
-            providing a `cellspecs` dictionary. The kwargs have precedence over the
-            parameters given in the journal pages, but will be overridden by parameters
-            given by `cellspecs`.
-
-            Merging:
-                recalc (Bool): set to False if you don't want automatic "recalc" of
-                    cycle numbers etc. when merging several data-sets.
-            Loading:
-                selector (dict): selector-based parameters sent to the cellpy-file loader (hdf5) if
-                loading from raw is not necessary (or turned off).
-
-        """
-        self.experiment.errors["update"] = []
-        if pool:
-            self.experiment.parallel_update(**kwargs)
-        else:
-            self.experiment.update(**kwargs)
-
-    def export_cellpy_files(self, path=None, **kwargs) -> None:
-        if path is None:
-            path = pathlib.Path(".").resolve()
-        self.experiment.errors["export_cellpy_files"] = []
-        self.experiment.export_cellpy_files(path=path, **kwargs)
-
-    def recalc(self, **kwargs) -> None:
-        """Run make_step_table and make_summary on all cells.
-
-        Keyword Args:
-            save (bool): Save updated cellpy-files if True (defaults to True).
-            step_opts (dict): parameters to inject to make_steps (defaults to None).
-            summary_opts (dict): parameters to inject to make_summary (defaults to None).
-            indexes (list): Only recalculate for given indexes (i.e. list of cell-names) (defaults to None).
-            calc_steps (bool): Run make_steps before making the summary (defaults to True).
-            testing (bool): Only for testing purposes (defaults to False).
-
-        Returns:
-            None
-        """
-        self.experiment.errors["recalc"] = []
-        self.experiment.recalc(**kwargs)
-
-    def make_summaries(self) -> None:
-        warnings.warn("Deprecated - use combine_summaries instead.", DeprecationWarning)
-
-        self.exporter.do()
-
-    def combine_summaries(self, export_to_csv=True, **kwargs) -> None:
-        """Combine selected columns from each of the cells into single frames"""
-
-        if export_to_csv:
-            self.exporter.do()
-        else:
-            self.summary_collector.do(**kwargs)
-
-    def plot_summaries(
-        self, output_filename=None, backend=None, reload_data=False, **kwargs
-    ) -> None:
-        """Plot the summaries"""
-
-        if reload_data or ("summary_engine" not in self.experiment.memory_dumped):
-            logging.debug("running summary_collector")
-            self.summary_collector.do(reset=True)
-
-        if backend is None:
-            backend = prms.Batch.backend
-
-        if backend in ["bokeh", "matplotlib"]:
-            prms.Batch.backend = backend
-
-        if backend == "bokeh":
-            try:
-                import bokeh.plotting
-
-                prms.Batch.backend = "bokeh"
-
-                if output_filename is not None:
-                    bokeh.plotting.output_file(output_filename)
-                else:
-                    if prms.Batch.notebook:
-                        bokeh.plotting.output_notebook()
-
-            except ModuleNotFoundError:
-                prms.Batch.backend = "matplotlib"
-                logging.warning(
-                    "could not find the bokeh module -> using matplotlib instead"
-                )
-
-        self.plotter.do(**kwargs)
-
-
-def init(*args, **kwargs) -> Batch:
-    """Returns an initialized instance of the Batch class.
-
-    Args:
-        *args: passed directly to Batch()
-            **name**: name of batch;
-            **project**: name of project;
-            **batch_col**: batch column identifier.
-        **kwargs:
-            **file_name**: json file if loading from pages;
-            **default_log_level**: "INFO" or "DEBUG";
-            the rest is passed directly to Batch().
-
-    Examples:
-        >>> empty_batch = Batch.init(db_reader=None)
-        >>> batch_from_file = Batch.init(file_name="cellpy_batch_my_experiment.json")
-        >>> normal_init_of_batch = Batch.init()
-    """
-    # TODO: add option for setting max cycle number (experiment.last_cycle)
-    # set up cellpy logger
-    default_log_level = kwargs.pop("default_log_level", None)
-    testing = kwargs.pop("testing", False)
-    file_name = kwargs.pop("file_name", None)
-    frame = kwargs.pop("frame", None)
-    log.setup_logging(
-        default_level=default_log_level, testing=testing, reset_big_log=True
-    )
-
-    logging.debug(f"returning Batch(kwargs: {kwargs})")
-    if file_name is not None:
-        kwargs.pop("db_reader", None)
-        return Batch(*args, file_name=file_name, db_reader=None, **kwargs)
-    if frame is not None:
-        kwargs.pop("db_reader", None)
-        return Batch(*args, file_name=None, db_reader=None, frame=frame, **kwargs)
-
-    return Batch(*args, **kwargs)
-
-
-def from_journal(journal_file, autolink=True, testing=False) -> Batch:
-    """Create a Batch from a journal file"""
-    # TODO: add option for setting max cycle number (experiment.last_cycle)
-    b = init(db_reader=None, file_name=journal_file, testing=testing)
-    if autolink:
-        b.link()
-    return b
-
-
-def load_pages(file_name) -> pd.DataFrame:
-    """Retrieve pages from a Journal file.
-
-    This function is here to let you easily inspect a Journal file without
-    starting up the full batch-functionality.
-
-    Examples:
-        >>> from cellpy.utils import batch
-        >>> journal_file_name = 'cellpy_journal_one.json'
-        >>> pages = batch.load_pages(journal_file_name)
-
-    Returns:
-        pandas.DataFrame
-
-    """
-
-    logging.info(f"Loading pages from {file_name}")
-    try:
-        pages, *_ = LabJournal.read_journal_jason_file(file_name)
-        return pages
-    except cellpy.exceptions.UnderDefined:
-        logging.critical("could not find any pages.")
-
-
-def process_batch(*args, **kwargs) -> Batch:
-    """Execute a batch run, either from a given file_name or by giving the name and project as input.
-
-    Examples:
-        >>> process_batch(file_name | (name, project), **kwargs)
-
-    Args:
-        *args: file_name or name and project (both string)
-
-    Keyword Args:
-        backend (str): what backend to use when plotting ('bokeh' or 'matplotlib').
-            Defaults to 'matplotlib'.
-        dpi (int): resolution used when saving matplotlib plot(s). Defaults to 300 dpi.
-        default_log_level (str): What log-level to use for console output. Chose between
-            'CRITICAL', 'DEBUG', or 'INFO'. The default is 'CRITICAL' (i.e. usually no log output to console).
-
-    Returns:
-        ``cellpy.batch.Batch`` object
-    """
-    silent = kwargs.pop("silent", False)
-    backend = kwargs.pop("backend", None)
-
-    if backend is not None:
-        prms.Batch.backend = backend
-    else:
-        prms.Batch.backend = "matplotlib"
-
-    dpi = kwargs.pop("dpi", 300)
-
-    default_log_level = kwargs.pop("default_log_level", "CRITICAL")
-    if len(args) == 1:
-        file_name = args[0]
-    else:
-        file_name = kwargs.pop("file_name", None)
-    testing = kwargs.pop("testing", False)
-    log.setup_logging(
-        default_level=default_log_level, reset_big_log=True, testing=testing
-    )
-    logging.debug(f"creating Batch(kwargs: {kwargs})")
-
-    if file_name is not None:
-        kwargs.pop("db_reader", None)
-        b = Batch(*args, file_name=file_name, db_reader=None, **kwargs)
-        b.create_journal(file_name)
-    else:
-        b = Batch(*args, **kwargs)
-        b.create_journal()
-
-    steps = {
-        "paginate": (b.paginate,),
-        "update": (b.update,),
-        "combine": (b.combine_summaries,),
-        "plot": (b.plot_summaries,),
-        "save": (_pb_save_plot, b, dpi),
-    }
-
-    with tqdm(total=(100 * len(steps) + 20), leave=False, file=sys.stdout) as pbar:
-        pbar.update(10)
-        for description in steps:
-            func, *args = steps[description]
-            pbar.set_description(description)
-            pbar.update(10)
-            try:
-                func(*args)
-            except cellpy.exceptions.NullData as e:
-                if not silent:
-                    tqdm.write(f"\nEXCEPTION (NullData): {str(e)}")
-                    tqdm.write("...aborting")
-                    return
-                else:
-                    raise e
-
-        pbar.set_description(f"final")
-        pbar.update(10)
-
-    return b
-
-
-def _pb_save_plot(b, dpi):
-    name = b.experiment.journal.name
-    out_dir = pathlib.Path(b.experiment.journal.batch_dir)
-
-    for n, farm in enumerate(b.plotter.farms):
-        if len(b.plotter.farms) > 1:
-            file_name = f"summary_plot_{name}_{str(n + 1).zfill(3)}.png"
-        else:
-            file_name = f"summary_plot_{name}.png"
-        out = out_dir / file_name
-        logging.info(f"saving file {file_name} in\n{out}")
-        farm.savefig(out, dpi=dpi)
-    # and other stuff
-
-
-def iterate_batches(folder, extension=".json", glob_pattern=None, **kwargs):
-    """Iterate through all journals in given folder.
-
-    Args:
-        folder (str or pathlib.Path): folder containing the journal files.
-        extension (str): extension for the journal files (used when creating a default glob-pattern).
-        glob_pattern (str): optional glob pattern.
-        **kwargs: keyword arguments passed to ``batch.process_batch``.
-    """
-
-    folder = pathlib.Path(folder)
-    logging.info(f"Folder for batches to be iterated: {folder}")
-    if not folder.is_dir():
-        print(f"Could not find the folder ({folder})")
-        print("Aborting...")
-        logging.info("ABORTING - folder not found.")
-        return
-    print(" Iterating through the folder ".center(80, "="))
-    print(f"Folder name: {folder}")
-    if not glob_pattern:
-        glob_pattern = f"*{extension}"
-    print(f"Glob pattern: {glob_pattern}")
-    files = sorted(folder.glob(glob_pattern))
-    if not files:
-        print("No files found! Aborting...")
-        logging.info("ABORTING - no files detected.")
-        return
-    print("Found the following files:")
-    for n, file in enumerate(files):
-        logging.debug(f"file: {file}")
-        print(f"  {str(n).zfill(4)} - {file}")
-
-    print(" Processing ".center(80, "-"))
-    output = []
-    failed = []
-    with tqdm(files, file=sys.stdout) as pbar:
-        for n, file in enumerate(pbar):
-            output_str = f"[{str(n).zfill(4)}]"
-            pbar.set_description(output_str)
-            output_str += f"({file.name})"
-            logging.debug(f"processing file: {file.name}")
-            try:
-                process_batch(file, **kwargs)
-                output_str += " [OK]"
-                logging.debug(f"No errors detected.")
-            except Exception as e:
-                output_str += " [FAILED!]"
-                failed.append(str(file))
-                logging.debug("Error detected.")
-                logging.debug(e)
-
-            output.append(output_str)
-
-    print(" Result ".center(80, "-"))
-    print("\n".join(output))
-    if failed:
-        print("\nFailed:")
-        failed_txt = "\n".join(failed)
-        print(failed_txt)
-        logging.info(failed_txt)
-    print("\n...Finished ")
-
-
-def check_standard():
-    from pathlib import Path
-
-    # Use these when working on my work PC:
-    test_data_path = r"C:\Scripting\MyFiles\development_cellpy\testdata"
-    out_data_path = r"C:\Scripting\Processing\Test\out"
-
-    # Use these when working on my MacBook:
-    # test_data_path = "/Users/jepe/scripting/cellpy/testdata"
-    # out_data_path = "/Users/jepe/cellpy_data"
-
-    test_data_path = Path(test_data_path)
-    out_data_path = Path(out_data_path)
-
-    logging.info("---SETTING SOME PRMS---")
-    prms.Paths.db_filename = "cellpy_db.xlsx"
-    prms.Paths.cellpydatadir = test_data_path / "hdf5"
-    prms.Paths.outdatadir = out_data_path
-    prms.Paths.rawdatadir = test_data_path / "data"
-    prms.Paths.db_path = test_data_path / "db"
-    prms.Paths.filelogdir = test_data_path / "log"
-
-    project = "prebens_experiment"
-    name = "test"
-    batch_col = "b01"
-
-    logging.info("---INITIALISATION OF BATCH---")
-    b = init(name, project, batch_col=batch_col)
-    b.experiment.export_raw = True
-    b.experiment.export_cycles = True
-    logging.info("*creating info df*")
-    b.create_journal()
-    logging.info("*creating folder structure*")
-    b.paginate()
-    logging.info("*load and save*")
-    b.update()
-    logging.info("*make summaries*")
-    try:
-        b.combine_summaries()
-        summaries = b.experiment.memory_dumped
-    except cellpy.exeptions.NullData:
-        print("NO DATA")
-        return
-    # except cellpy.exceptions.NullData:
-    #     print("NOTHING")
-    #     return
-
-    logging.info("*plotting summaries*")
-    b.plot_summaries("tmp_bokeh_plot.html")
-
-    # logging.info("*using special features*")
-    # logging.info(" - select_ocv_points")
-    # analyzer = OCVRelaxationAnalyzer()
-    # analyzer.assign(b.experiment)
-    # analyzer.do()
-    # ocv_df_list = analyzer.farms[0]
-    # for df in ocv_df_list:
-    #     df_up = df.loc[df.type == "ocvrlx_up", :]
-    #     df_down = df.loc[df.type == "ocvrlx_down", :]
-    #     logging.info(df_up)
-    logging.info("---FINISHED---")
-
-
-def check_new():
-    use_db = False
-    f = r"C:\scripts\processing_cellpy\out\SecondLife\cellpy_batch_embla_002.json"
-    # f = r"C:\Scripting\Processing\Celldata\outdata\SilcRoad\cellpy_batch_uio66.json"
-    # f = r"C:\Scripting\Processing\Celldata\outdata\MoZEES\cellpy_batch_round_robin_001.json"
-    name = "embla_test"
-    project = "cellpy_test"
-    batch_col = "b02"
-    if use_db:
-        process_batch(name, project, batch_col=batch_col, nom_cap=372)
-    else:
-        # process_batch(f, nom_cap=372)
-        process_batch(f, force_raw_file=False, force_cellpy=True, nom_cap=372)
-
-
-# TODO: allow exporting html when processing batch instead of just png
-
-
-def check_iterate():
-    folder_name = r"C:\Scripting\Processing\Celldata\live"
-    iterate_batches(folder_name, export_cycles=False, export_raw=False)
-
-
-if __name__ == "__main__":
-    print("---IN BATCH 2 MAIN---")
-    check_new()
+"""Routines for batch processing of cells (v2)."""
+
+import logging
+import os
+import pathlib
+import shutil
+import sys
+import warnings
+
+import pandas as pd
+from pandas import Index
+from tqdm.auto import tqdm
+
+import cellpy.exceptions
+from cellpy import log, prms
+from cellpy.parameters.internal_settings import (
+    headers_journal,
+    headers_step_table,
+    headers_summary,
+)
+from cellpy.internals.core import OtherPath
+from cellpy.utils.batch_tools.batch_analyzers import (
+    BaseSummaryAnalyzer,
+    OCVRelaxationAnalyzer,
+)
+from cellpy.utils.batch_tools.batch_core import Data
+from cellpy.utils.batch_tools.batch_experiments import CyclingExperiment
+from cellpy.utils.batch_tools.batch_exporters import CSVExporter
+from cellpy.utils.batch_tools.batch_journals import LabJournal
+from cellpy.utils.batch_tools.batch_plotters import CyclingSummaryPlotter
+from cellpy.utils.batch_tools.dumpers import ram_dumper
+
+# logger = logging.getLogger(__name__)
+logging.captureWarnings(True)
+
+COLUMNS_SELECTED_FOR_VIEW = [
+    headers_journal.mass,
+    headers_journal.total_mass,
+    headers_journal.loading,
+    headers_journal.nom_cap,
+]
+
+
+class Batch:
+    """A convenient class for running batch procedures.
+
+    The Batch class contains among other things:
+        - iterator protocol
+        - a journal with info about the different cells where the
+        main information is accessible as a pandas.DataFrame through the `.pages` attribute
+        - a data lookup accessor `.data` that behaves similarly as a dict.
+    """
+
+    def __init__(self, *args, **kwargs):
+        """Initialize the Batch class.
+
+        The initialization accepts arbitrary arguments and keyword arguments.
+        It first looks for the file_name and db_reader keyword arguments.
+
+        Usage:
+            b = Batch((name, (project)), **kwargs)
+
+        Examples:
+            >>> b = Batch("experiment001", "main_project")
+            >>> b = Batch("experiment001", "main_project", batch_col="b02")
+            >>> b = Batch(name="experiment001", project="main_project", batch_col="b02")
+            >>> b = Batch(file_name="cellpydata/batchfiles/cellpy_batch_experiment001.json")
+
+        Keyword Args (priority):
+            file_name (str or pathlib.Path): journal file name to load.
+            db_reader (str): data-base reader to use (defaults to "default" as given
+                in the config-file or prm-class).
+            frame (pandas.DataFrame): load from given dataframe.
+        Args:
+            *args: name (str) (project (str))
+
+        Keyword Args (other):
+            default_log_level (str): custom log-level (defaults to None (i.e. default log-level in cellpy)).
+            custom_log_dir (str or pathlib.Path): custom folder for putting the log-files.
+            force_raw_file (bool): load from raw regardless (defaults to False).
+            force_cellpy (bool): load cellpy-files regardless (defaults to False).
+            force_recalc (bool): Always recalculate (defaults to False).
+            export_cycles (bool): Extract and export individual cycles to csv (defaults to True).
+            export_raw (bool): Extract and export raw-data to csv (defaults to True).
+            export_ica (bool): Extract and export individual dQ/dV data to csv (defaults to True).
+            accept_errors (bool): Continue automatically to next file if error is raised (defaults to False).
+            nom_cap (float): give a nominal capacity if you want to use another value than
+                the one given in the config-file or prm-class.
+        """
+        # TODO: add option for setting max cycle number
+        #   use self.experiment.last_cycle = xxx
+        default_log_level = kwargs.pop("default_log_level", None)
+        custom_log_dir = kwargs.pop("custom_log_dir", None)
+        if default_log_level is not None or custom_log_dir is not None:
+            log.setup_logging(
+                custom_log_dir=custom_log_dir,
+                default_level=default_log_level,
+                reset_big_log=True,
+            )
+
+        db_reader = kwargs.pop("db_reader", "default")
+
+        file_name = kwargs.pop("file_name", None)
+        frame = kwargs.pop("frame", None)
+
+        logging.debug("creating CyclingExperiment")
+        self.experiment = CyclingExperiment(db_reader=db_reader)
+        logging.info("created CyclingExperiment")
+
+        self.experiment.force_cellpy = kwargs.pop("force_cellpy", False)
+        self.experiment.force_raw = kwargs.pop("force_raw_file", False)
+        self.experiment.force_recalc = kwargs.pop("force_recalc", False)
+        self.experiment.export_cycles = kwargs.pop("export_cycles", True)
+        self.experiment.export_raw = kwargs.pop("export_raw", True)
+        self.experiment.export_ica = kwargs.pop("export_ica", False)
+        self.experiment.accept_errors = kwargs.pop("accept_errors", False)
+        self.experiment.nom_cap = kwargs.pop("nom_cap", None)
+
+        if not file_name:
+            if frame is not None:
+                self.experiment.journal.from_frame(frame, **kwargs)
+            else:
+                if len(args) > 0:
+                    self.experiment.journal.name = args[0]
+
+                if len(args) > 1:
+                    self.experiment.journal.project = args[1]
+
+                for key in kwargs:
+                    if key == "name":
+                        self.experiment.journal.name = kwargs[key]
+                    elif key == "project":
+                        self.experiment.journal.project = kwargs[key]
+                    elif key == "batch_col":
+                        self.experiment.journal.batch_col = kwargs[key]
+        else:
+            self.experiment.journal.from_file(file_name=file_name, **kwargs)
+
+        self.exporter = CSVExporter()
+        self.exporter._assign_dumper(ram_dumper)
+        self.exporter.assign(self.experiment)
+
+        self.summary_collector = BaseSummaryAnalyzer()
+        self.summary_collector.assign(self.experiment)
+
+        self.plotter = CyclingSummaryPlotter()
+        self.plotter.assign(self.experiment)
+        self._journal_name = self.journal_name
+        self.headers_step_table = headers_step_table
+
+    def __str__(self):
+        return str(self.experiment)
+
+    def _repr_html_(self):
+        txt = f"<h2>Batch-object</h2> id={hex(id(self))}"
+        txt += f"<h3>batch.journal</h3>"
+        txt += f"<blockquote>{self.journal._repr_html_()}</blockquote>"
+        txt += f"<h3>batch.experiment</h3>"
+        txt += f"<blockquote>{self.experiment._repr_html_()}</blockquote>"
+
+        return txt
+
+    def __len__(self):
+        return len(self.experiment)
+
+    def __iter__(self):
+        return self.experiment.__iter__()
+
+    def show_pages(self, number_of_rows=5):
+        warnings.warn("Deprecated - use pages.head() instead", DeprecationWarning)
+        return self.experiment.journal.pages.head(number_of_rows)
+
+    @property
+    def view(self):
+        warnings.warn("Deprecated - use report instead", DeprecationWarning)
+        pages = self.experiment.journal.pages
+        pages = pages[COLUMNS_SELECTED_FOR_VIEW]
+        return pages
+
+    @property
+    def name(self):
+        return self.experiment.journal.name
+
+    def _check_cell_raw(self, cell_id):
+        try:
+            c = self.experiment.data[cell_id]
+            return len(c.data.raw)
+        except Exception as e:
+            logging.debug(f"Exception ignored: {e}")
+            return None
+
+    def _check_cell_steps(self, cell_id):
+        try:
+            c = self.experiment.data[cell_id]
+            return len(c.data.steps)
+        except Exception as e:
+            logging.debug(f"Exception ignored: {e}")
+            return None
+
+    def _check_cell_summary(self, cell_id):
+        try:
+            c = self.experiment.data[cell_id]
+            return len(c.data.summary)
+        except Exception as e:
+            logging.debug(f"Exception ignored: {e}")
+            return None
+
+    def _check_cell_max_cap(self, cell_id):
+        try:
+            c = self.experiment.data[cell_id]
+            s = c.data.summary
+            return s[headers_summary["charge_capacity_gravimetric"]].max()
+
+        except Exception as e:
+            logging.debug(f"Exception ignored: {e}")
+            return None
+
+    def _check_cell_min_cap(self, cell_id):
+        try:
+            c = self.experiment.data[cell_id]
+            s = c.data.summary
+            return s[headers_summary["charge_capacity_gravimetric"]].min()
+
+        except Exception as e:
+            logging.debug(f"Exception ignored: {e}")
+            return None
+
+    def _check_cell_avg_cap(self, cell_id):
+        try:
+            c = self.experiment.data[cell_id]
+            s = c.data.summary
+            return s[headers_summary["charge_capacity_gravimetric"]].mean()
+
+        except Exception as e:
+            logging.debug(f"Exception ignored: {e}")
+            return None
+
+    def _check_cell_std_cap(self, cell_id):
+        try:
+            c = self.experiment.data[cell_id]
+            s = c.data.summary
+            return s[headers_summary["charge_capacity_gravimetric"]].std()
+
+        except Exception as e:
+            logging.debug(f"Exception ignored: {e}")
+            return None
+
+    def _check_cell_empty(self, cell_id):
+        try:
+            c = self.experiment.data[cell_id]
+            return c.empty
+        except Exception as e:
+            logging.debug(f"Exception ignored: {e}")
+            return None
+
+    def _check_cell_cycles(self, cell_id):
+        try:
+            c = self.experiment.data[cell_id]
+            return c.data.steps[self.headers_step_table.cycle].max()
+        except Exception as e:
+            logging.debug(f"Exception ignored: {e}")
+            return None
+
+    def drop(self, cell_label=None):
+        """Drop cells from the journal.
+
+        If ``cell_label`` is not given, ``cellpy`` will look into the journal for session
+        info about bad cells, and if it finds it, it will remove those from the
+        journal.
+
+        Note! remember to save your journal again after modifying it.
+
+        Note! this method has not been properly tested yet.
+
+        Args:
+            cell_label (str): the cell label of the cell you would like to remove.
+
+        Returns:
+            ``cellpy.utils.batch`` object (returns a copy if `keep_old` is ``True``).
+
+        """
+        if cell_label is None:
+            try:
+                cell_labels = self.journal.session["bad_cells"]
+            except AttributeError:
+                logging.critical(
+                    "session info about bad cells is missing - cannot drop"
+                )
+                return
+        else:
+            cell_labels = [cell_label]
+
+        for cell_label in cell_labels:
+            if cell_label not in self.pages.index:
+                logging.critical(f"could not find {cell_label}")
+            else:
+                self.pages = self.pages.drop(cell_label)
+
+    def report(self, stylize=True):
+        """Create a report on all the cells in the batch object.
+
+        Remark! To perform a reporting, cellpy needs to access all the data (and it might take some time).
+
+        Returns:
+            ``pandas.DataFrame``
+        """
+        pages = self.experiment.journal.pages
+        pages = pages[COLUMNS_SELECTED_FOR_VIEW].copy()
+        # pages["empty"] = pages.index.map(self._check_cell_empty)
+        pages["raw_rows"] = pages.index.map(self._check_cell_raw)
+        pages["steps_rows"] = pages.index.map(self._check_cell_steps)
+        pages["summary_rows"] = pages.index.map(self._check_cell_summary)
+        pages["last_cycle"] = pages.index.map(self._check_cell_cycles)
+        pages["average_capacity"] = pages.index.map(self._check_cell_avg_cap)
+        pages["max_capacity"] = pages.index.map(self._check_cell_max_cap)
+        pages["min_capacity"] = pages.index.map(self._check_cell_min_cap)
+        pages["std_capacity"] = pages.index.map(self._check_cell_std_cap)
+
+        avg_last_cycle = pages.last_cycle.mean()
+        avg_max_capacity = pages.max_capacity.mean()
+
+        if stylize:
+
+            def highlight_outlier(s):
+                average = s.mean()
+                outlier = (s < average / 2) | (s > 2 * average)
+                return ["background-color: #f09223" if v else "" for v in outlier]
+
+            def highlight_small(s):
+                average = s.mean()
+                outlier = s < average / 4
+                return ["background-color: #41A1D8" if v else "" for v in outlier]
+
+            def highlight_very_small(s):
+                outlier = s <= 3
+                return ["background-color: #416CD8" if v else "" for v in outlier]
+
+            def highlight_big(s):
+                average = s.mean()
+                outlier = s > 2 * average
+                return ["background-color: #D85F41" if v else "" for v in outlier]
+
+            styled_pages = (
+                pages.style.apply(highlight_small, subset=["last_cycle"])
+                .apply(
+                    highlight_outlier,
+                    subset=["min_capacity", "max_capacity", "average_capacity"],
+                )
+                .apply(
+                    highlight_big,
+                    subset=["min_capacity", "max_capacity", "average_capacity"],
+                )
+                .apply(
+                    highlight_very_small,
+                    subset=["max_capacity", "average_capacity", "last_cycle"],
+                )
+                # .format({'min_capacity': "{:.2f}",
+                #        'max_capacity': "{:.2f}",
+                #        'average_capacity': "{:.2f}",
+                #        'std_capacity': '{:.2f}'})
+            )
+            pages = styled_pages
+
+        return pages
+
+    @property
+    def info_file(self):
+        # renamed to journal_name
+        warnings.warn("Deprecated - use journal_name instead", DeprecationWarning)
+        return self.experiment.journal.file_name
+
+    @property
+    def journal_name(self):
+        return self.experiment.journal.file_name
+
+    def _concat_memory_dumped(self, engine_name):
+        keys = [df.name for df in self.experiment.memory_dumped[engine_name]]
+        return pd.concat(self.experiment.memory_dumped[engine_name], keys=keys, axis=1)
+
+    @property
+    def summaries(self):
+        """Concatenated summaries from all cells (multiindex dataframe)."""
+        try:
+            return self._concat_memory_dumped("summary_engine")
+        except KeyError:
+            logging.critical("no summaries exists (dumping to ram first)")
+            self.summary_collector.do()
+            return self._concat_memory_dumped("summary_engine")
+
+    @property
+    def summary_headers(self):
+        """The column names of the concatenated summaries"""
+        try:
+            return self.summaries.columns.get_level_values(0)
+        except AttributeError:
+            logging.info("can't get any columns")
+
+    @property
+    def cell_names(self) -> list:
+        return self.experiment.cell_names
+
+    @property
+    def labels(self):
+        # Plan: allow cells to both have a label and a cell_name, where that latter should be a unique
+        # identifier. Consider also to allow for a group-name.
+        # The label and cell name can be the same. Consider allowing several cells to share the same label
+        # thus returning several cellpy cell objects. Our use "group" for this purpose.
+        print(
+            "Label-based look-up is not supported yet. Performing cell-name based look-up instead."
+        )
+        return self.experiment.cell_names
+
+    @property
+    def cells(self) -> Data:
+        """Access cells as a Data object (attribute lookup and automatic loading)
+
+        Usage (at least in jupyter notebook):
+            Write `b.cells.x` and press <TAB>. Then a pop-up will appear, and you can choose the
+            cell you would like to retrieve.
+        """
+        return self.experiment.data
+
+    @property
+    def cell_summary_headers(self) -> Index:
+        return self.experiment.data[self.experiment.cell_names[0]].data.summary.columns
+
+    @property
+    def cell_raw_headers(self) -> Index:
+        return self.experiment.data[self.experiment.cell_names[0]].data.raw.columns
+
+    @property
+    def cell_step_headers(self) -> Index:
+        return self.experiment.data[self.experiment.cell_names[0]].data.steps.columns
+
+    @property
+    def pages(self) -> pd.DataFrame:
+        return self.experiment.journal.pages
+
+    @pages.setter
+    def pages(self, df: pd.DataFrame):
+        self.experiment.journal.pages = df
+        all_cell_labels = set(self.experiment.cell_data_frames.keys())
+        cell_labels_to_keep = set(self.journal.pages.index)
+        cell_labels_to_remove = all_cell_labels - cell_labels_to_keep
+        for cell_label in cell_labels_to_remove:
+            del self.experiment.cell_data_frames[cell_label]
+
+    @property
+    def journal(self) -> LabJournal:
+        return self.experiment.journal
+
+    @journal.setter
+    def journal(self, new):
+        # self.experiment.journal = new
+        raise NotImplementedError(
+            "Setting a new journal object directly on a "
+            "batch object is not allowed at the moment. Try modifying "
+            "the journal.pages instead."
+        )
+
+    def old_duplicate_journal(self, folder=None) -> None:
+        """Copy the journal to folder.
+
+        Args:
+            folder (str or pathlib.Path): folder to copy to (defaults to the
+            current folder).
+        """
+
+        logging.debug(f"duplicating journal to folder {folder}")
+        journal_name = pathlib.Path(self.experiment.journal.file_name)
+        if not journal_name.is_file():
+            logging.info("No journal saved")
+            return
+        new_journal_name = journal_name.name
+        if folder is not None:
+            new_journal_name = pathlib.Path(folder) / new_journal_name
+        try:
+            shutil.copy(journal_name, new_journal_name)
+        except shutil.SameFileError:
+            logging.debug("same file exception encountered")
+
+    def duplicate_journal(self, folder=None) -> None:
+        """Copy the journal to folder.
+
+        Args:
+            folder (str or pathlib.Path): folder to copy to (defaults to the
+            current folder).
+        """
+        self.experiment.journal.duplicate_journal(folder)
+        #
+        # logging.debug(f"duplicating journal to folder {folder}")
+        # journal_name = pathlib.Path(self.experiment.journal.file_name)
+        # if not journal_name.is_file():
+        #     logging.info("No journal saved")
+        #     return
+        # new_journal_name = journal_name.name
+        # if folder is not None:
+        #     new_journal_name = pathlib.Path(folder) / new_journal_name
+        # try:
+        #     shutil.copy(journal_name, new_journal_name)
+        # except shutil.SameFileError:
+        #     logging.debug("same file exception encountered")
+
+    def create_journal(self, description=None, from_db=True, **kwargs):
+        """Create journal pages.
+
+            This method is a wrapper for the different Journal methods for making
+            journal pages (Batch.experiment.journal.xxx). It is under development. If you
+            want to use 'advanced' options (i.e. not loading from a db), please consider
+            using the methods available in Journal for now.
+
+            Args:
+                description: the information and meta-data needed to generate the journal pages ('empty': create an
+                    empty journal; ``dict``: create journal pages from a dictionary; ``pd.DataFrame``: create journal pages
+                    from a ``pandas.DataFrame``: 'filename.json': load cellpy batch file; 'filename.xlsx': create journal
+                    pages from an Excel file).
+                from_db (bool): Deprecation Warning: this parameter will be removed as it is
+                    the default anyway. Generate the pages from a db (the default option).
+                    This will be over-ridden if description is given.
+
+                **kwargs: sent to sub-function(s) (*e.g.* from_db -> simple_db_reader -> find_files ->
+                    filefinder.search_for_files).
+
+            kwargs -> from_db:
+                project=None, name=None, batch_col=None
+
+
+            kwargs -> simple_db_reader:
+                reader: a reader object (defaults to dbreader.Reader)
+                cell_ids: keys (cell IDs)
+                file_list: file list to send to filefinder (instead of searching in folders for files).
+                pre_path: prepended path to send to filefinder.
+                include_key: include the key col in the pages (the cell IDs).
+                include_individual_arguments: include the argument column in the pages.
+                additional_column_names: list of additional column names to include in the pages.
+
+            kwargs -> filefinder.search_for_files:
+                run_name(str): run-file identification.
+                raw_extension(str): optional, extension of run-files (without the '.').
+                cellpy_file_extension(str): optional, extension for cellpy files
+                    (without the '.').
+                raw_file_dir(path): optional, directory where to look for run-files
+                    (default: read prm-file)
+                cellpy_file_dir(path): optional, directory where to look for
+                    cellpy-files (default: read prm-file)
+                prm_filename(path): optional parameter file can be given.
+                file_name_format(str): format of raw-file names or a glob pattern
+                    (default: YYYYMMDD_[name]EEE_CC_TT_RR).
+                reg_exp(str): use regular expression instead (defaults to None).
+                sub_folders (bool): perform search also in sub-folders.
+                file_list (list of str): perform the search within a given list
+                    of filenames instead of searching the folder(s). The list should
+                    not contain the full filepath (only the actual file names). If
+                    you want to provide the full path, you will have to modify the
+                    file_name_format or reg_exp accordingly.
+                pre_path (path or str): path to prepend the list of files selected
+                     from the file_list.
+            kwargs -> journal.to_file:
+                duplicate_to_local_folder (bool): default True.
+
+
+        Returns:
+            info_dict
+
+        """
+
+        # TODO (jepe): create option to update journal without looking for files
+
+        logging.debug("Creating a journal")
+        logging.debug(f"description: {description}")
+        logging.debug(f"from_db: {from_db}")
+        logging.info(f"name: {self.experiment.journal.name}")
+        logging.info(f"project: {self.experiment.journal.project}")
+        to_project_folder = kwargs.pop("to_project_folder", True)
+        duplicate_to_local_folder = kwargs.pop("duplicate_to_local_folder", True)
+
+        if description is not None:
+            from_db = False
+        else:
+            if self.experiment.journal.pages is not None:
+                warnings.warn(
+                    "You created a journal - but you already have a "
+                    "journal. Hope you know what you are doing!"
+                )
+
+        if from_db:
+            self.experiment.journal.from_db(**kwargs)
+            self.experiment.journal.to_file(
+                duplicate_to_local_folder=duplicate_to_local_folder
+            )
+
+            # TODO: remove these:
+            if duplicate_to_local_folder:
+                self.experiment.journal.duplicate_journal()
+            if to_project_folder:
+                self.duplicate_journal(prms.Paths.batchfiledir)
+
+        else:
+            is_str = isinstance(description, str)
+            is_file = False
+
+            if is_str and pathlib.Path(description).is_file():
+                description = pathlib.Path(description)
+                is_file = True
+
+            if isinstance(description, pathlib.Path):
+                logging.debug("pathlib.Path object given")
+                is_file = True
+
+            if is_file:
+                logging.info(f"loading file {description}")
+                if description.suffix in [".json", ".xlsx"]:
+                    self.experiment.journal.from_file(description)
+                else:
+                    warnings.warn("unknown file extension")
+
+            else:
+                if is_str and description.lower() == "empty":
+                    logging.debug("creating empty journal pages")
+
+                    self.experiment.journal.pages = (
+                        self.experiment.journal.create_empty_pages()
+                    )
+
+                elif isinstance(description, pd.DataFrame):
+                    logging.debug("pandas DataFrame given")
+
+                    p = self.experiment.journal.create_empty_pages()
+                    columns = p.columns
+
+                    for column in columns:
+                        try:
+                            p[column] = description[column]
+                        except KeyError:
+                            logging.debug(f"missing key: {column}")
+
+                    # checking if filenames is a column
+                    if "filenames" in description.columns:
+                        indexes = description["filenames"]
+                    else:
+                        indexes = description.index
+
+                    p.index = indexes
+                    self.experiment.journal.pages = p
+
+                elif isinstance(description, dict):
+                    logging.debug("dictionary given")
+                    self.experiment.journal.pages = (
+                        self.experiment.journal.create_empty_pages()
+                    )
+                    for k in self.experiment.journal.pages.columns:
+                        try:
+                            value = description[k]
+                        except KeyError:
+                            warnings.warn(f"missing key: {k}")
+                        else:
+                            if not isinstance(value, list):
+                                warnings.warn("encountered item that is not a list")
+                                logging.debug(f"converting '{k}' to list-type")
+                                value = [value]
+                            if k == "raw_file_names":
+                                if not isinstance(value[0], list):
+                                    warnings.warn(
+                                        "encountered raw file description"
+                                        "that is not of list-type"
+                                    )
+                                    logging.debug(
+                                        "converting raw file description to a"
+                                        "list of lists"
+                                    )
+                                    value = [value]
+                            self.experiment.journal.pages[k] = value
+
+                    try:
+                        value = description["filenames"]
+                        if not isinstance(value, list):
+                            warnings.warn("encountered item that is not a list")
+                            logging.debug(f"converting '{k}' to list-type")
+                            value = [value]
+                        self.experiment.journal.pages.index = value
+                    except KeyError:
+                        logging.debug("could not interpret the index")
+
+                else:
+                    logging.debug(
+                        "the option you provided seems to be either of "
+                        "an unknown type or a file not found"
+                    )
+                    logging.info(
+                        "did not understand the option - creating empty journal pages"
+                    )
+
+            # finally
+            self.experiment.journal.to_file(
+                duplicate_to_local_folder=duplicate_to_local_folder
+            )
+            self.experiment.journal.generate_folder_names()
+            self.experiment.journal.paginate()
+            self.duplicate_journal(prms.Paths.batchfiledir)
+
+    def create_folder_structure(self) -> None:
+        warnings.warn("Deprecated - use paginate instead.", DeprecationWarning)
+        self.experiment.journal.paginate()
+        logging.info("created folders")
+
+    def paginate(self) -> None:
+        """Create the folders where cellpy will put its output."""
+
+        self.experiment.journal.paginate()
+        logging.info("created folders")
+
+    def save_journal(self) -> None:
+        """Save the journal (json-format).
+
+        The journal file will be saved in the project directory and in the
+        batch-file-directory (prms.Paths.batchfiledir). The latter is useful
+        for processing several batches using the iterate_batches functionality.
+        """
+
+        # Remark! Got an recursive error when running on mac.
+        self.experiment.journal.to_file(to_project_folder=True, paginate=False)
+        logging.info("saved journal pages to project folder")
+        self.duplicate_journal(prms.Paths.batchfiledir)
+        logging.info("duplicated journal pages to batch dir")
+        self.duplicate_journal()
+        logging.info("duplicated journal pages to current dir")
+
+    def export_journal(self, filename=None) -> None:
+        """Export the journal to xlsx."""
+        if filename is None:
+            filename = self.experiment.journal.file_name
+        filename = pathlib.Path(filename).with_suffix(".xlsx")
+        self.experiment.journal.to_file(
+            file_name=filename, to_project_folder=False, paginate=False
+        )
+
+    def duplicate_cellpy_files(
+        self, location: str = "standard", selector: dict = None, **kwargs
+    ) -> None:
+        """Copy the cellpy files and make a journal with the new names available in
+        the current folder.
+
+        Args:
+            location: where to copy the files. Either choose among the following
+                options:
+                "standard": data/interim folder
+                "here": current directory
+                "cellpydatadir": the stated cellpy data dir in your settings (prms)
+            or if the location is not one of the above, use the actual value of the
+                location argument.
+            selector (dict): if given, the cellpy files are reloaded after duplicating and
+                modified based on the given selector(s).
+
+            kwargs: sent to update if selector is provided
+
+        Returns:
+            The updated journal pages.
+        """
+
+        pages = self.experiment.journal.pages
+        cellpy_file_dir = OtherPath(prms.Paths.cellpydatadir)
+
+        if location == "standard":
+            batch_data_dir = pathlib.Path("data") / "interim"
+
+        elif location == "here":
+            batch_data_dir = pathlib.Path(".")
+
+        elif location == "cellpydatadir":
+            batch_data_dir = cellpy_file_dir
+
+        else:
+            batch_data_dir = location
+
+        def _new_file_path(x):
+            return str(batch_data_dir / pathlib.Path(x).name)
+
+        # update the journal pages
+        columns = pages.columns
+        pages["new_cellpy_file_name"] = pages.cellpy_file_name.apply(_new_file_path)
+
+        # copy the cellpy files
+        for n, row in pages.iterrows():
+            logging.info(f"{row.cellpy_file_name} -> {row.new_cellpy_file_name}")
+            try:
+                from_file = row.cellpy_file_name
+                to_file = row.new_cellpy_file_name
+                os.makedirs(os.path.dirname(to_file), exist_ok=True)
+                shutil.copy(from_file, to_file)
+            except shutil.SameFileError:
+                logging.info("Same file! No point in copying")
+            except FileNotFoundError:
+                logging.info("File not found! Cannot copy it!")
+
+        # save the journal pages
+        pages["cellpy_file_name"] = pages["new_cellpy_file_name"]
+        self.experiment.journal.pages = pages[columns]
+        journal_file_name = pathlib.Path(self.experiment.journal.file_name).name
+        self.experiment.journal.to_file(
+            journal_file_name, paginate=False, to_project_folder=False
+        )
+        if selector is not None:
+            logging.info("Modifying the cellpy-files.")
+            logging.info(f"selector: {selector}")
+            self.experiment.force_cellpy = True
+            self.update(selector=selector, **kwargs)
+
+    # TODO: list_journals?
+
+    def link(self, max_cycle=None, force_combine_summaries=False) -> None:
+        """Link journal content to the cellpy-files and load the step information.
+
+        Args:
+            max_cycle (int): set maximum cycle number to link to.
+            force_combine_summaries (bool): automatically run combine_summaries (set this to True
+                if you are re-linking without max_cycle for a batch that previously were linked
+                with max_cycle)
+
+        """
+
+        self.experiment.link(max_cycle=max_cycle)
+        if force_combine_summaries or max_cycle:
+            self.summary_collector.do(reset=True)
+
+    def load(self) -> None:
+        # does the same as update
+        warnings.warn("Deprecated - use update instead.", DeprecationWarning)
+        self.experiment.update()
+
+    def update(self, pool=False, **kwargs) -> None:
+        """Updates the selected datasets.
+
+        Keyword Args (to experiment-instance):
+            all_in_memory (bool): store the `cellpydata` in memory (default
+                False)
+            cell_specs (dict of dicts): individual arguments pr. cell. The `cellspecs` key-word argument
+                dictionary will override the **kwargs and the parameters from the journal pages
+                for the indicated cell.
+            logging_mode (str): sets the logging mode for the loader(s).
+            accept_errors (bool): if True, the loader will continue even if it encounters errors.
+
+
+        Additional kwargs:
+            transferred all the way to the instrument loader, if not
+            picked up earlier. Remark that you can obtain the same pr. cell by
+            providing a `cellspecs` dictionary. The kwargs have precedence over the
+            parameters given in the journal pages, but will be overridden by parameters
+            given by `cellspecs`.
+
+            Merging:
+                recalc (Bool): set to False if you don't want automatic "recalc" of
+                    cycle numbers etc. when merging several data-sets.
+            Loading:
+                selector (dict): selector-based parameters sent to the cellpy-file loader (hdf5) if
+                loading from raw is not necessary (or turned off).
+
+        """
+        self.experiment.errors["update"] = []
+        if pool:
+            self.experiment.parallel_update(**kwargs)
+        else:
+            self.experiment.update(**kwargs)
+
+    def export_cellpy_files(self, path=None, **kwargs) -> None:
+        if path is None:
+            path = pathlib.Path(".").resolve()
+        self.experiment.errors["export_cellpy_files"] = []
+        self.experiment.export_cellpy_files(path=path, **kwargs)
+
+    def recalc(self, **kwargs) -> None:
+        """Run make_step_table and make_summary on all cells.
+
+        Keyword Args:
+            save (bool): Save updated cellpy-files if True (defaults to True).
+            step_opts (dict): parameters to inject to make_steps (defaults to None).
+            summary_opts (dict): parameters to inject to make_summary (defaults to None).
+            indexes (list): Only recalculate for given indexes (i.e. list of cell-names) (defaults to None).
+            calc_steps (bool): Run make_steps before making the summary (defaults to True).
+            testing (bool): Only for testing purposes (defaults to False).
+
+        Returns:
+            None
+        """
+        self.experiment.errors["recalc"] = []
+        self.experiment.recalc(**kwargs)
+
+    def make_summaries(self) -> None:
+        warnings.warn("Deprecated - use combine_summaries instead.", DeprecationWarning)
+
+        self.exporter.do()
+
+    def combine_summaries(self, export_to_csv=True, **kwargs) -> None:
+        """Combine selected columns from each of the cells into single frames"""
+
+        if export_to_csv:
+            self.exporter.do()
+        else:
+            self.summary_collector.do(**kwargs)
+
+    def plot_summaries(
+        self, output_filename=None, backend=None, reload_data=False, **kwargs
+    ) -> None:
+        """Plot the summaries"""
+
+        if reload_data or ("summary_engine" not in self.experiment.memory_dumped):
+            logging.debug("running summary_collector")
+            self.summary_collector.do(reset=True)
+
+        if backend is None:
+            backend = prms.Batch.backend
+
+        if backend in ["bokeh", "matplotlib"]:
+            prms.Batch.backend = backend
+
+        if backend == "bokeh":
+            try:
+                import bokeh.plotting
+
+                prms.Batch.backend = "bokeh"
+
+                if output_filename is not None:
+                    bokeh.plotting.output_file(output_filename)
+                else:
+                    if prms.Batch.notebook:
+                        bokeh.plotting.output_notebook()
+
+            except ModuleNotFoundError:
+                prms.Batch.backend = "matplotlib"
+                logging.warning(
+                    "could not find the bokeh module -> using matplotlib instead"
+                )
+
+        self.plotter.do(**kwargs)
+
+
+def init(*args, **kwargs) -> Batch:
+    """Returns an initialized instance of the Batch class.
+
+    Args:
+        *args: passed directly to Batch()
+            **name**: name of batch;
+            **project**: name of project;
+            **batch_col**: batch column identifier.
+        **kwargs:
+            **file_name**: json file if loading from pages;
+            **default_log_level**: "INFO" or "DEBUG";
+            the rest is passed directly to Batch().
+
+    Examples:
+        >>> empty_batch = Batch.init(db_reader=None)
+        >>> batch_from_file = Batch.init(file_name="cellpy_batch_my_experiment.json")
+        >>> normal_init_of_batch = Batch.init()
+    """
+    # TODO: add option for setting max cycle number (experiment.last_cycle)
+    # set up cellpy logger
+    default_log_level = kwargs.pop("default_log_level", None)
+    testing = kwargs.pop("testing", False)
+    file_name = kwargs.pop("file_name", None)
+    frame = kwargs.pop("frame", None)
+    log.setup_logging(
+        default_level=default_log_level, testing=testing, reset_big_log=True
+    )
+
+    logging.debug(f"returning Batch(kwargs: {kwargs})")
+    if file_name is not None:
+        kwargs.pop("db_reader", None)
+        return Batch(*args, file_name=file_name, db_reader=None, **kwargs)
+    if frame is not None:
+        kwargs.pop("db_reader", None)
+        return Batch(*args, file_name=None, db_reader=None, frame=frame, **kwargs)
+
+    return Batch(*args, **kwargs)
+
+
+def from_journal(journal_file, autolink=True, testing=False) -> Batch:
+    """Create a Batch from a journal file"""
+    # TODO: add option for setting max cycle number (experiment.last_cycle)
+    b = init(db_reader=None, file_name=journal_file, testing=testing)
+    if autolink:
+        b.link()
+    return b
+
+
+def load_pages(file_name) -> pd.DataFrame:
+    """Retrieve pages from a Journal file.
+
+    This function is here to let you easily inspect a Journal file without
+    starting up the full batch-functionality.
+
+    Examples:
+        >>> from cellpy.utils import batch
+        >>> journal_file_name = 'cellpy_journal_one.json'
+        >>> pages = batch.load_pages(journal_file_name)
+
+    Returns:
+        pandas.DataFrame
+
+    """
+
+    logging.info(f"Loading pages from {file_name}")
+    try:
+        pages, *_ = LabJournal.read_journal_jason_file(file_name)
+        return pages
+    except cellpy.exceptions.UnderDefined:
+        logging.critical("could not find any pages.")
+
+
+def process_batch(*args, **kwargs) -> Batch:
+    """Execute a batch run, either from a given file_name or by giving the name and project as input.
+
+    Examples:
+        >>> process_batch(file_name | (name, project), **kwargs)
+
+    Args:
+        *args: file_name or name and project (both string)
+
+    Keyword Args:
+        backend (str): what backend to use when plotting ('bokeh' or 'matplotlib').
+            Defaults to 'matplotlib'.
+        dpi (int): resolution used when saving matplotlib plot(s). Defaults to 300 dpi.
+        default_log_level (str): What log-level to use for console output. Chose between
+            'CRITICAL', 'DEBUG', or 'INFO'. The default is 'CRITICAL' (i.e. usually no log output to console).
+
+    Returns:
+        ``cellpy.batch.Batch`` object
+    """
+    silent = kwargs.pop("silent", False)
+    backend = kwargs.pop("backend", None)
+
+    if backend is not None:
+        prms.Batch.backend = backend
+    else:
+        prms.Batch.backend = "matplotlib"
+
+    dpi = kwargs.pop("dpi", 300)
+
+    default_log_level = kwargs.pop("default_log_level", "CRITICAL")
+    if len(args) == 1:
+        file_name = args[0]
+    else:
+        file_name = kwargs.pop("file_name", None)
+    testing = kwargs.pop("testing", False)
+    log.setup_logging(
+        default_level=default_log_level, reset_big_log=True, testing=testing
+    )
+    logging.debug(f"creating Batch(kwargs: {kwargs})")
+
+    if file_name is not None:
+        kwargs.pop("db_reader", None)
+        b = Batch(*args, file_name=file_name, db_reader=None, **kwargs)
+        b.create_journal(file_name)
+    else:
+        b = Batch(*args, **kwargs)
+        b.create_journal()
+
+    steps = {
+        "paginate": (b.paginate,),
+        "update": (b.update,),
+        "combine": (b.combine_summaries,),
+        "plot": (b.plot_summaries,),
+        "save": (_pb_save_plot, b, dpi),
+    }
+
+    with tqdm(total=(100 * len(steps) + 20), leave=False, file=sys.stdout) as pbar:
+        pbar.update(10)
+        for description in steps:
+            func, *args = steps[description]
+            pbar.set_description(description)
+            pbar.update(10)
+            try:
+                func(*args)
+            except cellpy.exceptions.NullData as e:
+                if not silent:
+                    tqdm.write(f"\nEXCEPTION (NullData): {str(e)}")
+                    tqdm.write("...aborting")
+                    return
+                else:
+                    raise e
+
+        pbar.set_description(f"final")
+        pbar.update(10)
+
+    return b
+
+
+def _pb_save_plot(b, dpi):
+    name = b.experiment.journal.name
+    out_dir = pathlib.Path(b.experiment.journal.batch_dir)
+
+    for n, farm in enumerate(b.plotter.farms):
+        if len(b.plotter.farms) > 1:
+            file_name = f"summary_plot_{name}_{str(n + 1).zfill(3)}.png"
+        else:
+            file_name = f"summary_plot_{name}.png"
+        out = out_dir / file_name
+        logging.info(f"saving file {file_name} in\n{out}")
+        farm.savefig(out, dpi=dpi)
+    # and other stuff
+
+
+def iterate_batches(folder, extension=".json", glob_pattern=None, **kwargs):
+    """Iterate through all journals in given folder.
+
+    Args:
+        folder (str or pathlib.Path): folder containing the journal files.
+        extension (str): extension for the journal files (used when creating a default glob-pattern).
+        glob_pattern (str): optional glob pattern.
+        **kwargs: keyword arguments passed to ``batch.process_batch``.
+    """
+
+    folder = pathlib.Path(folder)
+    logging.info(f"Folder for batches to be iterated: {folder}")
+    if not folder.is_dir():
+        print(f"Could not find the folder ({folder})")
+        print("Aborting...")
+        logging.info("ABORTING - folder not found.")
+        return
+    print(" Iterating through the folder ".center(80, "="))
+    print(f"Folder name: {folder}")
+    if not glob_pattern:
+        glob_pattern = f"*{extension}"
+    print(f"Glob pattern: {glob_pattern}")
+    files = sorted(folder.glob(glob_pattern))
+    if not files:
+        print("No files found! Aborting...")
+        logging.info("ABORTING - no files detected.")
+        return
+    print("Found the following files:")
+    for n, file in enumerate(files):
+        logging.debug(f"file: {file}")
+        print(f"  {str(n).zfill(4)} - {file}")
+
+    print(" Processing ".center(80, "-"))
+    output = []
+    failed = []
+    with tqdm(files, file=sys.stdout) as pbar:
+        for n, file in enumerate(pbar):
+            output_str = f"[{str(n).zfill(4)}]"
+            pbar.set_description(output_str)
+            output_str += f"({file.name})"
+            logging.debug(f"processing file: {file.name}")
+            try:
+                process_batch(file, **kwargs)
+                output_str += " [OK]"
+                logging.debug(f"No errors detected.")
+            except Exception as e:
+                output_str += " [FAILED!]"
+                failed.append(str(file))
+                logging.debug("Error detected.")
+                logging.debug(e)
+
+            output.append(output_str)
+
+    print(" Result ".center(80, "-"))
+    print("\n".join(output))
+    if failed:
+        print("\nFailed:")
+        failed_txt = "\n".join(failed)
+        print(failed_txt)
+        logging.info(failed_txt)
+    print("\n...Finished ")
+
+
+def check_standard():
+    from pathlib import Path
+
+    # Use these when working on my work PC:
+    test_data_path = r"C:\Scripting\MyFiles\development_cellpy\testdata"
+    out_data_path = r"C:\Scripting\Processing\Test\out"
+
+    # Use these when working on my MacBook:
+    # test_data_path = "/Users/jepe/scripting/cellpy/testdata"
+    # out_data_path = "/Users/jepe/cellpy_data"
+
+    test_data_path = Path(test_data_path)
+    out_data_path = Path(out_data_path)
+
+    logging.info("---SETTING SOME PRMS---")
+    prms.Paths.db_filename = "cellpy_db.xlsx"
+    prms.Paths.cellpydatadir = test_data_path / "hdf5"
+    prms.Paths.outdatadir = out_data_path
+    prms.Paths.rawdatadir = test_data_path / "data"
+    prms.Paths.db_path = test_data_path / "db"
+    prms.Paths.filelogdir = test_data_path / "log"
+
+    project = "prebens_experiment"
+    name = "test"
+    batch_col = "b01"
+
+    logging.info("---INITIALISATION OF BATCH---")
+    b = init(name, project, batch_col=batch_col)
+    b.experiment.export_raw = True
+    b.experiment.export_cycles = True
+    logging.info("*creating info df*")
+    b.create_journal()
+    logging.info("*creating folder structure*")
+    b.paginate()
+    logging.info("*load and save*")
+    b.update()
+    logging.info("*make summaries*")
+    try:
+        b.combine_summaries()
+        summaries = b.experiment.memory_dumped
+    except cellpy.exeptions.NullData:
+        print("NO DATA")
+        return
+    # except cellpy.exceptions.NullData:
+    #     print("NOTHING")
+    #     return
+
+    logging.info("*plotting summaries*")
+    b.plot_summaries("tmp_bokeh_plot.html")
+
+    # logging.info("*using special features*")
+    # logging.info(" - select_ocv_points")
+    # analyzer = OCVRelaxationAnalyzer()
+    # analyzer.assign(b.experiment)
+    # analyzer.do()
+    # ocv_df_list = analyzer.farms[0]
+    # for df in ocv_df_list:
+    #     df_up = df.loc[df.type == "ocvrlx_up", :]
+    #     df_down = df.loc[df.type == "ocvrlx_down", :]
+    #     logging.info(df_up)
+    logging.info("---FINISHED---")
+
+
+def check_new():
+    use_db = False
+    f = r"C:\scripts\processing_cellpy\out\SecondLife\cellpy_batch_embla_002.json"
+    # f = r"C:\Scripting\Processing\Celldata\outdata\SilcRoad\cellpy_batch_uio66.json"
+    # f = r"C:\Scripting\Processing\Celldata\outdata\MoZEES\cellpy_batch_round_robin_001.json"
+    name = "embla_test"
+    project = "cellpy_test"
+    batch_col = "b02"
+    if use_db:
+        process_batch(name, project, batch_col=batch_col, nom_cap=372)
+    else:
+        # process_batch(f, nom_cap=372)
+        process_batch(f, force_raw_file=False, force_cellpy=True, nom_cap=372)
+
+
+# TODO: allow exporting html when processing batch instead of just png
+
+
+def check_iterate():
+    folder_name = r"C:\Scripting\Processing\Celldata\live"
+    iterate_batches(folder_name, export_cycles=False, export_raw=False)
+
+
+if __name__ == "__main__":
+    print("---IN BATCH 2 MAIN---")
+    check_new()
```

### Comparing `cellpy-1.0.0a0/cellpy/utils/batch_tools/batch_analyzers.py` & `cellpy-1.0.0a3/cellpy/utils/batch_tools/batch_analyzers.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/cellpy/utils/batch_tools/batch_core.py` & `cellpy-1.0.0a3/cellpy/utils/batch_tools/batch_core.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/cellpy/utils/batch_tools/batch_experiments.py` & `cellpy-1.0.0a3/cellpy/utils/batch_tools/batch_experiments.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,993 +1,995 @@
-import ast
-import logging
-import os
-import pathlib
-import sys
-import warnings
-
-import pandas as pd
-from tqdm.auto import tqdm
-
-import cellpy
-from cellpy import prms
-from cellpy.parameters.internal_settings import get_headers_journal, get_headers_summary
-from cellpy.readers import cellreader
-from cellpy.internals.core import OtherPath
-from cellpy.utils.batch_tools import batch_helpers as helper
-from cellpy.utils.batch_tools.batch_core import BaseExperiment
-from cellpy.utils.batch_tools.batch_journals import LabJournal
-
-hdr_journal = get_headers_journal()
-hdr_summary = get_headers_summary()
-
-
-class CyclingExperiment(BaseExperiment):
-    """Load experimental data into memory.
-
-    This is a re-implementation of the old batch behaviour where
-    all the data-files are processed sequentially (and optionally exported)
-    while the summary tables are kept and processed. This implementation
-    also saves the step tables (for later use when using look-up
-    functionality).
-
-
-    Attributes:
-        journal (:obj: LabJournal): information about the experiment.
-        force_cellpy (bool): tries only to load the cellpy-file if True.
-        force_raw (bool): loads raw-file(s) even though appropriate cellpy-file
-           exists if True.
-        save_cellpy (bool): saves a cellpy-file for each cell if True.
-        accept_errors (bool): in case of error, dont raise an exception, but
-           continue to the next file if True.
-        all_in_memory (bool): store the cellpydata-objects in memory if True.
-        export_cycles (bool): export voltage-capacity curves if True.
-        shifted_cycles (bool): set this to True if you want to export the
-           voltage-capacity curves using the shifted-cycles option (only valid
-           if you set export_cycles to True).
-        export_raw (bool): export the raw-data if True.
-        export_ica (bool): export dq-dv curves if True.
-        last_cycle (int): sets the last cycle (i.e. the highest cycle number)
-           that you would like to process dq-dv on). Use all if None (the
-           default value).
-        selected_summaries (list): a list of summary labels defining what
-           summary columns to make joint summaries from (optional).
-        errors (dict): contains a dictionary listing all the errors encountered.
-
-    Args:
-        db_reader (str or object): custom db_reader (see doc on db_reader).
-
-    Example:
-
-
-    """
-
-    def __init__(self, *args, **kwargs):
-        db_reader = kwargs.pop("db_reader", "default")
-        super().__init__(*args)
-        self.journal = LabJournal(db_reader=db_reader)
-        self.errors = dict()
-        self.log = dict()
-
-        self.force_cellpy = False
-        self.force_raw = False
-        self.force_recalc = False
-        self.save_cellpy = True
-        self.accept_errors = False
-        self.all_in_memory = False
-
-        self.export_cycles = False
-        self.shifted_cycles = False
-        self.export_raw = True
-        self.export_ica = False
-        self.last_cycle = None
-        self.nom_cap = None
-        self.instrument = None
-        self.custom_data_folder = None
-
-        self.selected_summaries = None
-
-    def _repr_html_(self):
-        txt = f"<h2>CyclingExperiment-object</h2> id={hex(id(self))}"
-        txt += "<h3>Main attributes</h3>"
-        txt += f"""
-        <table>
-            <thead>
-                <tr>
-                    <th>Attribute</th>
-                    <th>Value</th>
-                </tr>
-            </thead>
-            <tbody>
-                <tr><td><b>force_cellpy</b></td><td>{self.force_cellpy}</td></tr>
-                <tr><td><b>force_raw</b></td><td>{self.force_raw}</td></tr>
-                <tr><td><b>force_recalc</b></td><td>{self.force_recalc}</td></tr>
-                <tr><td><b>save_cellpy</b></td><td>{self.save_cellpy}</td></tr>
-                <tr><td><b>accept_errors</b></td><td>{self.accept_errors}</td></tr>
-                <tr><td><b>all_in_memory</b></td><td>{self.all_in_memory}</td></tr>
-                <tr><td><b>export_cycles</b></td><td>{self.export_cycles}</td></tr>
-                <tr><td><b>shifted_cycles</b></td><td>{self.shifted_cycles}</td></tr>
-                <tr><td><b>export_raw</b></td><td>{self.export_raw}</td></tr>
-                <tr><td><b>export_ica</b></td><td>{self.export_ica}</td></tr>
-                <tr><td><b>last_cycle</b></td><td>{self.last_cycle}</td></tr>
-                <tr><td><b>nom_cap</b></td><td>{self.nom_cap}</td></tr>
-                <tr><td><b>instrument</b></td><td>{self.instrument}</td></tr>
-                <tr><td><b>custom_data_folder</b></td><td>{self.custom_data_folder}</td></tr>
-                <tr><td><b>selected_summaries</b></td><td>{self.selected_summaries}</td></tr>
-            </tbody>
-        </table>
-        """
-        txt += "<h3>Cells</h3>"
-        txt += f"<p><b>data</b>: contains {len(self)} cells.</p>"
-        return txt
-
-    @staticmethod
-    def _get_cell_spec_from_page(indx: int, row: pd.Series) -> dict:
-        # Edit this if we decide to make "argument families", e.g. loader_split or merger_recalc.
-
-        PRM_SPLITTER = ";"
-        EQUAL_SIGN = "="
-
-        def _arg_parser(text: str) -> None:
-            individual_specs = text.split(PRM_SPLITTER)
-            for p in individual_specs:
-                p, a = p.split(EQUAL_SIGN)
-
-        logging.debug(f"getting cell_spec from journal pages ({indx})")
-        try:
-            cell_spec = row[hdr_journal.argument]
-            logging.debug(cell_spec)
-            if not isinstance(cell_spec, dict):
-                raise TypeError("the cell spec argument is not a dictionary")
-        except Exception as e:
-            logging.warning(f"could not get cell spec for {indx}")
-            logging.warning(f"error message: {e}")
-            return {}
-
-        # converting from str if needed
-        for spec in cell_spec:
-            if isinstance(cell_spec[spec], str):
-                if cell_spec[spec].lower() == "true":
-                    cell_spec[spec] = True
-                elif cell_spec[spec].lower() == "false":
-                    cell_spec[spec] = False
-                elif cell_spec[spec].lower() == "none":
-                    cell_spec[spec] = None
-                else:
-                    try:
-                        logging.debug(
-                            f"Using ast.literal_eval to convert cell-spec value from str '{cell_spec[spec]}'"
-                        )
-                        cell_spec[spec] = ast.literal_eval(cell_spec[spec])
-                    except ValueError as e:
-                        logging.warning(
-                            f"ERROR! Could not convert from str to python object!"
-                        )
-                        logging.debug(e)
-        return cell_spec
-
-    def update(self, all_in_memory=None, cell_specs=None, logging_mode=None, **kwargs):
-        """Updates the selected datasets.
-
-        Args:
-            all_in_memory (bool): store the `cellpydata` in memory (default
-                False)
-            cell_specs (dict of dicts): individual arguments pr. cell. The `cellspecs` key-word argument
-                dictionary will override the **kwargs and the parameters from the journal pages
-                for the indicated cell.
-            logging_mode (str): sets the logging mode for the loader(s).
-
-            kwargs:
-                transferred all the way to the instrument loader, if not
-                picked up earlier. Remark that you can obtain the same pr. cell by
-                providing a `cellspecs` dictionary. The kwargs have precedence over the
-                parameters given in the journal pages, but will be overridden by parameters
-                given by `cellspecs`.
-
-                Merging:
-                    recalc (Bool): set to False if you don't want automatic "recalc" of
-                        cycle numbers etc. when merging several data-sets.
-                Loading:
-                    selector (dict): selector-based parameters sent to the cellpy-file loader (hdf5) if
-                    loading from raw is not necessary (or turned off).
-
-                Debugging:
-                    debug (Bool): set to True if you want to run in debug mode (should never be used by non-developers).
-
-        Debug-mode:
-                 - runs only for the first item in your journal
-
-        Examples:
-            >>> # Don't perform recalculation of cycle numbers etc. when merging
-            >>> # All cells:
-            >>> b.update(recalc=False)
-            >>> # For specific cell(s):
-            >>> cell_specs_cell_01 = {"name_of_cell_01": {"recalc": False}}
-            >>> b.update(cell_specs=cell_specs_cell_01)
-
-        """
-
-        # TODO: implement experiment.last_cycle
-
-        debugging = kwargs.pop("debug", False)
-        testing = kwargs.pop("testing", False)
-
-        # --- cleaning up attributes / arguments etc ---
-        force_cellpy = kwargs.pop("force_cellpy", self.force_cellpy)
-        force_raw = kwargs.pop("force_raw", self.force_raw)
-
-        logging.info("[update experiment]")
-        if all_in_memory is not None:
-            self.all_in_memory = all_in_memory
-
-        logging.info(f"Additional keyword arguments: {kwargs}")
-        selector = kwargs.get("selector", None)
-
-        pages = self.journal.pages
-        if self.nom_cap:
-            warnings.warn(
-                "Setting nominal capacity through attributes will be deprecated soon since it modifies "
-                "the journal pages."
-            )
-            pages[hdr_journal.nom_cap] = self.nom_cap
-
-        if self.instrument:
-            warnings.warn(
-                "Setting instrument through attributes will be deprecated soon since it modifies the journal pages."
-            )
-            pages[hdr_journal.instrument] = self.instrument
-
-        if x := kwargs.pop("instrument", None):
-            warnings.warn(
-                "Setting instrument through params will be deprecated soon since it modifies the journal pages."
-                "Future version will require instrument in the journal pages."
-            )
-            pages[hdr_journal.instrument] = x
-
-        if pages.empty:
-            raise Exception("your journal is empty")
-
-        # --- init ---
-        summary_frames = dict()
-        cell_data_frames = dict()
-        number_of_runs = len(pages)
-        logging.debug(f"You have {number_of_runs} cells in your journal")
-        counter = 0
-        errors = []
-
-        pbar = tqdm(list(pages.iterrows()), file=sys.stdout, leave=False)
-
-        if debugging:
-            pbar = tqdm(list(pages.iterrows())[0:1], file=sys.stdout, leave=False)
-
-        # --- iterating ---
-        # TODO: create a multiprocessing pool and get one statusbar pr cell
-        for index, row in pbar:
-            counter += 1
-            h_txt = f"{index}"
-            n_txt = f"loading {counter}"
-            l_txt = f"starting to process file # {counter} ({index})"
-            pbar.set_description(n_txt, refresh=True)
-            cell_spec_page = self._get_cell_spec_from_page(index, row)
-
-            if cell_specs is not None:
-                cell_spec = cell_specs.get(index, dict())
-            else:
-                cell_spec = dict()
-
-            cell_spec = {**cell_spec_page, **kwargs, **cell_spec}
-            l_txt += f" cell_spec: {cell_spec}"
-            logging.debug(l_txt)
-
-            # --- UPDATING ARGUMENTS ---
-            filename = None
-            instrument = None
-            cellpy_file = OtherPath(row[hdr_journal.cellpy_file_name])
-            _cellpy_file = None
-            if not force_raw and cellpy_file.is_file():
-                _cellpy_file = cellpy_file
-                logging.debug(f"Got cellpy file: {_cellpy_file}")
-            if not force_cellpy:
-                filename = row[hdr_journal.raw_file_names]
-                instrument = row[hdr_journal.instrument]
-
-            cycle_mode = row[hdr_journal.cell_type]
-            mass = row[hdr_journal.mass]
-            nom_cap = row[hdr_journal.nom_cap]
-
-            loading = None
-            area = None
-            if hdr_journal.loading in row:
-                loading = row[hdr_journal.loading]
-            if hdr_journal.area in row:
-                area = row[hdr_journal.area]
-
-            summary_kwargs = {
-                "use_cellpy_stat_file": prms.Reader.use_cellpy_stat_file,
-            }
-
-            step_kwargs = {}
-            if not filename and not force_cellpy:
-                logging.info(
-                    f"Raw file(s) not given in the journal.pages for index={index}"
-                )
-                errors.append(index)
-                continue
-
-            elif not cellpy_file and force_cellpy:
-                logging.info(
-                    f"Cellpy file not given in the journal.pages for index={index}"
-                )
-                errors.append(index)
-                continue
-
-            else:
-                logging.info(f"Processing {index}")
-
-            logging.info("loading cell")
-            try:
-                logging.debug("inside try: running cellpy.get")
-                cell_data = cellpy.get(
-                    filename=filename,
-                    instrument=instrument,
-                    cellpy_file=_cellpy_file,
-                    cycle_mode=cycle_mode,
-                    mass=mass,
-                    nom_cap=nom_cap,
-                    loading=loading,
-                    area=area,
-                    step_kwargs=step_kwargs,
-                    summary_kwargs=summary_kwargs,
-                    selector=selector,
-                    logging_mode=logging_mode,
-                    testing=testing,
-                    **cell_spec,
-                )
-                logging.info("loaded cell")
-
-            except Exception as e:
-                logging.info("Failed to load: " + str(e))
-                errors.append("update:" + str(index))
-                h_txt += " [-]"
-                pbar.set_postfix_str(s=h_txt, refresh=True)
-                if not self.accept_errors:
-                    raise e
-                continue
-
-            if cell_data.empty:
-                logging.info("...not loaded...")
-                logging.debug("Data is empty. Could not load cell!")
-                errors.append("check:" + str(index))
-                h_txt += " [-]"
-                pbar.set_postfix_str(s=h_txt, refresh=True)
-                continue
-
-            logging.info("...loaded successfully...")
-            h_txt += " [OK]"
-            pbar.set_postfix_str(s=h_txt, refresh=True)
-            summary_tmp = cell_data.data.summary
-            logging.info("Trying to get summary_data")
-
-            if cell_data.data.steps is None or self.force_recalc:
-                logging.info("Running make_step_table")
-                n_txt = f"steps {counter}"
-                pbar.set_description(n_txt, refresh=True)
-                cell_data.make_step_table()
-
-            if summary_tmp is None or self.force_recalc:
-                logging.info("Running make_summary")
-                n_txt = f"summary {counter}"
-                pbar.set_description(n_txt, refresh=True)
-                cell_data.make_summary(find_end_voltage=True, find_ir=True)
-
-            # some clean-ups (might not be needed anymore):
-            if not summary_tmp.index.name == hdr_summary.cycle_index:
-                logging.debug("Setting index to Cycle_Index")
-                # check if it is a byte-string
-                if b"Cycle_Index" in summary_tmp.columns:
-                    logging.debug("Seems to be a byte-string in the column-headers")
-                    summary_tmp.rename(
-                        columns={b"Cycle_Index": "Cycle_Index"}, inplace=True
-                    )
-                try:
-                    summary_tmp.set_index("cycle_index", inplace=True)
-                except KeyError:
-                    logging.debug("cycle_index already an index")
-
-            summary_frames[index] = summary_tmp
-
-            if self.all_in_memory:
-                cell_data_frames[index] = cell_data
-            else:
-                cell_data_frames[index] = cellreader.CellpyCell(initialize=True)
-                cell_data_frames[index].data.steps = cell_data.data.steps
-
-            if self.save_cellpy:
-                logging.info("saving to cellpy-format")
-                n_txt = f"saving {counter}"
-                pbar.set_description(n_txt, refresh=True)
-                if self.custom_data_folder is not None:
-                    print("Save to custom data-folder not implemented yet")
-                    print(f"Saving to {row.cellpy_file_name} instead")
-                if not row.fixed:
-                    logging.info("saving cell to %s" % row.cellpy_file_name)
-                    cell_data.ensure_step_table = True
-                    try:
-                        cell_data.save(row.cellpy_file_name)
-                    except Exception as e:
-                        logging.error("saving file failed")
-                        logging.error(e)
-
-                else:
-                    logging.debug("saving cell skipped (set to 'fixed' in info_df)")
-            else:
-                logging.info("You opted to not save to cellpy-format")
-                logging.info("It is usually recommended to save to cellpy-format:")
-                logging.info(" >>> b.experiment.save_cellpy = True")
-                logging.info(
-                    "Without the cellpy-files, you cannot select specific cells"
-                )
-                logging.info("if you did not opt to store all in memory")
-
-            if self.export_raw or self.export_cycles:
-                export_text = "exporting"
-                if self.export_raw:
-                    export_text += " [raw]"
-                if self.export_cycles:
-                    export_text += " [cycles]"
-                logging.info(export_text)
-                n_txt = f"{export_text} {counter}"
-                pbar.set_description(n_txt, refresh=True)
-                cell_data.to_csv(
-                    self.journal.raw_dir,
-                    sep=prms.Reader.sep,
-                    cycles=self.export_cycles,
-                    shifted=self.shifted_cycles,
-                    raw=self.export_raw,
-                    last_cycle=self.last_cycle,
-                )
-
-            if self.export_ica:
-                logging.info("exporting [ica]")
-                try:
-                    helper.export_dqdv(
-                        cell_data,
-                        savedir=self.journal.raw_dir,
-                        sep=prms.Reader.sep,
-                        last_cycle=self.last_cycle,
-                    )
-                except Exception as e:
-                    logging.error("Could not make/export dq/dv data")
-                    logging.debug(
-                        "Failed to make/export " "dq/dv data (%s): %s" % (index, str(e))
-                    )
-                    errors.append("ica:" + str(index))
-
-        self.errors["update"] = errors
-        self.summary_frames = summary_frames
-        self.cell_data_frames = cell_data_frames
-
-    def parallel_update(
-        self, all_in_memory=None, cell_specs=None, logging_mode=None, **kwargs
-    ):
-        """Updates the selected datasets in parallel.
-
-        Args:
-            all_in_memory (bool): store the `cellpydata` in memory (default
-                False)
-            cell_specs (dict of dicts): individual arguments pr. cell. The `cellspecs` key-word argument
-                dictionary will override the **kwargs and the parameters from the journal pages
-                for the indicated cell.
-            logging_mode (str): sets the logging mode for the loader(s).
-
-            kwargs:
-                transferred all the way to the instrument loader, if not
-                picked up earlier. Remark that you can obtain the same pr. cell by
-                providing a `cellspecs` dictionary. The kwargs have precedence over the
-                parameters given in the journal pages, but will be overridden by parameters
-                given by `cellspecs`.
-
-                Merging:
-                    recalc (Bool): set to False if you don't want automatic "recalc" of
-                        cycle numbers etc. when merging several data-sets.
-                Loading:
-                    selector (dict): selector-based parameters sent to the cellpy-file loader (hdf5) if
-                    loading from raw is not necessary (or turned off).
-
-                Debugging:
-                    debug (Bool): set to True if you want to run in debug mode (should never be used by non-developers).
-
-        Debug-mode:
-                 - runs only for the first item in your journal
-
-        Examples:
-            >>> # Don't perform recalculation of cycle numbers etc. when merging
-            >>> # All cells:
-            >>> b.update(recalc=False)
-            >>> # For specific cell(s):
-            >>> cell_specs_cell_01 = {"name_of_cell_01": {"recalc": False}}
-            >>> b.update(cell_specs=cell_specs_cell_01)
-
-        """
-        status = "PROD"  # set this to DEV when developing this
-        async_mode = "threading"
-        logging.debug("PARALLEL UPDATE")
-        # TODO: implement experiment.last_cycle
-        if status != "DEV":
-            print("SORRY - MULTIPROCESSING IS NOT IMPLEMENTED PROPERLY YET")
-            return self.update(
-                all_in_memory=all_in_memory,
-                cell_specs=cell_specs,
-                logging_mode=logging_mode,
-                **kwargs,
-            )
-
-        import concurrent.futures
-        import multiprocessing
-
-        max_number_processes = multiprocessing.cpu_count()
-
-        if async_mode == "threading":
-            pool_executor = concurrent.futures.ThreadPoolExecutor
-        else:
-            pool_executor = concurrent.futures.ProcessPoolExecutor
-
-        debugging = kwargs.pop("debug", False)
-
-        # --- cleaning up attributes / arguments etc ---
-        force_cellpy = kwargs.pop("force_cellpy", self.force_cellpy)
-        force_raw = kwargs.pop("force_raw", self.force_raw)
-
-        logging.info("[update experiment]")
-        if all_in_memory is not None:
-            self.all_in_memory = all_in_memory
-
-        logging.info(f"Additional keyword arguments: {kwargs}")
-        selector = kwargs.get("selector", None)
-
-        pages = self.journal.pages
-        if self.nom_cap:
-            warnings.warn(
-                "Setting nominal capacity through attributes will be deprecated soon since it modifies "
-                "the journal pages."
-            )
-            pages[hdr_journal.nom_cap] = self.nom_cap
-
-        if self.instrument:
-            warnings.warn(
-                "Setting instrument through attributes will be deprecated soon since it modifies the journal pages."
-            )
-            pages[hdr_journal.instrument] = self.instrument
-
-        if x := kwargs.pop("instrument", None):
-            warnings.warn(
-                "Setting instrument through params will be deprecated soon since it modifies the journal pages."
-                "Future version will require instrument in the journal pages."
-            )
-            pages[hdr_journal.instrument] = x
-
-        if pages.empty:
-            raise Exception("your journal is empty")
-
-        # --- init ---
-        summary_frames = dict()
-        cell_data_frames = dict()
-        number_of_runs = len(pages)
-        logging.debug(f"You have {number_of_runs} cells in your journal")
-        counter = 0
-        errors = []
-
-        pbar = tqdm(list(pages.iterrows()), file=sys.stdout, leave=False)
-
-        if debugging:
-            pbar = tqdm(list(pages.iterrows())[0:1], file=sys.stdout, leave=False)
-
-        # --- iterating ---
-        # TODO: create a multiprocessing pool and get one statusbar pr cell
-        params = []
-        with pool_executor(max_number_processes) as executor:
-            for index, row in pages.iterrows():
-                counter += 1
-                cell_spec_page = self._get_cell_spec_from_page(index, row)
-
-                if cell_specs is not None:
-                    cell_spec = cell_specs.get(index, dict())
-                else:
-                    cell_spec = dict()
-
-                cell_spec = {**cell_spec_page, **kwargs, **cell_spec}
-
-                # --- UPDATING ARGUMENTS ---
-                filename = None
-                instrument = None
-                cellpy_file = OtherPath(row[hdr_journal.cellpy_file_name])
-                _cellpy_file = None
-                if not force_raw and cellpy_file.is_file():
-                    _cellpy_file = cellpy_file
-                    logging.debug(f"Got cellpy file: {_cellpy_file}")
-                if not force_cellpy:
-                    filename = row[hdr_journal.raw_file_names]
-                    instrument = row[hdr_journal.instrument]
-
-                cycle_mode = row[hdr_journal.cell_type]
-                mass = row[hdr_journal.mass]
-                nom_cap = row[hdr_journal.nom_cap]
-
-                loading = None
-                area = None
-                if hdr_journal.loading in row:
-                    loading = row[hdr_journal.loading]
-                if hdr_journal.area in row:
-                    area = row[hdr_journal.area]
-
-                summary_kwargs = {
-                    "use_cellpy_stat_file": prms.Reader.use_cellpy_stat_file,
-                }
-
-                step_kwargs = {}
-                if not filename and not force_cellpy:
-                    logging.info(
-                        f"Raw file(s) not given in the journal.pages for index={index}"
-                    )
-                    errors.append(index)
-                    continue
-
-                elif not cellpy_file and force_cellpy:
-                    logging.info(
-                        f"Cellpy file not given in the journal.pages for index={index}"
-                    )
-                    errors.append(index)
-                    continue
-
-                else:
-                    logging.info(f"Processing {index}")
-
-                logging.info("loading cell")
-                params.append(
-                    dict(
-                        filename=filename,
-                        instrument=instrument,
-                        cellpy_file=_cellpy_file,
-                        cycle_mode=cycle_mode,
-                        mass=mass,
-                        nom_cap=nom_cap,
-                        loading=loading,
-                        area=area,
-                        step_kwargs=step_kwargs,
-                        summary_kwargs=summary_kwargs,
-                        selector=selector,
-                        logging_mode=logging_mode,
-                        testing=False,
-                        **cell_spec,
-                    )
-                )
-
-            pool = [executor.submit(cellpy.get, **param) for param in params]
-            for i in concurrent.futures.as_completed(pool):
-                cell_data = i.result()
-                if cell_data.empty:
-                    logging.info("...not loaded...")
-                    logging.debug("Data is empty. Could not load cell!")
-                    errors.append("check:" + str(index))
-
-                logging.info("...loaded successfully...")
-                summary_tmp = cell_data.data.summary
-                logging.info("Trying to get summary_data")
-
-                if cell_data.data.steps is None or self.force_recalc:
-                    logging.info("Running make_step_table")
-                    cell_data.make_step_table()
-
-                if summary_tmp is None or self.force_recalc:
-                    logging.info("Running make_summary")
-                    cell_data.make_summary(find_end_voltage=True, find_ir=True)
-
-                # some clean-ups (might not be needed anymore):
-                if not summary_tmp.index.name == hdr_summary.cycle_index:
-                    logging.debug("Setting index to Cycle_Index")
-                    # check if it is a byte-string
-                    if b"Cycle_Index" in summary_tmp.columns:
-                        logging.debug("Seems to be a byte-string in the column-headers")
-                        summary_tmp.rename(
-                            columns={b"Cycle_Index": "Cycle_Index"}, inplace=True
-                        )
-                    try:
-                        summary_tmp.set_index("cycle_index", inplace=True)
-                    except KeyError:
-                        logging.debug("cycle_index already an index")
-
-                summary_frames[index] = summary_tmp
-
-                if self.all_in_memory:
-                    cell_data_frames[index] = cell_data
-                else:
-                    cell_data_frames[index] = cellreader.CellpyCell(initialize=True)
-                    cell_data_frames[index].data.steps = cell_data.data.steps
-
-                if self.save_cellpy:
-                    logging.info("saving to cellpy-format")
-                    n_txt = f"saving {counter}"
-                    pbar.set_description(n_txt, refresh=True)
-                    if self.custom_data_folder is not None:
-                        print("Save to custom data-folder not implemented yet")
-                        print(f"Saving to {row.cellpy_file_name} instead")
-                    if not row.fixed:
-                        logging.info("saving cell to %s" % row.cellpy_file_name)
-                        cell_data.ensure_step_table = True
-                        try:
-                            cell_data.save(row.cellpy_file_name)
-                        except Exception as e:
-                            logging.error("saving file failed")
-                            logging.error(e)
-
-                    else:
-                        logging.debug("saving cell skipped (set to 'fixed' in info_df)")
-                else:
-                    logging.info("You opted to not save to cellpy-format")
-                    logging.info("It is usually recommended to save to cellpy-format:")
-                    logging.info(" >>> b.experiment.save_cellpy = True")
-                    logging.info(
-                        "Without the cellpy-files, you cannot select specific cells"
-                    )
-                    logging.info("if you did not opt to store all in memory")
-
-                if self.export_raw or self.export_cycles:
-                    export_text = "exporting"
-                    if self.export_raw:
-                        export_text += " [raw]"
-                    if self.export_cycles:
-                        export_text += " [cycles]"
-                    logging.info(export_text)
-                    n_txt = f"{export_text} {counter}"
-                    pbar.set_description(n_txt, refresh=True)
-                    cell_data.to_csv(
-                        self.journal.raw_dir,
-                        sep=prms.Reader.sep,
-                        cycles=self.export_cycles,
-                        shifted=self.shifted_cycles,
-                        raw=self.export_raw,
-                        last_cycle=self.last_cycle,
-                    )
-
-                if self.export_ica:
-                    logging.info("exporting [ica]")
-                    try:
-                        helper.export_dqdv(
-                            cell_data,
-                            savedir=self.journal.raw_dir,
-                            sep=prms.Reader.sep,
-                            last_cycle=self.last_cycle,
-                        )
-                    except Exception as e:
-                        logging.error("Could not make/export dq/dv data")
-                        logging.debug(
-                            "Failed to make/export "
-                            "dq/dv data (%s): %s" % (index, str(e))
-                        )
-                        errors.append("ica:" + str(index))
-
-        self.errors["update"] = errors
-        self.summary_frames = summary_frames
-        self.cell_data_frames = cell_data_frames
-
-    def export_cellpy_files(self, path=None, **kwargs):
-        """Export all cellpy-files to a given path.
-
-        Remarks:
-            This method can only export to local folders
-            (OtherPath objects are not formally supported, but
-            might still work if the path is local).
-
-        Args:
-            path (str, pathlib.Path): path to export to (default: current working directory)
-        """
-        if path is None:
-            path = "."
-        errors = []
-        path = pathlib.Path(path)
-        cell_names = self.cell_names
-        for cell_name in cell_names:
-            cellpy_file_name = self.journal.pages.loc[
-                cell_name, hdr_journal.cellpy_file_name
-            ]
-            cellpy_file_name = path / pathlib.Path(cellpy_file_name).name
-            print(f"Exporting {cell_name} to {cellpy_file_name}")
-            try:
-                c = self.data[cell_name]
-            except TypeError as e:
-                errors.append(f"could not extract data for {cell_name} - linking")
-                self._link_cellpy_file(cell_name)
-
-            c.save(cellpy_file_name, **kwargs)
-        self.errors["export_cellpy_files"] = errors
-
-    @property
-    def cell_names(self):
-        """Returns a list of cell-names (strings)"""
-        try:
-            return [key for key in self.cell_data_frames]
-        except TypeError:
-            return None
-
-    def status(self):
-        print("\n")
-        print(" STATUS ".center(80, "="))
-        print(self)
-        print(" summary frames ".center(80, "-"))
-        if self.summary_frames is not None:
-            for key in self.summary_frames:
-                print(f" {{{key}}}")
-        print(" memory dumped ".center(80, "-"))
-        if self.memory_dumped is not None:
-            for key in self.memory_dumped:
-                print(f"{key}: {type(self.memory_dumped[key])}")
-        print(80 * "=")
-
-    def link(self, **kwargs):
-        """Ensure that an appropriate link to the cellpy-files exists for
-        each cell.
-
-        The experiment will then contain a CellpyCell object for each cell
-        (in the cell_data_frames attribute) with only the step-table stored.
-
-        Remark that running update persists the summary frames instead (or
-        everything in case you specify all_in_memory=True).
-        This might be considered "a strange and unexpected behaviour". Sorry
-        for that (but the authors of this package is also a bit strange...).
-
-        (OK, I will change it. Soon.)
-
-        **kwargs: passed to _link_cellpy_file
-            max_cycle (int): maximum cycle number to link/load (remark that the
-                cellpy objects will get the property overwrite_able set to False
-                if you give a max_cycle to prevent accidentally saving a "truncated"
-                file (use c.save(filename, overwrite=True) to force overwrite))
-
-
-        """
-        logging.info("[establishing links]")
-        logging.debug("checking and establishing link to data")
-
-        errors = []
-
-        for cell_label in self.journal.pages.index:
-            logging.debug(f"trying to link {cell_label}")
-            try:
-                self._link_cellpy_file(cell_label, **kwargs)
-            except IOError as e:
-                logging.warning(e)
-                e_txt = f"{cell_label}: links not established - try update instead"
-                logging.warning(e_txt)
-                errors.append(e_txt)
-
-        self.errors["link"] = errors
-
-    def recalc(
-        self,
-        save=True,
-        step_opts=None,
-        summary_opts=None,
-        indexes=None,
-        calc_steps=True,
-        testing=False,
-    ):
-        """Run make_step_table and make_summary on all cells.
-
-        Args:
-            save (bool): Save updated cellpy-files if True.
-            step_opts (dict): parameters to inject to make_steps.
-            summary_opts (dict): parameters to inject to make_summary.
-            indexes (list): Only recalculate for given indexes (i.e. list of cell-names).
-            calc_steps (bool): Run make_steps before making the summary.
-            testing (bool): Only for testing purposes.
-
-        Returns:
-            None
-        """
-
-        # TODO: option (default) to only recalc if the values (mass, nom_cap,...) have changed
-        errors = []
-        log = []
-        if testing:
-            pbar = tqdm(
-                list(self.journal.pages.iloc[0:2, :].iterrows()),
-                file=sys.stdout,
-                leave=False,
-            )
-        elif indexes is not None:
-            pbar = tqdm(
-                list(self.journal.pages.loc[indexes, :].iterrows()),
-                file=sys.stdout,
-                leave=False,
-            )
-        else:
-            pbar = tqdm(
-                list(self.journal.pages.iterrows()), file=sys.stdout, leave=False
-            )
-        for indx, row in pbar:
-            nom_cap = row[hdr_journal.nom_cap]
-            mass = row[hdr_journal.mass]
-            pbar.set_description(indx)
-            try:
-                c = self.data[indx]
-            except TypeError as e:
-                e_txt = (
-                    f"could not extract data for {indx} - have you forgotten to link?"
-                )
-                errors.append(e_txt)
-                warnings.warn(e_txt)
-
-            else:
-                if nom_cap:
-                    c.set_nom_cap(nom_cap)
-                if mass:
-                    c.set_mass(mass)
-                try:
-                    if calc_steps:
-                        pbar.set_postfix_str(s="steps", refresh=True)
-                        if step_opts is not None:
-                            c.make_step_table(**step_opts)
-                        else:
-                            c.make_step_table()
-
-                    pbar.set_postfix_str(s="summary", refresh=True)
-                    if summary_opts is not None:
-                        c.make_summary(**summary_opts)
-                    else:
-                        c.make_summary(find_end_voltage=True, find_ir=True)
-
-                except Exception as e:
-                    e_txt = f"recalculating for {indx} failed!"
-                    errors.append(e_txt)
-                    warnings.warn(e_txt)
-                else:
-                    if save:
-                        # remark! got a win error when trying to save (hdf5-file in use) (must fix this)
-                        pbar.set_postfix_str(s="save", refresh=True)
-                        try:
-                            c.save(row.cellpy_file_name)
-                            log.append(f"saved {indx} to {row.cellpy_file_name}")
-                        except Exception as e:
-                            e_txt = f"saving {indx} to {row.cellpy_file_name} failed!"
-                            errors.append(e_txt)
-                            warnings.warn(e_txt)
-        self.errors["recalc"] = errors
-        self.log["recalc"] = log
-
-
-class ImpedanceExperiment(BaseExperiment):
-    def __init__(self):
-        super().__init__()
-
-
-class LifeTimeExperiment(BaseExperiment):
-    def __init__(self):
-        super().__init__()
-
-
-if __name__ == "__main__":
-    from pathlib import Path
-    import os
-    import pandas as pd
-    import numpy as np
-    import seaborn as sns
-    import plotly.express as px
-
-    import cellpy
-    from cellpy.utils import batch, helpers, plotutils
-
-    project_dir = Path("../../../testdata/batch_project")
-    print(f"{project_dir.resolve()=}")
-    journal = project_dir / "test_project.json"
-    journal = journal.resolve()
-    print(f"{journal=}")
-    assert project_dir.is_dir()
-    assert journal.is_file()
-    os.chdir(project_dir)
-
-    print(f"cellpy version: {cellpy.__version__}")
-    cellpy.log.setup_logging("INFO")
-
-    b = batch.from_journal(journal)
-    b.update()
-
-    print("Ended OK")
+import ast
+import logging
+import os
+import pathlib
+import sys
+import warnings
+
+import pandas as pd
+from tqdm.auto import tqdm
+
+import cellpy
+from cellpy import prms
+from cellpy.parameters.internal_settings import get_headers_journal, get_headers_summary
+from cellpy.readers import cellreader
+from cellpy.internals.core import OtherPath
+from cellpy.utils.batch_tools import batch_helpers as helper
+from cellpy.utils.batch_tools.batch_core import BaseExperiment
+from cellpy.utils.batch_tools.batch_journals import LabJournal
+
+hdr_journal = get_headers_journal()
+hdr_summary = get_headers_summary()
+
+
+class CyclingExperiment(BaseExperiment):
+    """Load experimental data into memory.
+
+    This is a re-implementation of the old batch behaviour where
+    all the data-files are processed sequentially (and optionally exported)
+    while the summary tables are kept and processed. This implementation
+    also saves the step tables (for later use when using look-up
+    functionality).
+
+
+    Attributes:
+        journal (:obj: LabJournal): information about the experiment.
+        force_cellpy (bool): tries only to load the cellpy-file if True.
+        force_raw (bool): loads raw-file(s) even though appropriate cellpy-file
+           exists if True.
+        save_cellpy (bool): saves a cellpy-file for each cell if True.
+        accept_errors (bool): in case of error, dont raise an exception, but
+           continue to the next file if True.
+        all_in_memory (bool): store the cellpydata-objects in memory if True.
+        export_cycles (bool): export voltage-capacity curves if True.
+        shifted_cycles (bool): set this to True if you want to export the
+           voltage-capacity curves using the shifted-cycles option (only valid
+           if you set export_cycles to True).
+        export_raw (bool): export the raw-data if True.
+        export_ica (bool): export dq-dv curves if True.
+        last_cycle (int): sets the last cycle (i.e. the highest cycle number)
+           that you would like to process dq-dv on). Use all if None (the
+           default value).
+        selected_summaries (list): a list of summary labels defining what
+           summary columns to make joint summaries from (optional).
+        errors (dict): contains a dictionary listing all the errors encountered.
+
+    Args:
+        db_reader (str or object): custom db_reader (see doc on db_reader).
+
+    Example:
+
+
+    """
+
+    def __init__(self, *args, **kwargs):
+        db_reader = kwargs.pop("db_reader", "default")
+        super().__init__(*args)
+        self.journal = LabJournal(db_reader=db_reader)
+        self.errors = dict()
+        self.log = dict()
+
+        self.force_cellpy = False
+        self.force_raw = False
+        self.force_recalc = False
+        self.save_cellpy = True
+        self.accept_errors = False
+        self.all_in_memory = False
+
+        self.export_cycles = False
+        self.shifted_cycles = False
+        self.export_raw = True
+        self.export_ica = False
+        self.last_cycle = None
+        self.nom_cap = None
+        self.instrument = None
+        self.custom_data_folder = None
+
+        self.selected_summaries = None
+
+    def _repr_html_(self):
+        txt = f"<h2>CyclingExperiment-object</h2> id={hex(id(self))}"
+        txt += "<h3>Main attributes</h3>"
+        txt += f"""
+        <table>
+            <thead>
+                <tr>
+                    <th>Attribute</th>
+                    <th>Value</th>
+                </tr>
+            </thead>
+            <tbody>
+                <tr><td><b>force_cellpy</b></td><td>{self.force_cellpy}</td></tr>
+                <tr><td><b>force_raw</b></td><td>{self.force_raw}</td></tr>
+                <tr><td><b>force_recalc</b></td><td>{self.force_recalc}</td></tr>
+                <tr><td><b>save_cellpy</b></td><td>{self.save_cellpy}</td></tr>
+                <tr><td><b>accept_errors</b></td><td>{self.accept_errors}</td></tr>
+                <tr><td><b>all_in_memory</b></td><td>{self.all_in_memory}</td></tr>
+                <tr><td><b>export_cycles</b></td><td>{self.export_cycles}</td></tr>
+                <tr><td><b>shifted_cycles</b></td><td>{self.shifted_cycles}</td></tr>
+                <tr><td><b>export_raw</b></td><td>{self.export_raw}</td></tr>
+                <tr><td><b>export_ica</b></td><td>{self.export_ica}</td></tr>
+                <tr><td><b>last_cycle</b></td><td>{self.last_cycle}</td></tr>
+                <tr><td><b>nom_cap</b></td><td>{self.nom_cap}</td></tr>
+                <tr><td><b>instrument</b></td><td>{self.instrument}</td></tr>
+                <tr><td><b>custom_data_folder</b></td><td>{self.custom_data_folder}</td></tr>
+                <tr><td><b>selected_summaries</b></td><td>{self.selected_summaries}</td></tr>
+            </tbody>
+        </table>
+        """
+        txt += "<h3>Cells</h3>"
+        txt += f"<p><b>data</b>: contains {len(self)} cells.</p>"
+        return txt
+
+    @staticmethod
+    def _get_cell_spec_from_page(indx: int, row: pd.Series) -> dict:
+        # Edit this if we decide to make "argument families", e.g. loader_split or merger_recalc.
+
+        PRM_SPLITTER = ";"
+        EQUAL_SIGN = "="
+
+        def _arg_parser(text: str) -> None:
+            individual_specs = text.split(PRM_SPLITTER)
+            for p in individual_specs:
+                p, a = p.split(EQUAL_SIGN)
+
+        logging.debug(f"getting cell_spec from journal pages ({indx})")
+        try:
+            cell_spec = row[hdr_journal.argument]
+            logging.debug(cell_spec)
+            if not isinstance(cell_spec, dict):
+                raise TypeError("the cell spec argument is not a dictionary")
+        except Exception as e:
+            logging.warning(f"could not get cell spec for {indx}")
+            logging.warning(f"error message: {e}")
+            return {}
+
+        # converting from str if needed
+        for spec in cell_spec:
+            if isinstance(cell_spec[spec], str):
+                if cell_spec[spec].lower() == "true":
+                    cell_spec[spec] = True
+                elif cell_spec[spec].lower() == "false":
+                    cell_spec[spec] = False
+                elif cell_spec[spec].lower() == "none":
+                    cell_spec[spec] = None
+                else:
+                    try:
+                        logging.debug(
+                            f"Using ast.literal_eval to convert cell-spec value from str '{cell_spec[spec]}'"
+                        )
+                        cell_spec[spec] = ast.literal_eval(cell_spec[spec])
+                    except ValueError as e:
+                        logging.warning(
+                            f"ERROR! Could not convert from str to python object!"
+                        )
+                        logging.debug(e)
+        return cell_spec
+
+    def update(self, all_in_memory=None, cell_specs=None, logging_mode=None, accept_errors=None, **kwargs):
+        """Updates the selected datasets.
+
+        Args:
+            all_in_memory (bool): store the `cellpydata` in memory (default
+                False)
+            cell_specs (dict of dicts): individual arguments pr. cell. The `cellspecs` key-word argument
+                dictionary will override the **kwargs and the parameters from the journal pages
+                for the indicated cell.
+            logging_mode (str): sets the logging mode for the loader(s).
+            accept_errors (bool): if True, the loader will continue even if it encounters errors.
+
+            kwargs:
+                transferred all the way to the instrument loader, if not
+                picked up earlier. Remark that you can obtain the same pr. cell by
+                providing a `cellspecs` dictionary. The kwargs have precedence over the
+                parameters given in the journal pages, but will be overridden by parameters
+                given by `cellspecs`.
+
+                Merging:
+                    recalc (Bool): set to False if you don't want automatic "recalc" of
+                        cycle numbers etc. when merging several data-sets.
+                Loading:
+                    selector (dict): selector-based parameters sent to the cellpy-file loader (hdf5) if
+                    loading from raw is not necessary (or turned off).
+
+                Debugging:
+                    debug (Bool): set to True if you want to run in debug mode (should never be used by non-developers).
+
+        Debug-mode:
+                 - runs only for the first item in your journal
+
+        Examples:
+            >>> # Don't perform recalculation of cycle numbers etc. when merging
+            >>> # All cells:
+            >>> b.update(recalc=False)
+            >>> # For specific cell(s):
+            >>> cell_specs_cell_01 = {"name_of_cell_01": {"recalc": False}}
+            >>> b.update(cell_specs=cell_specs_cell_01)
+
+        """
+
+        # TODO: implement experiment.last_cycle
+        accept_errors = accept_errors or self.accept_errors
+
+        debugging = kwargs.pop("debug", False)
+        testing = kwargs.pop("testing", False)
+
+        # --- cleaning up attributes / arguments etc ---
+        force_cellpy = kwargs.pop("force_cellpy", self.force_cellpy)
+        force_raw = kwargs.pop("force_raw", self.force_raw)
+
+        logging.info("[update experiment]")
+        if all_in_memory is not None:
+            self.all_in_memory = all_in_memory
+
+        logging.info(f"Additional keyword arguments: {kwargs}")
+        selector = kwargs.get("selector", None)
+
+        pages = self.journal.pages
+        if self.nom_cap:
+            warnings.warn(
+                "Setting nominal capacity through attributes will be deprecated soon since it modifies "
+                "the journal pages."
+            )
+            pages[hdr_journal.nom_cap] = self.nom_cap
+
+        if self.instrument:
+            warnings.warn(
+                "Setting instrument through attributes will be deprecated soon since it modifies the journal pages."
+            )
+            pages[hdr_journal.instrument] = self.instrument
+
+        if x := kwargs.pop("instrument", None):
+            warnings.warn(
+                "Setting instrument through params will be deprecated soon since it modifies the journal pages."
+                "Future version will require instrument in the journal pages."
+            )
+            pages[hdr_journal.instrument] = x
+
+        if pages.empty:
+            raise Exception("your journal is empty")
+
+        # --- init ---
+        summary_frames = dict()
+        cell_data_frames = dict()
+        number_of_runs = len(pages)
+        logging.debug(f"You have {number_of_runs} cells in your journal")
+        counter = 0
+        errors = []
+
+        pbar = tqdm(list(pages.iterrows()), file=sys.stdout, leave=False)
+
+        if debugging:
+            pbar = tqdm(list(pages.iterrows())[0:1], file=sys.stdout, leave=False)
+
+        # --- iterating ---
+        # TODO: create a multiprocessing pool and get one statusbar pr cell
+        for index, row in pbar:
+            counter += 1
+            h_txt = f"{index}"
+            n_txt = f"loading {counter}"
+            l_txt = f"starting to process file # {counter} ({index})"
+            pbar.set_description(n_txt, refresh=True)
+            cell_spec_page = self._get_cell_spec_from_page(index, row)
+
+            if cell_specs is not None:
+                cell_spec = cell_specs.get(index, dict())
+            else:
+                cell_spec = dict()
+
+            cell_spec = {**cell_spec_page, **kwargs, **cell_spec}
+            l_txt += f" cell_spec: {cell_spec}"
+            logging.debug(l_txt)
+
+            # --- UPDATING ARGUMENTS ---
+            filename = None
+            instrument = None
+            cellpy_file = OtherPath(row[hdr_journal.cellpy_file_name])
+            _cellpy_file = None
+            if not force_raw and cellpy_file.is_file():
+                _cellpy_file = cellpy_file
+                logging.debug(f"Got cellpy file: {_cellpy_file}")
+            if not force_cellpy:
+                filename = row[hdr_journal.raw_file_names]
+                instrument = row[hdr_journal.instrument]
+
+            cycle_mode = row[hdr_journal.cell_type]
+            mass = row[hdr_journal.mass]
+            nom_cap = row[hdr_journal.nom_cap]
+
+            loading = None
+            area = None
+            if hdr_journal.loading in row:
+                loading = row[hdr_journal.loading]
+            if hdr_journal.area in row:
+                area = row[hdr_journal.area]
+
+            summary_kwargs = {
+                "use_cellpy_stat_file": prms.Reader.use_cellpy_stat_file,
+            }
+
+            step_kwargs = {}
+            if not filename and not force_cellpy:
+                logging.info(
+                    f"Raw file(s) not given in the journal.pages for index={index}"
+                )
+                errors.append(index)
+                continue
+
+            elif not cellpy_file and force_cellpy:
+                logging.info(
+                    f"Cellpy file not given in the journal.pages for index={index}"
+                )
+                errors.append(index)
+                continue
+
+            else:
+                logging.info(f"Processing {index}")
+
+            logging.info("loading cell")
+            try:
+                logging.debug("inside try: running cellpy.get")
+                cell_data = cellpy.get(
+                    filename=filename,
+                    instrument=instrument,
+                    cellpy_file=_cellpy_file,
+                    cycle_mode=cycle_mode,
+                    mass=mass,
+                    nom_cap=nom_cap,
+                    loading=loading,
+                    area=area,
+                    step_kwargs=step_kwargs,
+                    summary_kwargs=summary_kwargs,
+                    selector=selector,
+                    logging_mode=logging_mode,
+                    testing=testing,
+                    **cell_spec,
+                )
+                logging.info("loaded cell")
+
+            except Exception as e:
+                logging.info("Failed to load: " + str(e))
+                errors.append("update:" + str(index))
+                h_txt += " [-]"
+                pbar.set_postfix_str(s=h_txt, refresh=True)
+                if not accept_errors:
+                    raise e
+                continue
+
+            if cell_data.empty:
+                logging.info("...not loaded...")
+                logging.debug("Data is empty. Could not load cell!")
+                errors.append("check:" + str(index))
+                h_txt += " [-]"
+                pbar.set_postfix_str(s=h_txt, refresh=True)
+                continue
+
+            logging.info("...loaded successfully...")
+            h_txt += " [OK]"
+            pbar.set_postfix_str(s=h_txt, refresh=True)
+            summary_tmp = cell_data.data.summary
+            logging.info("Trying to get summary_data")
+
+            if cell_data.data.steps is None or self.force_recalc:
+                logging.info("Running make_step_table")
+                n_txt = f"steps {counter}"
+                pbar.set_description(n_txt, refresh=True)
+                cell_data.make_step_table()
+
+            if summary_tmp is None or self.force_recalc:
+                logging.info("Running make_summary")
+                n_txt = f"summary {counter}"
+                pbar.set_description(n_txt, refresh=True)
+                cell_data.make_summary(find_end_voltage=True, find_ir=True)
+
+            # some clean-ups (might not be needed anymore):
+            if not summary_tmp.index.name == hdr_summary.cycle_index:
+                logging.debug("Setting index to Cycle_Index")
+                # check if it is a byte-string
+                if b"Cycle_Index" in summary_tmp.columns:
+                    logging.debug("Seems to be a byte-string in the column-headers")
+                    summary_tmp.rename(
+                        columns={b"Cycle_Index": "Cycle_Index"}, inplace=True
+                    )
+                try:
+                    summary_tmp.set_index("cycle_index", inplace=True)
+                except KeyError:
+                    logging.debug("cycle_index already an index")
+
+            summary_frames[index] = summary_tmp
+
+            if self.all_in_memory:
+                cell_data_frames[index] = cell_data
+            else:
+                cell_data_frames[index] = cellreader.CellpyCell(initialize=True)
+                cell_data_frames[index].data.steps = cell_data.data.steps
+
+            if self.save_cellpy:
+                logging.info("saving to cellpy-format")
+                n_txt = f"saving {counter}"
+                pbar.set_description(n_txt, refresh=True)
+                if self.custom_data_folder is not None:
+                    print("Save to custom data-folder not implemented yet")
+                    print(f"Saving to {row.cellpy_file_name} instead")
+                if not row.fixed:
+                    logging.info("saving cell to %s" % row.cellpy_file_name)
+                    cell_data.ensure_step_table = True
+                    try:
+                        cell_data.save(row.cellpy_file_name)
+                    except Exception as e:
+                        logging.error("saving file failed")
+                        logging.error(e)
+
+                else:
+                    logging.debug("saving cell skipped (set to 'fixed' in info_df)")
+            else:
+                logging.info("You opted to not save to cellpy-format")
+                logging.info("It is usually recommended to save to cellpy-format:")
+                logging.info(" >>> b.experiment.save_cellpy = True")
+                logging.info(
+                    "Without the cellpy-files, you cannot select specific cells"
+                )
+                logging.info("if you did not opt to store all in memory")
+
+            if self.export_raw or self.export_cycles:
+                export_text = "exporting"
+                if self.export_raw:
+                    export_text += " [raw]"
+                if self.export_cycles:
+                    export_text += " [cycles]"
+                logging.info(export_text)
+                n_txt = f"{export_text} {counter}"
+                pbar.set_description(n_txt, refresh=True)
+                cell_data.to_csv(
+                    self.journal.raw_dir,
+                    sep=prms.Reader.sep,
+                    cycles=self.export_cycles,
+                    shifted=self.shifted_cycles,
+                    raw=self.export_raw,
+                    last_cycle=self.last_cycle,
+                )
+
+            if self.export_ica:
+                logging.info("exporting [ica]")
+                try:
+                    helper.export_dqdv(
+                        cell_data,
+                        savedir=self.journal.raw_dir,
+                        sep=prms.Reader.sep,
+                        last_cycle=self.last_cycle,
+                    )
+                except Exception as e:
+                    logging.error("Could not make/export dq/dv data")
+                    logging.debug(
+                        "Failed to make/export " "dq/dv data (%s): %s" % (index, str(e))
+                    )
+                    errors.append("ica:" + str(index))
+
+        self.errors["update"] = errors
+        self.summary_frames = summary_frames
+        self.cell_data_frames = cell_data_frames
+
+    def parallel_update(
+        self, all_in_memory=None, cell_specs=None, logging_mode=None, **kwargs
+    ):
+        """Updates the selected datasets in parallel.
+
+        Args:
+            all_in_memory (bool): store the `cellpydata` in memory (default
+                False)
+            cell_specs (dict of dicts): individual arguments pr. cell. The `cellspecs` key-word argument
+                dictionary will override the **kwargs and the parameters from the journal pages
+                for the indicated cell.
+            logging_mode (str): sets the logging mode for the loader(s).
+
+            kwargs:
+                transferred all the way to the instrument loader, if not
+                picked up earlier. Remark that you can obtain the same pr. cell by
+                providing a `cellspecs` dictionary. The kwargs have precedence over the
+                parameters given in the journal pages, but will be overridden by parameters
+                given by `cellspecs`.
+
+                Merging:
+                    recalc (Bool): set to False if you don't want automatic "recalc" of
+                        cycle numbers etc. when merging several data-sets.
+                Loading:
+                    selector (dict): selector-based parameters sent to the cellpy-file loader (hdf5) if
+                    loading from raw is not necessary (or turned off).
+
+                Debugging:
+                    debug (Bool): set to True if you want to run in debug mode (should never be used by non-developers).
+
+        Debug-mode:
+                 - runs only for the first item in your journal
+
+        Examples:
+            >>> # Don't perform recalculation of cycle numbers etc. when merging
+            >>> # All cells:
+            >>> b.update(recalc=False)
+            >>> # For specific cell(s):
+            >>> cell_specs_cell_01 = {"name_of_cell_01": {"recalc": False}}
+            >>> b.update(cell_specs=cell_specs_cell_01)
+
+        """
+        status = "PROD"  # set this to DEV when developing this
+        async_mode = "threading"
+        logging.debug("PARALLEL UPDATE")
+        # TODO: implement experiment.last_cycle
+        if status != "DEV":
+            print("SORRY - MULTIPROCESSING IS NOT IMPLEMENTED PROPERLY YET")
+            return self.update(
+                all_in_memory=all_in_memory,
+                cell_specs=cell_specs,
+                logging_mode=logging_mode,
+                **kwargs,
+            )
+
+        import concurrent.futures
+        import multiprocessing
+
+        max_number_processes = multiprocessing.cpu_count()
+
+        if async_mode == "threading":
+            pool_executor = concurrent.futures.ThreadPoolExecutor
+        else:
+            pool_executor = concurrent.futures.ProcessPoolExecutor
+
+        debugging = kwargs.pop("debug", False)
+
+        # --- cleaning up attributes / arguments etc ---
+        force_cellpy = kwargs.pop("force_cellpy", self.force_cellpy)
+        force_raw = kwargs.pop("force_raw", self.force_raw)
+
+        logging.info("[update experiment]")
+        if all_in_memory is not None:
+            self.all_in_memory = all_in_memory
+
+        logging.info(f"Additional keyword arguments: {kwargs}")
+        selector = kwargs.get("selector", None)
+
+        pages = self.journal.pages
+        if self.nom_cap:
+            warnings.warn(
+                "Setting nominal capacity through attributes will be deprecated soon since it modifies "
+                "the journal pages."
+            )
+            pages[hdr_journal.nom_cap] = self.nom_cap
+
+        if self.instrument:
+            warnings.warn(
+                "Setting instrument through attributes will be deprecated soon since it modifies the journal pages."
+            )
+            pages[hdr_journal.instrument] = self.instrument
+
+        if x := kwargs.pop("instrument", None):
+            warnings.warn(
+                "Setting instrument through params will be deprecated soon since it modifies the journal pages."
+                "Future version will require instrument in the journal pages."
+            )
+            pages[hdr_journal.instrument] = x
+
+        if pages.empty:
+            raise Exception("your journal is empty")
+
+        # --- init ---
+        summary_frames = dict()
+        cell_data_frames = dict()
+        number_of_runs = len(pages)
+        logging.debug(f"You have {number_of_runs} cells in your journal")
+        counter = 0
+        errors = []
+
+        pbar = tqdm(list(pages.iterrows()), file=sys.stdout, leave=False)
+
+        if debugging:
+            pbar = tqdm(list(pages.iterrows())[0:1], file=sys.stdout, leave=False)
+
+        # --- iterating ---
+        # TODO: create a multiprocessing pool and get one statusbar pr cell
+        params = []
+        with pool_executor(max_number_processes) as executor:
+            for index, row in pages.iterrows():
+                counter += 1
+                cell_spec_page = self._get_cell_spec_from_page(index, row)
+
+                if cell_specs is not None:
+                    cell_spec = cell_specs.get(index, dict())
+                else:
+                    cell_spec = dict()
+
+                cell_spec = {**cell_spec_page, **kwargs, **cell_spec}
+
+                # --- UPDATING ARGUMENTS ---
+                filename = None
+                instrument = None
+                cellpy_file = OtherPath(row[hdr_journal.cellpy_file_name])
+                _cellpy_file = None
+                if not force_raw and cellpy_file.is_file():
+                    _cellpy_file = cellpy_file
+                    logging.debug(f"Got cellpy file: {_cellpy_file}")
+                if not force_cellpy:
+                    filename = row[hdr_journal.raw_file_names]
+                    instrument = row[hdr_journal.instrument]
+
+                cycle_mode = row[hdr_journal.cell_type]
+                mass = row[hdr_journal.mass]
+                nom_cap = row[hdr_journal.nom_cap]
+
+                loading = None
+                area = None
+                if hdr_journal.loading in row:
+                    loading = row[hdr_journal.loading]
+                if hdr_journal.area in row:
+                    area = row[hdr_journal.area]
+
+                summary_kwargs = {
+                    "use_cellpy_stat_file": prms.Reader.use_cellpy_stat_file,
+                }
+
+                step_kwargs = {}
+                if not filename and not force_cellpy:
+                    logging.info(
+                        f"Raw file(s) not given in the journal.pages for index={index}"
+                    )
+                    errors.append(index)
+                    continue
+
+                elif not cellpy_file and force_cellpy:
+                    logging.info(
+                        f"Cellpy file not given in the journal.pages for index={index}"
+                    )
+                    errors.append(index)
+                    continue
+
+                else:
+                    logging.info(f"Processing {index}")
+
+                logging.info("loading cell")
+                params.append(
+                    dict(
+                        filename=filename,
+                        instrument=instrument,
+                        cellpy_file=_cellpy_file,
+                        cycle_mode=cycle_mode,
+                        mass=mass,
+                        nom_cap=nom_cap,
+                        loading=loading,
+                        area=area,
+                        step_kwargs=step_kwargs,
+                        summary_kwargs=summary_kwargs,
+                        selector=selector,
+                        logging_mode=logging_mode,
+                        testing=False,
+                        **cell_spec,
+                    )
+                )
+
+            pool = [executor.submit(cellpy.get, **param) for param in params]
+            for i in concurrent.futures.as_completed(pool):
+                cell_data = i.result()
+                if cell_data.empty:
+                    logging.info("...not loaded...")
+                    logging.debug("Data is empty. Could not load cell!")
+                    errors.append("check:" + str(index))
+
+                logging.info("...loaded successfully...")
+                summary_tmp = cell_data.data.summary
+                logging.info("Trying to get summary_data")
+
+                if cell_data.data.steps is None or self.force_recalc:
+                    logging.info("Running make_step_table")
+                    cell_data.make_step_table()
+
+                if summary_tmp is None or self.force_recalc:
+                    logging.info("Running make_summary")
+                    cell_data.make_summary(find_end_voltage=True, find_ir=True)
+
+                # some clean-ups (might not be needed anymore):
+                if not summary_tmp.index.name == hdr_summary.cycle_index:
+                    logging.debug("Setting index to Cycle_Index")
+                    # check if it is a byte-string
+                    if b"Cycle_Index" in summary_tmp.columns:
+                        logging.debug("Seems to be a byte-string in the column-headers")
+                        summary_tmp.rename(
+                            columns={b"Cycle_Index": "Cycle_Index"}, inplace=True
+                        )
+                    try:
+                        summary_tmp.set_index("cycle_index", inplace=True)
+                    except KeyError:
+                        logging.debug("cycle_index already an index")
+
+                summary_frames[index] = summary_tmp
+
+                if self.all_in_memory:
+                    cell_data_frames[index] = cell_data
+                else:
+                    cell_data_frames[index] = cellreader.CellpyCell(initialize=True)
+                    cell_data_frames[index].data.steps = cell_data.data.steps
+
+                if self.save_cellpy:
+                    logging.info("saving to cellpy-format")
+                    n_txt = f"saving {counter}"
+                    pbar.set_description(n_txt, refresh=True)
+                    if self.custom_data_folder is not None:
+                        print("Save to custom data-folder not implemented yet")
+                        print(f"Saving to {row.cellpy_file_name} instead")
+                    if not row.fixed:
+                        logging.info("saving cell to %s" % row.cellpy_file_name)
+                        cell_data.ensure_step_table = True
+                        try:
+                            cell_data.save(row.cellpy_file_name)
+                        except Exception as e:
+                            logging.error("saving file failed")
+                            logging.error(e)
+
+                    else:
+                        logging.debug("saving cell skipped (set to 'fixed' in info_df)")
+                else:
+                    logging.info("You opted to not save to cellpy-format")
+                    logging.info("It is usually recommended to save to cellpy-format:")
+                    logging.info(" >>> b.experiment.save_cellpy = True")
+                    logging.info(
+                        "Without the cellpy-files, you cannot select specific cells"
+                    )
+                    logging.info("if you did not opt to store all in memory")
+
+                if self.export_raw or self.export_cycles:
+                    export_text = "exporting"
+                    if self.export_raw:
+                        export_text += " [raw]"
+                    if self.export_cycles:
+                        export_text += " [cycles]"
+                    logging.info(export_text)
+                    n_txt = f"{export_text} {counter}"
+                    pbar.set_description(n_txt, refresh=True)
+                    cell_data.to_csv(
+                        self.journal.raw_dir,
+                        sep=prms.Reader.sep,
+                        cycles=self.export_cycles,
+                        shifted=self.shifted_cycles,
+                        raw=self.export_raw,
+                        last_cycle=self.last_cycle,
+                    )
+
+                if self.export_ica:
+                    logging.info("exporting [ica]")
+                    try:
+                        helper.export_dqdv(
+                            cell_data,
+                            savedir=self.journal.raw_dir,
+                            sep=prms.Reader.sep,
+                            last_cycle=self.last_cycle,
+                        )
+                    except Exception as e:
+                        logging.error("Could not make/export dq/dv data")
+                        logging.debug(
+                            "Failed to make/export "
+                            "dq/dv data (%s): %s" % (index, str(e))
+                        )
+                        errors.append("ica:" + str(index))
+
+        self.errors["update"] = errors
+        self.summary_frames = summary_frames
+        self.cell_data_frames = cell_data_frames
+
+    def export_cellpy_files(self, path=None, **kwargs):
+        """Export all cellpy-files to a given path.
+
+        Remarks:
+            This method can only export to local folders
+            (OtherPath objects are not formally supported, but
+            might still work if the path is local).
+
+        Args:
+            path (str, pathlib.Path): path to export to (default: current working directory)
+        """
+        if path is None:
+            path = "."
+        errors = []
+        path = pathlib.Path(path)
+        cell_names = self.cell_names
+        for cell_name in cell_names:
+            cellpy_file_name = self.journal.pages.loc[
+                cell_name, hdr_journal.cellpy_file_name
+            ]
+            cellpy_file_name = path / pathlib.Path(cellpy_file_name).name
+            print(f"Exporting {cell_name} to {cellpy_file_name}")
+            try:
+                c = self.data[cell_name]
+            except TypeError as e:
+                errors.append(f"could not extract data for {cell_name} - linking")
+                self._link_cellpy_file(cell_name)
+
+            c.save(cellpy_file_name, **kwargs)
+        self.errors["export_cellpy_files"] = errors
+
+    @property
+    def cell_names(self):
+        """Returns a list of cell-names (strings)"""
+        try:
+            return [key for key in self.cell_data_frames]
+        except TypeError:
+            return None
+
+    def status(self):
+        print("\n")
+        print(" STATUS ".center(80, "="))
+        print(self)
+        print(" summary frames ".center(80, "-"))
+        if self.summary_frames is not None:
+            for key in self.summary_frames:
+                print(f" {{{key}}}")
+        print(" memory dumped ".center(80, "-"))
+        if self.memory_dumped is not None:
+            for key in self.memory_dumped:
+                print(f"{key}: {type(self.memory_dumped[key])}")
+        print(80 * "=")
+
+    def link(self, **kwargs):
+        """Ensure that an appropriate link to the cellpy-files exists for
+        each cell.
+
+        The experiment will then contain a CellpyCell object for each cell
+        (in the cell_data_frames attribute) with only the step-table stored.
+
+        Remark that running update persists the summary frames instead (or
+        everything in case you specify all_in_memory=True).
+        This might be considered "a strange and unexpected behaviour". Sorry
+        for that (but the authors of this package is also a bit strange...).
+
+        (OK, I will change it. Soon.)
+
+        **kwargs: passed to _link_cellpy_file
+            max_cycle (int): maximum cycle number to link/load (remark that the
+                cellpy objects will get the property overwrite_able set to False
+                if you give a max_cycle to prevent accidentally saving a "truncated"
+                file (use c.save(filename, overwrite=True) to force overwrite))
+
+
+        """
+        logging.info("[establishing links]")
+        logging.debug("checking and establishing link to data")
+
+        errors = []
+
+        for cell_label in self.journal.pages.index:
+            logging.debug(f"trying to link {cell_label}")
+            try:
+                self._link_cellpy_file(cell_label, **kwargs)
+            except IOError as e:
+                logging.warning(e)
+                e_txt = f"{cell_label}: links not established - try update instead"
+                logging.warning(e_txt)
+                errors.append(e_txt)
+
+        self.errors["link"] = errors
+
+    def recalc(
+        self,
+        save=True,
+        step_opts=None,
+        summary_opts=None,
+        indexes=None,
+        calc_steps=True,
+        testing=False,
+    ):
+        """Run make_step_table and make_summary on all cells.
+
+        Args:
+            save (bool): Save updated cellpy-files if True.
+            step_opts (dict): parameters to inject to make_steps.
+            summary_opts (dict): parameters to inject to make_summary.
+            indexes (list): Only recalculate for given indexes (i.e. list of cell-names).
+            calc_steps (bool): Run make_steps before making the summary.
+            testing (bool): Only for testing purposes.
+
+        Returns:
+            None
+        """
+
+        # TODO: option (default) to only recalc if the values (mass, nom_cap,...) have changed
+        errors = []
+        log = []
+        if testing:
+            pbar = tqdm(
+                list(self.journal.pages.iloc[0:2, :].iterrows()),
+                file=sys.stdout,
+                leave=False,
+            )
+        elif indexes is not None:
+            pbar = tqdm(
+                list(self.journal.pages.loc[indexes, :].iterrows()),
+                file=sys.stdout,
+                leave=False,
+            )
+        else:
+            pbar = tqdm(
+                list(self.journal.pages.iterrows()), file=sys.stdout, leave=False
+            )
+        for indx, row in pbar:
+            nom_cap = row[hdr_journal.nom_cap]
+            mass = row[hdr_journal.mass]
+            pbar.set_description(indx)
+            try:
+                c = self.data[indx]
+            except TypeError as e:
+                e_txt = (
+                    f"could not extract data for {indx} - have you forgotten to link?"
+                )
+                errors.append(e_txt)
+                warnings.warn(e_txt)
+
+            else:
+                if nom_cap:
+                    c.set_nom_cap(nom_cap)
+                if mass:
+                    c.set_mass(mass)
+                try:
+                    if calc_steps:
+                        pbar.set_postfix_str(s="steps", refresh=True)
+                        if step_opts is not None:
+                            c.make_step_table(**step_opts)
+                        else:
+                            c.make_step_table()
+
+                    pbar.set_postfix_str(s="summary", refresh=True)
+                    if summary_opts is not None:
+                        c.make_summary(**summary_opts)
+                    else:
+                        c.make_summary(find_end_voltage=True, find_ir=True)
+
+                except Exception as e:
+                    e_txt = f"recalculating for {indx} failed!"
+                    errors.append(e_txt)
+                    warnings.warn(e_txt)
+                else:
+                    if save:
+                        # remark! got a win error when trying to save (hdf5-file in use) (must fix this)
+                        pbar.set_postfix_str(s="save", refresh=True)
+                        try:
+                            c.save(row.cellpy_file_name)
+                            log.append(f"saved {indx} to {row.cellpy_file_name}")
+                        except Exception as e:
+                            e_txt = f"saving {indx} to {row.cellpy_file_name} failed!"
+                            errors.append(e_txt)
+                            warnings.warn(e_txt)
+        self.errors["recalc"] = errors
+        self.log["recalc"] = log
+
+
+class ImpedanceExperiment(BaseExperiment):
+    def __init__(self):
+        super().__init__()
+
+
+class LifeTimeExperiment(BaseExperiment):
+    def __init__(self):
+        super().__init__()
+
+
+if __name__ == "__main__":
+    from pathlib import Path
+    import os
+    import pandas as pd
+    import numpy as np
+    import seaborn as sns
+    import plotly.express as px
+
+    import cellpy
+    from cellpy.utils import batch, helpers, plotutils
+
+    project_dir = Path("../../../testdata/batch_project")
+    print(f"{project_dir.resolve()=}")
+    journal = project_dir / "test_project.json"
+    journal = journal.resolve()
+    print(f"{journal=}")
+    assert project_dir.is_dir()
+    assert journal.is_file()
+    os.chdir(project_dir)
+
+    print(f"cellpy version: {cellpy.__version__}")
+    cellpy.log.setup_logging("INFO")
+
+    b = batch.from_journal(journal)
+    b.update()
+
+    print("Ended OK")
```

### Comparing `cellpy-1.0.0a0/cellpy/utils/batch_tools/batch_exporters.py` & `cellpy-1.0.0a3/cellpy/utils/batch_tools/batch_exporters.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/cellpy/utils/batch_tools/batch_journals.py` & `cellpy-1.0.0a3/cellpy/utils/batch_tools/batch_journals.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,785 +1,789 @@
-import json
-import logging
-import os
-import pathlib
-import platform
-import shutil
-import tempfile
-import warnings
-from abc import ABC
-
-import pandas as pd
-
-from cellpy.exceptions import UnderDefined
-from cellpy.parameters import prms
-from cellpy.parameters.internal_settings import (
-    get_headers_journal,
-    keys_journal_session,
-)
-from cellpy.parameters.legacy.update_headers import (
-    headers_journal_v0 as hdr_journal_old,
-)
-from cellpy.readers import dbreader
-from cellpy.utils.batch_tools.batch_core import BaseJournal
-from cellpy.utils.batch_tools.engines import simple_db_engine, sql_db_engine
-
-hdr_journal = get_headers_journal()
-
-trans_dict = {}
-missing_keys = []
-for key in hdr_journal:
-    if key in hdr_journal_old:
-        trans_dict[hdr_journal_old[key]] = hdr_journal[key]
-    else:
-        missing_keys.append(key)
-
-
-class LabJournal(BaseJournal, ABC):
-    def __init__(self, db_reader="default", engine=None, batch_col=None, **kwargs):
-        """Journal for selected batch.
-
-        The journal contains pages (pandas.DataFrame) with prms for
-        each cell (one cell pr row).
-
-        Args:
-            db_reader: either default (a simple excel reader already
-                implemented in cellpy) or other db readers that implement
-                the needed API.
-            engine: defaults to simple_db_engine for parsing db using the
-                db_reader
-                    self.pages = simple_db_engine(
-                        self.db_reader, id_keys, **kwargs
-                    )
-            batch_col: the column name for the batch column in the db (used by simple_db_engine).
-            **kwargs: passed to the db_reader
-        """
-
-        super().__init__()
-        if db_reader is None:
-            return
-
-        if isinstance(db_reader, str):
-            if db_reader == "off":
-                self.db_reader = None
-                return
-            if db_reader == "default":
-                db_reader = prms.Db.db_type
-            if db_reader == "simple_excel_reader":
-                self.db_reader = dbreader.Reader()
-                self.engine = simple_db_engine
-            elif db_reader == "sql_db_reader":
-                raise NotImplementedError("sql_db_reader is not implemented yet")
-                # self.db_reader = sql_dbreader.SqlReader()
-                # self.engine = sql_db_engine
-            else:
-                raise UnderDefined(f"The db-reader '{db_reader}' is not supported")
-        else:
-            logging.debug(f"Remark! db_reader: {db_reader}")
-            self.db_reader = db_reader
-
-        if engine is None:
-            self.engine = simple_db_engine
-
-        self.batch_col = batch_col or "b01"
-
-    def _repr_html_(self):
-        txt = f"<h2>LabJournal-object</h2> id={hex(id(self))}"
-        txt += "<h3>Main attributes</h3>"
-        txt += f"""
-        <table>
-            <thead>
-                <tr>
-                    <th>Attribute</th>
-                    <th>Value</th>
-                </tr>
-            </thead>
-            <tbody>
-                <tr><td><b>name</b></td><td>{self.name}</td></tr>
-                <tr><td><b>project</b></td><td>{self.project}</td></tr>
-                <tr><td><b>file_name</b></td><td>{self.file_name}</td></tr>
-                <tr><td><b>db_reader</b></td><td>{self.db_reader}</td></tr>
-        """
-        if self.db_reader == "default":
-            txt += f"<tr><td><b>batch_col</b></td><td>{self.batch_col}</td></tr>"
-        txt += f"""
-                <tr><td><b>time_stamp</b></td><td>{self.time_stamp}</td></tr>
-                <tr><td><b>project_dir</b></td><td>{self.project_dir}</td></tr>
-                <tr><td><b>raw_dir</b></td><td>{self.raw_dir}</td></tr>
-                <tr><td><b>batch_dir</b></td><td>{self.batch_dir}</td></tr>
-            </tbody>
-        </table>
-        """
-        txt += "<h3>Session info</h3>"
-        for key in self.session:
-            txt += f"<p><b>{key}</b>: {self.session[key]}</p>"
-
-        txt += "<h3>Pages</h3>"
-        try:
-            txt += self.pages._repr_html_()  # pylint: disable=protected-access
-        except AttributeError:
-            txt += "<p><b>pages</b><br> not found!</p>"
-        except ValueError:
-            txt += "<p><b>pages</b><br> not readable!</p>"
-        return txt
-
-    def _check_file_name(self, file_name, to_project_folder=False):
-        if file_name is None:
-            if not self.file_name:
-                self.generate_file_name()
-            file_name = pathlib.Path(self.file_name)
-
-        else:
-            file_name = pathlib.Path(file_name)
-        if to_project_folder:
-            file_name = file_name.with_suffix(".json").name
-            project_dir = pathlib.Path(self.project_dir)
-
-            file_name = project_dir / file_name
-        self.file_name = file_name  # updates object (maybe not smart)
-        return file_name
-
-    def from_db(self, project=None, name=None, batch_col=None, **kwargs):
-        """populate journal from db.
-
-        Args:
-            project (str): project name.
-            name (str): experiment name.
-            batch_col (int): batch column.
-
-        **kwargs: sent to engine.
-
-        simple_db-engine -> filefinder.search_for_files:
-            run_name(str): run-file identification.
-            raw_extension(str): optional, extension of run-files (without the '.').
-            cellpy_file_extension(str): optional, extension for cellpy files
-                (without the '.').
-            raw_file_dir(path): optional, directory where to look for run-files
-                (default: read prm-file)
-            cellpy_file_dir(path): optional, directory where to look for
-                cellpy-files (default: read prm-file)
-            prm_filename(path): optional parameter file can be given.
-            file_name_format(str): format of raw-file names or a glob pattern
-                (default: YYYYMMDD_[name]EEE_CC_TT_RR) [not finished yet].
-            reg_exp(str): use regular expression instead (defaults to None) [not finished yet].
-            sub_folders (bool): perform search also in sub-folders.
-            file_list (list of str): perform the search within a given list
-                of filenames instead of searching the folder(s). The list should
-                not contain the full filepath (only the actual file names). If
-                you want to provide the full path, you will have to modify the
-                file_name_format or reg_exp accordingly.
-            pre_path (path or str): path to prepend the list of files selected
-                 from the file_list.
-
-        Returns:
-            None
-        """
-        logging.debug("creating journal from db")
-        if batch_col is None:
-            batch_col = self.batch_col
-        if project is not None:
-            self.project = project
-        if name is None:
-            name = self.name
-        else:
-            self.name = name
-        logging.debug(f"batch_name, batch_col: {name}, {batch_col}")
-
-        if self.db_reader is not None:
-            if isinstance(self.db_reader, dbreader.Reader):  # Simple excel-db
-                id_keys = self.db_reader.select_batch(name, batch_col)
-                self.pages = self.engine(self.db_reader, id_keys, **kwargs)
-            else:
-                logging.debug(
-                    "creating journal pages using advanced reader methods (not simple excel-db)"
-                )
-                self.pages = self.engine(self.db_reader, batch_name=name, **kwargs)
-
-            if self.pages.empty:
-                logging.critical(
-                    f"EMPTY JOURNAL: are you sure you have provided correct input to batch?"
-                )
-                logging.critical(f"name: {name}")
-                logging.critical(f"project: {self.project}")
-                logging.critical(f"batch_col: {batch_col}")
-        else:
-            logging.debug("creating empty journal pages")
-            self.pages = pd.DataFrame()
-
-        self.generate_empty_session()
-        self.generate_folder_names()
-        self.paginate()
-
-    def generate_empty_session(self):
-        self.session = {}
-        for item in keys_journal_session:
-            self.session[item] = None
-
-    @staticmethod
-    def _fix_cellpy_paths(p):
-        if platform.system() != "Windows":
-            if p.find("\\") >= 0:
-                # convert from win to posix
-                p = pathlib.PureWindowsPath(p)
-        else:
-            if p.find("/") >= 0:
-                # convert from posix to win
-                p = pathlib.PurePosixPath(p)
-        return pathlib.Path(p)
-
-    @classmethod
-    def read_journal_jason_file(cls, file_name, **kwargs):
-        logging.debug(f"json loader starting on {file_name}")
-        with open(file_name, "r") as infile:
-            top_level_dict = json.load(infile)
-        pages_dict = top_level_dict["info_df"]
-        meta = top_level_dict["metadata"]
-        session = top_level_dict.get("session", None)
-        pages = pd.DataFrame(pages_dict)
-        if pages.empty:
-            logging.critical("could not find any pages in the journal")
-            raise UnderDefined
-
-        pages = cls._clean_pages(pages)
-
-        if session is None:
-            logging.debug(f"no session - generating empty one")
-            session = dict()
-
-        session, pages = cls._clean_session(session, pages)
-
-        return pages, meta, session
-
-    @classmethod
-    def read_journal_excel_file(cls, file_name, **kwargs):
-        sheet_names = {"meta": "meta", "pages": "pages", "session": "session"}
-        project = kwargs.pop("project", "NaN")
-        name = kwargs.pop("batch", pathlib.Path(file_name).stem)
-        _meta = {
-            "name": name,
-            "project": project,
-            "project_dir": pathlib.Path("."),
-            "batch_dir": pathlib.Path("."),
-            "raw_dir": pathlib.Path("."),
-        }
-        logging.debug(f"xlsx loader starting on {file_name}")
-
-        meta_sheet_name = sheet_names["meta"]  # not tested yet
-        pages_sheet_name = sheet_names["pages"]
-        session_sheet_name = sheet_names["session"]  # not tested yet
-
-        temporary_directory = tempfile.mkdtemp()
-        temporary_file_name = shutil.copy(file_name, temporary_directory)
-        try:
-            pages = pd.read_excel(
-                temporary_file_name, engine="openpyxl", sheet_name=pages_sheet_name
-            )
-        except KeyError:
-            print(f"Worksheet '{pages_sheet_name}' does not exist.")
-            return None
-
-        try:
-            session = pd.read_excel(
-                temporary_file_name,
-                sheet_name=session_sheet_name,
-                engine="openpyxl",
-                header=[0, 1],
-            )
-        except (KeyError, ValueError):
-            print(f"Worksheet '{session_sheet_name}' does not exist.")
-            session = None
-
-        try:
-            meta = pd.read_excel(
-                temporary_file_name, sheet_name=meta_sheet_name, engine="openpyxl"
-            )
-
-        except (KeyError, ValueError):
-            print(f"Worksheet '{meta_sheet_name}' does not exist.")
-            meta = None
-
-        if pages.empty:
-            logging.critical("could not find any pages in the journal")
-            raise UnderDefined
-        pages = cls._clean_pages(pages)
-        pages = pages.set_index(hdr_journal.filename)
-
-        if meta is None:
-            meta = _meta
-        else:
-            meta = cls._unpack_meta(meta) or _meta
-
-        if session is None:
-            logging.debug(f"no session - generating empty one")
-            session = dict()
-        else:
-            session = cls._unpack_session(session)
-
-        session, pages = cls._clean_session(session, pages)
-
-        return pages, meta, session
-
-    @classmethod
-    def _unpack_session(cls, session):
-        try:
-            bcn2 = {
-                l: list(sb["cycle_index"].values)
-                for l, sb in session["bad_cycles"].groupby("cell_name")
-            }
-        except KeyError:
-            bcn2 = []
-
-        try:
-            bc2 = list(session["bad_cells"]["cell_name"].dropna().values.flatten())
-        except KeyError:
-            bc2 = []
-
-        try:
-            s2 = list(session["starred"]["cell_name"].dropna().values.flatten())
-        except KeyError:
-            s2 = []
-
-        try:
-            n2 = list(session["notes"]["txt"].dropna().values.flatten())
-        except KeyError:
-            n2 = []
-
-        session = {"bad_cycles": bcn2, "bad_cells": bc2, "starred": s2, "notes": n2}
-
-        return session
-
-    @classmethod
-    def _unpack_meta(cls, meta):
-        try:
-            meta = meta.loc[:, ["parameter", "value"]]
-        except KeyError:
-            return
-        meta = meta.set_index("parameter")
-        return meta.to_dict()["value"]
-
-    @classmethod
-    def _clean_session(cls, session, pages):
-        # include steps for cleaning up the session dict here
-        if not session:
-            logging.critical("no session found in your journal file")
-        for item in keys_journal_session:
-            session[item] = session.get(item, None)
-
-        return session, pages
-
-    @classmethod
-    def _clean_pages(cls, pages: pd.DataFrame) -> pd.DataFrame:
-        import ast
-
-        logging.debug("removing empty rows")
-        pages = pages.dropna(how="all")
-        logging.debug("checking path-names")
-        try:
-            p = pages[hdr_journal.raw_file_names]
-            new_p = []
-            for f in p:
-                if isinstance(f, str):
-                    try:
-                        new_f = ast.literal_eval(f"'{f}'")
-                        if isinstance(new_f, list):
-                            f = new_f
-                    except Exception as e:
-                        warnings.warn(e)
-                        warnings.warn(f"Could not evaluate {f}")
-
-                new_p.append(f)
-            pages[hdr_journal.raw_file_names] = new_p
-
-        except KeyError:
-            print(
-                "Tried but failed in converting raw_file_names into an appropriate list"
-            )
-        try:
-            pages[hdr_journal.cellpy_file_name] = pages[
-                hdr_journal.cellpy_file_name
-            ].apply(cls._fix_cellpy_paths)
-        except KeyError:
-            # assumes it is an old type journal file
-            print(f"The key '{hdr_journal.cellpy_file_name}' is missing!")
-            print(f"Assumes that this is an old-type journal file.")
-            try:
-                pages.rename(columns=trans_dict, inplace=True)
-                pages[hdr_journal.cellpy_file_name] = pages[
-                    hdr_journal.cellpy_file_name
-                ].apply(cls._fix_cellpy_paths)
-                logging.warning("old journal file - updating")
-            except KeyError:
-                print("Error! Could still not parse the pages.")
-                print(f"Missing key: {hdr_journal.cellpy_file_name}")
-                pages[hdr_journal.cellpy_file_name] = None
-
-        # only keep selected cells if keep column exists
-        if "keep" in pages.columns:
-            logging.debug("Journal contains 'keep' - selecting only 'keep' > 0.")
-            pages = pages.loc[pages.keep > 0, :]
-
-        for column_name in missing_keys:
-            if column_name not in pages.columns:
-                logging.debug(f"wrong journal format - missing: {column_name}")
-                pages[column_name] = None
-
-        for column_name in hdr_journal:
-            if column_name not in pages.columns:
-                if column_name != hdr_journal.filename:
-                    pages[column_name] = None
-
-        return pages
-
-    def from_file(self, file_name=None, paginate=True, **kwargs):
-        """Loads a DataFrame with all the needed info about the experiment"""
-        file_name = self._check_file_name(file_name)
-        logging.info(f"reading {file_name}")
-        if pathlib.Path(file_name).suffix.lower() == ".xlsx":
-            file_loader = self.read_journal_excel_file
-        else:
-            file_loader = self.read_journal_jason_file
-        try:
-            out = file_loader(file_name, **kwargs)
-            if out is None:
-                raise IOError(f"Error reading {file_name}.")
-            pages, meta_dict, session = out
-        except UnderDefined as e:
-            logging.critical(f"could not load {file_name}")
-            raise UnderDefined from e
-
-        logging.debug(f"got pages and meta_dict")
-
-        self.pages = pages
-        self.session = session
-        self.file_name = file_name
-        self._prm_packer(meta_dict)
-
-        if paginate:
-            self.generate_folder_names()
-            self.paginate()
-
-    def from_frame(self, frame, name=None, project=None, paginate=None, **kwargs):
-        if name is not None:
-            self.name = name
-        if project is not None:
-            self.project = project
-
-        self.pages = (
-            frame  # TODO: include a check here to see if the pages are appropriate
-        )
-        for hdr in hdr_journal.values():
-            if hdr not in self.pages.columns:
-                self.pages[hdr] = None
-
-        if hdr_journal.filename in self.pages.columns:
-            self.pages = self.pages.set_index(hdr_journal.filename)
-
-        if paginate is None:
-            if self.name and self.project:
-                paginate = True
-
-        if paginate:
-            logging.critical(f"paginating {project}/{name} ")
-            self.generate_folder_names()
-            self.paginate()
-
-    def from_file_old(self, file_name=None):
-        """Loads a DataFrame with all the needed info about the experiment"""
-
-        file_name = self._check_file_name(file_name)
-
-        with open(file_name, "r") as infile:
-            top_level_dict = json.load(infile)
-
-        pages_dict = top_level_dict["info_df"]
-        pages = pd.DataFrame(pages_dict)
-        pages[hdr_journal.cellpy_file_name] = pages[hdr_journal.cellpy_file_name].apply(
-            self._fix_cellpy_paths
-        )
-        self.pages = pages
-        self.file_name = file_name
-        self._prm_packer(top_level_dict["metadata"])
-        self.generate_folder_names()
-        self.paginate()
-
-    def create_empty_pages(self, description=None):
-        if description is not None:
-            print(f"Creating from {type(description)} is not implemented yet")
-
-        logging.debug("Creating an empty journal")
-        logging.debug(f"name: {self.name}")
-        logging.debug(f"project: {self.project}")
-
-        col_names = list(hdr_journal.values())
-        pages = pd.DataFrame(columns=col_names)
-        pages.set_index(hdr_journal.filename, inplace=True)
-        return pages
-
-    def duplicate_journal(self, folder=None) -> None:
-        """Copy the journal to folder.
-
-        Args:
-            folder (str or pathlib.Path): folder to copy to (defaults to the
-            current folder).
-        """
-
-        logging.debug(f"duplicating journal to folder {folder}")
-        journal_name = pathlib.Path(self.file_name)
-        if not journal_name.is_file():
-            logging.info("No journal saved")
-            return
-        new_journal_name = journal_name.name
-        if folder is not None:
-            new_journal_name = pathlib.Path(folder) / new_journal_name
-        try:
-            shutil.copy(journal_name, new_journal_name)
-        except shutil.SameFileError:
-            logging.debug("same file exception encountered")
-
-    def to_file(
-        self,
-        file_name=None,
-        paginate=True,
-        to_project_folder=True,
-        duplicate_to_local_folder=True,
-    ):
-        """Saves a DataFrame with all the needed info about the experiment.
-
-        Args:
-            file_name (str or pathlib.Path): journal file name (.json or .xlsx)
-            paginate (bool): make project folders
-            to_project_folder (bool): save journal file to the folder containing your cellpy projects
-            duplicate_to_local_folder (bool): save journal file to the folder you are in now also
-
-        Returns:
-            None
-        """
-        file_name = self._check_file_name(
-            file_name, to_project_folder=to_project_folder
-        )
-
-        pages = self.pages
-        session = self.session
-        meta = self._prm_packer()
-        top_level_dict = {"info_df": pages, "metadata": meta, "session": session}
-
-        is_json = False
-        is_xlsx = False
-
-        if file_name.suffix == ".xlsx":
-            is_xlsx = True
-
-        if file_name.suffix == ".json":
-            is_json = True
-
-        if is_xlsx:
-            df_session = self._pack_session(session)
-            df_meta = self._pack_meta(meta)
-
-            try:
-                pages.index.name = "filename"
-                with pd.ExcelWriter(file_name, mode="w", engine="openpyxl") as writer:
-                    pages.to_excel(writer, sheet_name="pages", engine="openpyxl")
-                    # no index is not supported for multi-index (update to index=False when pandas implement it):
-                    df_session.to_excel(writer, sheet_name="session", engine="openpyxl")
-                    df_meta.to_excel(
-                        writer, sheet_name="meta", engine="openpyxl", index=False
-                    )
-            except PermissionError as e:
-                print(f"Could not load journal to xlsx ({e})")
-
-        if is_json:
-            jason_string = json.dumps(
-                top_level_dict,
-                default=lambda info_df: json.loads(
-                    info_df.to_json(default_handler=str)
-                ),
-            )
-
-            with open(file_name, "w") as outfile:
-                outfile.write(jason_string)
-
-        self.file_name = file_name
-        logging.info(f"Saved file to {file_name}")
-
-        if paginate:
-            self.paginate()
-
-        if duplicate_to_local_folder:
-            self.duplicate_journal()
-
-    @staticmethod
-    def _pack_session(session):
-        frames = []
-        keys = []
-        try:
-            l_bad_cycle_numbers = []
-
-            for k, v in session["bad_cycles"].items():
-                l_bad_cycle_numbers.append(pd.DataFrame(data=v, columns=[k]))
-
-            df_bad_cycle_numbers = (
-                pd.concat(l_bad_cycle_numbers, axis=1)
-                .melt(var_name="cell_name", value_name="cycle_index")
-                .dropna()
-            )
-            frames.append(df_bad_cycle_numbers)
-            keys.append("bad_cycles")
-        except (KeyError, AttributeError):
-            logging.debug("missing bad cycle numbers")
-
-        df_bad_cells = pd.DataFrame(session["bad_cells"], columns=["cell_name"])
-        frames.append(df_bad_cells)
-        keys.append("bad_cells")
-
-        df_starred = pd.DataFrame(session["starred"], columns=["cell_name"])
-        frames.append(df_starred)
-        keys.append("starred")
-
-        df_notes = pd.DataFrame(session["notes"], columns=["txt"])
-        frames.append(df_notes)
-        keys.append("notes")
-
-        session = pd.concat(frames, axis=1, keys=keys)
-        return session
-
-    @staticmethod
-    def _pack_meta(meta):
-        meta = pd.DataFrame(meta, index=[0]).melt(
-            var_name="parameter", value_name="value"
-        )
-        return meta
-
-    def generate_folder_names(self):
-        """Set appropriate folder names."""
-        logging.debug("creating folder names")
-        if self.project and isinstance(self.project, (pathlib.Path, str)):
-            logging.debug("got project name")
-            logging.debug(self.project)
-            self.project_dir = os.path.join(prms.Paths.outdatadir, self.project)
-        else:
-            logging.critical(
-                "Could not create project dir (missing project definition)"
-            )
-        if self.name:
-            self.batch_dir = os.path.join(self.project_dir, self.name)
-            self.raw_dir = os.path.join(self.batch_dir, "raw_data")
-        else:
-            logging.critical(
-                "Could not create batch_dir and raw_dir", "(missing batch name)"
-            )
-        logging.debug(f"batch dir: {self.batch_dir}")
-        logging.debug(f"project dir: {self.project_dir}")
-        logging.debug(f"raw dir: {self.raw_dir}")
-
-    def paginate(self):
-        """Make folders where we would like to put results etc."""
-
-        project_dir = self.project_dir
-        raw_dir = self.raw_dir
-        batch_dir = self.batch_dir
-
-        if project_dir is None:
-            raise UnderDefined("no project directory defined")
-        if raw_dir is None:
-            raise UnderDefined("no raw directory defined")
-        if batch_dir is None:
-            raise UnderDefined("no batch directory defined")
-
-        # create the folders
-        if not os.path.isdir(project_dir):
-            os.mkdir(project_dir)
-            logging.info(f"created folder {project_dir}")
-        if not os.path.isdir(batch_dir):
-            os.mkdir(batch_dir)
-            logging.info(f"created folder {batch_dir}")
-        if not os.path.isdir(raw_dir):
-            os.mkdir(raw_dir)
-            logging.info(f"created folder {raw_dir}")
-
-        self.project_dir = project_dir
-        self.batch_dir = batch_dir
-        self.raw_dir = raw_dir
-
-        return project_dir, batch_dir, raw_dir
-
-    def generate_file_name(self):
-        """generate a suitable file name for the experiment"""
-        if not self.project:
-            raise UnderDefined("project name not given")
-        out_data_dir = prms.Paths.outdatadir
-        project_dir = os.path.join(out_data_dir, self.project)
-        file_name = f"cellpy_batch_{self.name}.json"
-        self.file_name = os.path.join(project_dir, file_name)
-
-    # v.1.0.0:
-    def look_for_file(self):
-        pass
-
-    def get_column(self, header):
-        """populate new column from db"""
-        pass
-
-    def get_cell(self, id_key):
-        """get additional cell info from db"""
-        pass
-
-    def add_comment(self, comment):
-        """add a comment (will be saved in the journal file)"""
-        pass
-
-    def remove_comment(self, comment_id):
-        pass
-
-    def view_comments(self):
-        pass
-
-    def remove_cell(self, cell_id):
-        pass
-
-    def add_cell(self, cell_id, **kwargs):
-        """Add a cell to the pages"""
-        pass
-
-
-def _dev_journal_loading():
-    from cellpy import log
-
-    log.setup_logging(default_level="DEBUG")
-    journal_file = pathlib.Path(
-        "../../../testdata/batch_project/test_project.json"
-    ).resolve()
-    assert journal_file.is_file()
-
-    logging.debug(f"reading journal file {journal_file}")
-    journal = LabJournal(db_reader=None)
-    journal.from_file(journal_file, paginate=False)
-    print(80 * "-")
-    print(journal.pages)
-    print(80 * "-")
-    print(journal.session)
-
-    # creating a mock session
-    bad_cycle_numbers = {
-        "20160805_test001_45_cc": [4, 337, 338],
-        "20160805_test001_47_cc": [7, 8, 9],
-    }
-    bad_cells = ["20160805_test001_45_cc"]
-
-    notes = {"date_stamp": "one comment for the road", "date_stamp2": "another comment"}
-    session = {
-        "bad_cycle_numbers": bad_cycle_numbers,
-        "bad_cells": bad_cells,
-        "notes": notes,
-    }
-
-    # journal.session = session
-
-    new_journal_name = journal_file.with_name(f"{journal_file.stem}_tmp.xlsx")
-    print(new_journal_name)
-    journal.to_file(file_name=new_journal_name, paginate=False, to_project_folder=False)
-
-
-if __name__ == "__main__":
-    print(" running journal ".center(80, "-"))
-    _dev_journal_loading()
-    print(" finished ".center(80, "-"))
+import json
+import logging
+import os
+import pathlib
+import platform
+import shutil
+import tempfile
+import warnings
+from abc import ABC
+
+import pandas as pd
+
+from cellpy.exceptions import UnderDefined
+from cellpy.parameters import prms
+from cellpy.parameters.internal_settings import (
+    get_headers_journal,
+    keys_journal_session,
+)
+from cellpy.parameters.legacy.update_headers import (
+    headers_journal_v0 as hdr_journal_old,
+)
+from cellpy.readers import dbreader
+from cellpy.utils.batch_tools.batch_core import BaseJournal
+from cellpy.utils.batch_tools.engines import simple_db_engine, sql_db_engine
+
+hdr_journal = get_headers_journal()
+
+trans_dict = {}
+missing_keys = []
+for key in hdr_journal:
+    if key in hdr_journal_old:
+        trans_dict[hdr_journal_old[key]] = hdr_journal[key]
+    else:
+        missing_keys.append(key)
+
+
+class LabJournal(BaseJournal, ABC):
+    def __init__(self, db_reader="default", engine=None, batch_col=None, **kwargs):
+        """Journal for selected batch.
+
+        The journal contains pages (pandas.DataFrame) with prms for
+        each cell (one cell pr row).
+
+        Args:
+            db_reader: either default (a simple excel reader already
+                implemented in cellpy) or other db readers that implement
+                the needed API.
+            engine: defaults to simple_db_engine for parsing db using the
+                db_reader
+                    self.pages = simple_db_engine(
+                        self.db_reader, id_keys, **kwargs
+                    )
+            batch_col: the column name for the batch column in the db (used by simple_db_engine).
+            **kwargs: passed to the db_reader
+        """
+
+        super().__init__()
+        if db_reader is None:
+            return
+
+        if isinstance(db_reader, str):
+            if db_reader == "off":
+                self.db_reader = None
+                return
+            if db_reader == "default":
+                db_reader = prms.Db.db_type
+            if db_reader == "simple_excel_reader":
+                self.db_reader = dbreader.Reader()
+                self.engine = simple_db_engine
+            elif db_reader == "sql_db_reader":
+                raise NotImplementedError("sql_db_reader is not implemented yet")
+                # self.db_reader = sql_dbreader.SqlReader()
+                # self.engine = sql_db_engine
+            else:
+                raise UnderDefined(f"The db-reader '{db_reader}' is not supported")
+        else:
+            logging.debug(f"Remark! db_reader: {db_reader}")
+            self.db_reader = db_reader
+
+        if engine is None:
+            self.engine = simple_db_engine
+
+        self.batch_col = batch_col or "b01"
+
+    def _repr_html_(self):
+        txt = f"<h2>LabJournal-object</h2> id={hex(id(self))}"
+        txt += "<h3>Main attributes</h3>"
+        txt += f"""
+        <table>
+            <thead>
+                <tr>
+                    <th>Attribute</th>
+                    <th>Value</th>
+                </tr>
+            </thead>
+            <tbody>
+                <tr><td><b>name</b></td><td>{self.name}</td></tr>
+                <tr><td><b>project</b></td><td>{self.project}</td></tr>
+                <tr><td><b>file_name</b></td><td>{self.file_name}</td></tr>
+                <tr><td><b>db_reader</b></td><td>{self.db_reader}</td></tr>
+        """
+        if self.db_reader == "default":
+            txt += f"<tr><td><b>batch_col</b></td><td>{self.batch_col}</td></tr>"
+        txt += f"""
+                <tr><td><b>time_stamp</b></td><td>{self.time_stamp}</td></tr>
+                <tr><td><b>project_dir</b></td><td>{self.project_dir}</td></tr>
+                <tr><td><b>raw_dir</b></td><td>{self.raw_dir}</td></tr>
+                <tr><td><b>batch_dir</b></td><td>{self.batch_dir}</td></tr>
+            </tbody>
+        </table>
+        """
+        txt += "<h3>Session info</h3>"
+        for key in self.session:
+            txt += f"<p><b>{key}</b>: {self.session[key]}</p>"
+
+        txt += "<h3>Pages</h3>"
+        try:
+            txt += self.pages._repr_html_()  # pylint: disable=protected-access
+        except AttributeError:
+            txt += "<p><b>pages</b><br> not found!</p>"
+        except ValueError:
+            txt += "<p><b>pages</b><br> not readable!</p>"
+        return txt
+
+    def _check_file_name(self, file_name, to_project_folder=False):
+        if file_name is None:
+            if not self.file_name:
+                self.generate_file_name()
+            file_name = pathlib.Path(self.file_name)
+
+        else:
+            file_name = pathlib.Path(file_name)
+        if to_project_folder:
+            file_name = file_name.with_suffix(".json").name
+            project_dir = pathlib.Path(self.project_dir)
+
+            file_name = project_dir / file_name
+        self.file_name = file_name  # updates object (maybe not smart)
+        return file_name
+
+    def from_db(self, project=None, name=None, batch_col=None, **kwargs):
+        """populate journal from db.
+
+        Args:
+            project (str): project name.
+            name (str): experiment name.
+            batch_col (int): batch column.
+
+        **kwargs: sent to engine.
+
+        simple_db-engine -> filefinder.search_for_files:
+            run_name(str): run-file identification.
+            raw_extension(str): optional, extension of run-files (without the '.').
+            cellpy_file_extension(str): optional, extension for cellpy files
+                (without the '.').
+            raw_file_dir(path): optional, directory where to look for run-files
+                (default: read prm-file)
+            cellpy_file_dir(path): optional, directory where to look for
+                cellpy-files (default: read prm-file)
+            prm_filename(path): optional parameter file can be given.
+            file_name_format(str): format of raw-file names or a glob pattern
+                (default: YYYYMMDD_[name]EEE_CC_TT_RR) [not finished yet].
+            reg_exp(str): use regular expression instead (defaults to None) [not finished yet].
+            sub_folders (bool): perform search also in sub-folders.
+            file_list (list of str): perform the search within a given list
+                of filenames instead of searching the folder(s). The list should
+                not contain the full filepath (only the actual file names). If
+                you want to provide the full path, you will have to modify the
+                file_name_format or reg_exp accordingly.
+            pre_path (path or str): path to prepend the list of files selected
+                 from the file_list.
+
+        Returns:
+            None
+        """
+        logging.debug("creating journal from db")
+        if batch_col is None:
+            batch_col = self.batch_col
+        if project is not None:
+            self.project = project
+        if name is None:
+            name = self.name
+        else:
+            self.name = name
+        logging.debug(f"batch_name, batch_col: {name}, {batch_col}")
+
+        if self.db_reader is not None:
+            if isinstance(self.db_reader, dbreader.Reader):  # Simple excel-db
+                id_keys = self.db_reader.select_batch(name, batch_col)
+                logging.debug(f"id_keys: {id_keys}")
+
+                self.pages = self.engine(self.db_reader, id_keys, **kwargs)
+            else:
+                logging.debug(
+                    "creating journal pages using advanced reader methods (not simple excel-db)"
+                )
+                self.pages = self.engine(self.db_reader, batch_name=name, **kwargs)
+
+            if self.pages.empty:
+                logging.critical(
+                    f"EMPTY JOURNAL: are you sure you have provided correct input to batch?"
+                )
+                logging.critical(f"name: {name}")
+                logging.critical(f"project: {self.project}")
+                logging.critical(f"batch_col: {batch_col}")
+        else:
+            logging.debug("creating empty journal pages")
+            self.pages = pd.DataFrame()
+
+        self.generate_empty_session()
+        self.generate_folder_names()
+        self.paginate()
+
+    def generate_empty_session(self):
+        self.session = {}
+        for item in keys_journal_session:
+            self.session[item] = None
+
+    @staticmethod
+    def _fix_cellpy_paths(p):
+        logging.debug("_fix_cellpy_paths does not work with OtherPaths yet")
+        # if platform.system() != "Windows":
+        #     if p.find("\\") >= 0:
+        #         # convert from win to posix
+        #         p = pathlib.PureWindowsPath(p)
+        # else:
+        #     if p.find("/") >= 0:
+        #         # convert from posix to win
+        #         p = pathlib.PurePosixPath(p)
+        # p = pathlib.Path(p)
+        return p
+
+    @classmethod
+    def read_journal_jason_file(cls, file_name, **kwargs):
+        logging.debug(f"json loader starting on {file_name}")
+        with open(file_name, "r") as infile:
+            top_level_dict = json.load(infile)
+        pages_dict = top_level_dict["info_df"]
+        meta = top_level_dict["metadata"]
+        session = top_level_dict.get("session", None)
+        pages = pd.DataFrame(pages_dict)
+        if pages.empty:
+            logging.critical("could not find any pages in the journal")
+            raise UnderDefined
+
+        pages = cls._clean_pages(pages)
+
+        if session is None:
+            logging.debug(f"no session - generating empty one")
+            session = dict()
+
+        session, pages = cls._clean_session(session, pages)
+
+        return pages, meta, session
+
+    @classmethod
+    def read_journal_excel_file(cls, file_name, **kwargs):
+        sheet_names = {"meta": "meta", "pages": "pages", "session": "session"}
+        project = kwargs.pop("project", "NaN")
+        name = kwargs.pop("batch", pathlib.Path(file_name).stem)
+        _meta = {
+            "name": name,
+            "project": project,
+            "project_dir": pathlib.Path("."),
+            "batch_dir": pathlib.Path("."),
+            "raw_dir": pathlib.Path("."),
+        }
+        logging.debug(f"xlsx loader starting on {file_name}")
+
+        meta_sheet_name = sheet_names["meta"]  # not tested yet
+        pages_sheet_name = sheet_names["pages"]
+        session_sheet_name = sheet_names["session"]  # not tested yet
+
+        temporary_directory = tempfile.mkdtemp()
+        temporary_file_name = shutil.copy(file_name, temporary_directory)
+        try:
+            pages = pd.read_excel(
+                temporary_file_name, engine="openpyxl", sheet_name=pages_sheet_name
+            )
+        except KeyError:
+            print(f"Worksheet '{pages_sheet_name}' does not exist.")
+            return None
+
+        try:
+            session = pd.read_excel(
+                temporary_file_name,
+                sheet_name=session_sheet_name,
+                engine="openpyxl",
+                header=[0, 1],
+            )
+        except (KeyError, ValueError):
+            print(f"Worksheet '{session_sheet_name}' does not exist.")
+            session = None
+
+        try:
+            meta = pd.read_excel(
+                temporary_file_name, sheet_name=meta_sheet_name, engine="openpyxl"
+            )
+
+        except (KeyError, ValueError):
+            print(f"Worksheet '{meta_sheet_name}' does not exist.")
+            meta = None
+
+        if pages.empty:
+            logging.critical("could not find any pages in the journal")
+            raise UnderDefined
+        pages = cls._clean_pages(pages)
+        pages = pages.set_index(hdr_journal.filename)
+
+        if meta is None:
+            meta = _meta
+        else:
+            meta = cls._unpack_meta(meta) or _meta
+
+        if session is None:
+            logging.debug(f"no session - generating empty one")
+            session = dict()
+        else:
+            session = cls._unpack_session(session)
+
+        session, pages = cls._clean_session(session, pages)
+
+        return pages, meta, session
+
+    @classmethod
+    def _unpack_session(cls, session):
+        try:
+            bcn2 = {
+                l: list(sb["cycle_index"].values)
+                for l, sb in session["bad_cycles"].groupby("cell_name")
+            }
+        except KeyError:
+            bcn2 = []
+
+        try:
+            bc2 = list(session["bad_cells"]["cell_name"].dropna().values.flatten())
+        except KeyError:
+            bc2 = []
+
+        try:
+            s2 = list(session["starred"]["cell_name"].dropna().values.flatten())
+        except KeyError:
+            s2 = []
+
+        try:
+            n2 = list(session["notes"]["txt"].dropna().values.flatten())
+        except KeyError:
+            n2 = []
+
+        session = {"bad_cycles": bcn2, "bad_cells": bc2, "starred": s2, "notes": n2}
+
+        return session
+
+    @classmethod
+    def _unpack_meta(cls, meta):
+        try:
+            meta = meta.loc[:, ["parameter", "value"]]
+        except KeyError:
+            return
+        meta = meta.set_index("parameter")
+        return meta.to_dict()["value"]
+
+    @classmethod
+    def _clean_session(cls, session, pages):
+        # include steps for cleaning up the session dict here
+        if not session:
+            logging.critical("no session found in your journal file")
+        for item in keys_journal_session:
+            session[item] = session.get(item, None)
+
+        return session, pages
+
+    @classmethod
+    def _clean_pages(cls, pages: pd.DataFrame) -> pd.DataFrame:
+        import ast
+
+        logging.debug("removing empty rows")
+        pages = pages.dropna(how="all")
+        logging.debug("checking path-names")
+        try:
+            p = pages[hdr_journal.raw_file_names]
+            new_p = []
+            for f in p:
+                if isinstance(f, str):
+                    try:
+                        new_f = ast.literal_eval(f"'{f}'")
+                        if isinstance(new_f, list):
+                            f = new_f
+                    except Exception as e:
+                        warnings.warn(e)
+                        warnings.warn(f"Could not evaluate {f}")
+
+                new_p.append(f)
+            pages[hdr_journal.raw_file_names] = new_p
+
+        except KeyError:
+            print(
+                "Tried but failed in converting raw_file_names into an appropriate list"
+            )
+        try:
+            pages[hdr_journal.cellpy_file_name] = pages[
+                hdr_journal.cellpy_file_name
+            ].apply(cls._fix_cellpy_paths)
+        except KeyError:
+            # assumes it is an old type journal file
+            print(f"The key '{hdr_journal.cellpy_file_name}' is missing!")
+            print(f"Assumes that this is an old-type journal file.")
+            try:
+                pages.rename(columns=trans_dict, inplace=True)
+                pages[hdr_journal.cellpy_file_name] = pages[
+                    hdr_journal.cellpy_file_name
+                ].apply(cls._fix_cellpy_paths)
+                logging.warning("old journal file - updating")
+            except KeyError:
+                print("Error! Could still not parse the pages.")
+                print(f"Missing key: {hdr_journal.cellpy_file_name}")
+                pages[hdr_journal.cellpy_file_name] = None
+
+        # only keep selected cells if keep column exists
+        if "keep" in pages.columns:
+            logging.debug("Journal contains 'keep' - selecting only 'keep' > 0.")
+            pages = pages.loc[pages.keep > 0, :]
+
+        for column_name in missing_keys:
+            if column_name not in pages.columns:
+                logging.debug(f"wrong journal format - missing: {column_name}")
+                pages[column_name] = None
+
+        for column_name in hdr_journal:
+            if column_name not in pages.columns:
+                if column_name != hdr_journal.filename:
+                    pages[column_name] = None
+
+        return pages
+
+    def from_file(self, file_name=None, paginate=True, **kwargs):
+        """Loads a DataFrame with all the needed info about the experiment"""
+        file_name = self._check_file_name(file_name)
+        logging.info(f"reading {file_name}")
+        if pathlib.Path(file_name).suffix.lower() == ".xlsx":
+            file_loader = self.read_journal_excel_file
+        else:
+            file_loader = self.read_journal_jason_file
+        try:
+            out = file_loader(file_name, **kwargs)
+            if out is None:
+                raise IOError(f"Error reading {file_name}.")
+            pages, meta_dict, session = out
+        except UnderDefined as e:
+            logging.critical(f"could not load {file_name}")
+            raise UnderDefined from e
+
+        logging.debug(f"got pages and meta_dict")
+
+        self.pages = pages
+        self.session = session
+        self.file_name = file_name
+        self._prm_packer(meta_dict)
+
+        if paginate:
+            self.generate_folder_names()
+            self.paginate()
+
+    def from_frame(self, frame, name=None, project=None, paginate=None, **kwargs):
+        if name is not None:
+            self.name = name
+        if project is not None:
+            self.project = project
+
+        self.pages = (
+            frame  # TODO: include a check here to see if the pages are appropriate
+        )
+        for hdr in hdr_journal.values():
+            if hdr not in self.pages.columns:
+                self.pages[hdr] = None
+
+        if hdr_journal.filename in self.pages.columns:
+            self.pages = self.pages.set_index(hdr_journal.filename)
+
+        if paginate is None:
+            if self.name and self.project:
+                paginate = True
+
+        if paginate:
+            logging.critical(f"paginating {project}/{name} ")
+            self.generate_folder_names()
+            self.paginate()
+
+    def from_file_old(self, file_name=None):
+        """Loads a DataFrame with all the needed info about the experiment"""
+
+        file_name = self._check_file_name(file_name)
+
+        with open(file_name, "r") as infile:
+            top_level_dict = json.load(infile)
+
+        pages_dict = top_level_dict["info_df"]
+        pages = pd.DataFrame(pages_dict)
+        pages[hdr_journal.cellpy_file_name] = pages[hdr_journal.cellpy_file_name].apply(
+            self._fix_cellpy_paths
+        )
+        self.pages = pages
+        self.file_name = file_name
+        self._prm_packer(top_level_dict["metadata"])
+        self.generate_folder_names()
+        self.paginate()
+
+    def create_empty_pages(self, description=None):
+        if description is not None:
+            print(f"Creating from {type(description)} is not implemented yet")
+
+        logging.debug("Creating an empty journal")
+        logging.debug(f"name: {self.name}")
+        logging.debug(f"project: {self.project}")
+
+        col_names = list(hdr_journal.values())
+        pages = pd.DataFrame(columns=col_names)
+        pages.set_index(hdr_journal.filename, inplace=True)
+        return pages
+
+    def duplicate_journal(self, folder=None) -> None:
+        """Copy the journal to folder.
+
+        Args:
+            folder (str or pathlib.Path): folder to copy to (defaults to the
+            current folder).
+        """
+
+        logging.debug(f"duplicating journal to folder {folder}")
+        journal_name = pathlib.Path(self.file_name)
+        if not journal_name.is_file():
+            logging.info("No journal saved")
+            return
+        new_journal_name = journal_name.name
+        if folder is not None:
+            new_journal_name = pathlib.Path(folder) / new_journal_name
+        try:
+            shutil.copy(journal_name, new_journal_name)
+        except shutil.SameFileError:
+            logging.debug("same file exception encountered")
+
+    def to_file(
+        self,
+        file_name=None,
+        paginate=True,
+        to_project_folder=True,
+        duplicate_to_local_folder=True,
+    ):
+        """Saves a DataFrame with all the needed info about the experiment.
+
+        Args:
+            file_name (str or pathlib.Path): journal file name (.json or .xlsx)
+            paginate (bool): make project folders
+            to_project_folder (bool): save journal file to the folder containing your cellpy projects
+            duplicate_to_local_folder (bool): save journal file to the folder you are in now also
+
+        Returns:
+            None
+        """
+        file_name = self._check_file_name(
+            file_name, to_project_folder=to_project_folder
+        )
+
+        pages = self.pages
+        session = self.session
+        meta = self._prm_packer()
+        top_level_dict = {"info_df": pages, "metadata": meta, "session": session}
+
+        is_json = False
+        is_xlsx = False
+
+        if file_name.suffix == ".xlsx":
+            is_xlsx = True
+
+        if file_name.suffix == ".json":
+            is_json = True
+
+        if is_xlsx:
+            df_session = self._pack_session(session)
+            df_meta = self._pack_meta(meta)
+
+            try:
+                pages.index.name = "filename"
+                with pd.ExcelWriter(file_name, mode="w", engine="openpyxl") as writer:
+                    pages.to_excel(writer, sheet_name="pages", engine="openpyxl")
+                    # no index is not supported for multi-index (update to index=False when pandas implement it):
+                    df_session.to_excel(writer, sheet_name="session", engine="openpyxl")
+                    df_meta.to_excel(
+                        writer, sheet_name="meta", engine="openpyxl", index=False
+                    )
+            except PermissionError as e:
+                print(f"Could not load journal to xlsx ({e})")
+
+        if is_json:
+            jason_string = json.dumps(
+                top_level_dict,
+                default=lambda info_df: json.loads(
+                    info_df.to_json(default_handler=str)
+                ),
+            )
+
+            with open(file_name, "w") as outfile:
+                outfile.write(jason_string)
+
+        self.file_name = file_name
+        logging.info(f"Saved file to {file_name}")
+
+        if paginate:
+            self.paginate()
+
+        if duplicate_to_local_folder:
+            self.duplicate_journal()
+
+    @staticmethod
+    def _pack_session(session):
+        frames = []
+        keys = []
+        try:
+            l_bad_cycle_numbers = []
+
+            for k, v in session["bad_cycles"].items():
+                l_bad_cycle_numbers.append(pd.DataFrame(data=v, columns=[k]))
+
+            df_bad_cycle_numbers = (
+                pd.concat(l_bad_cycle_numbers, axis=1)
+                .melt(var_name="cell_name", value_name="cycle_index")
+                .dropna()
+            )
+            frames.append(df_bad_cycle_numbers)
+            keys.append("bad_cycles")
+        except (KeyError, AttributeError):
+            logging.debug("missing bad cycle numbers")
+
+        df_bad_cells = pd.DataFrame(session["bad_cells"], columns=["cell_name"])
+        frames.append(df_bad_cells)
+        keys.append("bad_cells")
+
+        df_starred = pd.DataFrame(session["starred"], columns=["cell_name"])
+        frames.append(df_starred)
+        keys.append("starred")
+
+        df_notes = pd.DataFrame(session["notes"], columns=["txt"])
+        frames.append(df_notes)
+        keys.append("notes")
+
+        session = pd.concat(frames, axis=1, keys=keys)
+        return session
+
+    @staticmethod
+    def _pack_meta(meta):
+        meta = pd.DataFrame(meta, index=[0]).melt(
+            var_name="parameter", value_name="value"
+        )
+        return meta
+
+    def generate_folder_names(self):
+        """Set appropriate folder names."""
+        logging.debug("creating folder names")
+        if self.project and isinstance(self.project, (pathlib.Path, str)):
+            logging.debug("got project name")
+            logging.debug(self.project)
+            self.project_dir = os.path.join(prms.Paths.outdatadir, self.project)
+        else:
+            logging.critical(
+                "Could not create project dir (missing project definition)"
+            )
+        if self.name:
+            self.batch_dir = os.path.join(self.project_dir, self.name)
+            self.raw_dir = os.path.join(self.batch_dir, "raw_data")
+        else:
+            logging.critical(
+                "Could not create batch_dir and raw_dir", "(missing batch name)"
+            )
+        logging.debug(f"batch dir: {self.batch_dir}")
+        logging.debug(f"project dir: {self.project_dir}")
+        logging.debug(f"raw dir: {self.raw_dir}")
+
+    def paginate(self):
+        """Make folders where we would like to put results etc."""
+
+        project_dir = self.project_dir
+        raw_dir = self.raw_dir
+        batch_dir = self.batch_dir
+
+        if project_dir is None:
+            raise UnderDefined("no project directory defined")
+        if raw_dir is None:
+            raise UnderDefined("no raw directory defined")
+        if batch_dir is None:
+            raise UnderDefined("no batch directory defined")
+
+        # create the folders
+        if not os.path.isdir(project_dir):
+            os.mkdir(project_dir)
+            logging.info(f"created folder {project_dir}")
+        if not os.path.isdir(batch_dir):
+            os.mkdir(batch_dir)
+            logging.info(f"created folder {batch_dir}")
+        if not os.path.isdir(raw_dir):
+            os.mkdir(raw_dir)
+            logging.info(f"created folder {raw_dir}")
+
+        self.project_dir = project_dir
+        self.batch_dir = batch_dir
+        self.raw_dir = raw_dir
+
+        return project_dir, batch_dir, raw_dir
+
+    def generate_file_name(self):
+        """generate a suitable file name for the experiment"""
+        if not self.project:
+            raise UnderDefined("project name not given")
+        out_data_dir = prms.Paths.outdatadir
+        project_dir = os.path.join(out_data_dir, self.project)
+        file_name = f"cellpy_batch_{self.name}.json"
+        self.file_name = os.path.join(project_dir, file_name)
+
+    # v.1.0.0:
+    def look_for_file(self):
+        pass
+
+    def get_column(self, header):
+        """populate new column from db"""
+        pass
+
+    def get_cell(self, id_key):
+        """get additional cell info from db"""
+        pass
+
+    def add_comment(self, comment):
+        """add a comment (will be saved in the journal file)"""
+        pass
+
+    def remove_comment(self, comment_id):
+        pass
+
+    def view_comments(self):
+        pass
+
+    def remove_cell(self, cell_id):
+        pass
+
+    def add_cell(self, cell_id, **kwargs):
+        """Add a cell to the pages"""
+        pass
+
+
+def _dev_journal_loading():
+    from cellpy import log
+
+    log.setup_logging(default_level="DEBUG")
+    journal_file = pathlib.Path(
+        "../../../testdata/batch_project/test_project.json"
+    ).resolve()
+    assert journal_file.is_file()
+
+    logging.debug(f"reading journal file {journal_file}")
+    journal = LabJournal(db_reader=None)
+    journal.from_file(journal_file, paginate=False)
+    print(80 * "-")
+    print(journal.pages)
+    print(80 * "-")
+    print(journal.session)
+
+    # creating a mock session
+    bad_cycle_numbers = {
+        "20160805_test001_45_cc": [4, 337, 338],
+        "20160805_test001_47_cc": [7, 8, 9],
+    }
+    bad_cells = ["20160805_test001_45_cc"]
+
+    notes = {"date_stamp": "one comment for the road", "date_stamp2": "another comment"}
+    session = {
+        "bad_cycle_numbers": bad_cycle_numbers,
+        "bad_cells": bad_cells,
+        "notes": notes,
+    }
+
+    # journal.session = session
+
+    new_journal_name = journal_file.with_name(f"{journal_file.stem}_tmp.xlsx")
+    print(new_journal_name)
+    journal.to_file(file_name=new_journal_name, paginate=False, to_project_folder=False)
+
+
+if __name__ == "__main__":
+    print(" running journal ".center(80, "-"))
+    _dev_journal_loading()
+    print(" finished ".center(80, "-"))
```

### Comparing `cellpy-1.0.0a0/cellpy/utils/batch_tools/batch_plotters.py` & `cellpy-1.0.0a3/cellpy/utils/batch_tools/batch_plotters.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/cellpy/utils/batch_tools/dumpers.py` & `cellpy-1.0.0a3/cellpy/utils/batch_tools/dumpers.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/cellpy/utils/batch_tools/engines.py` & `cellpy-1.0.0a3/cellpy/utils/batch_tools/engines.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,283 +1,284 @@
-"""Engines are functions that are used by the Do-ers.
-
-    Keyword Args: experiments, farms, barn, optionals
-    Returns: farms, barn
-"""
-
-import logging
-import time
-import warnings
-
-import pandas as pd
-
-from cellpy import dbreader
-from cellpy.parameters.internal_settings import get_headers_journal, get_headers_summary
-from cellpy.utils.batch_tools import batch_helpers as helper
-
-hdr_journal = get_headers_journal()
-hdr_summary = get_headers_summary()
-
-SELECTED_SUMMARIES = [
-    hdr_summary["discharge_capacity_gravimetric"],
-    hdr_summary["charge_capacity_gravimetric"],
-    hdr_summary["coulombic_efficiency"],
-    hdr_summary["cumulated_coulombic_efficiency"],
-    hdr_summary["ir_discharge"],
-    hdr_summary["ir_charge"],
-    hdr_summary["end_voltage_discharge"],
-    hdr_summary["end_voltage_charge"],
-    hdr_summary["charge_c_rate"],
-    hdr_summary["discharge_c_rate"],
-]
-
-
-def cycles_engine(**kwargs):
-    """engine to extract cycles"""
-    logging.debug("cycles_engine::Not finished yet (sorry).")
-    warnings.warn(
-        "This utility function will be seriously changed soon and possibly removed",
-        category=DeprecationWarning,
-    )
-    # raise NotImplementedError
-
-    experiments = kwargs["experiments"]
-
-    farms = []
-    barn = "raw_dir"  # Its a murder in the red barn - murder in the red barn
-
-    for experiment in experiments:
-        farms.append([])
-        if experiment.all_in_memory:
-            logging.debug("all in memory")
-            for key in experiment.cell_data_frames:
-                logging.debug(f"extracting cycles from {key}")
-                # extract cycles here and send it to the farm
-        else:
-            logging.debug("dont have it in memory - need to lookup in the files")
-            for key in experiment.cell_data_frames:
-                logging.debug(f"looking up cellpyfile for {key}")
-                # extract cycles here and send it to the farm
-
-    return farms, barn
-
-
-def raw_data_engine(**kwargs):
-    """engine to extract raw data"""
-    warnings.warn(
-        "This utility function will be seriously changed soon and possibly removed",
-        category=DeprecationWarning,
-    )
-    logging.debug("cycles_engine")
-    farms = None
-    barn = "raw_dir"
-    raise NotImplementedError
-
-
-def summary_engine(**kwargs):
-    """engine to extract summary data"""
-    logging.debug("summary_engine")
-    # farms = kwargs["farms"]
-
-    farms = []
-    experiments = kwargs.pop("experiments")
-    reset = kwargs.pop("reset", False)
-
-    for experiment in experiments:
-        if experiment.selected_summaries is None:
-            selected_summaries = SELECTED_SUMMARIES
-        else:
-            selected_summaries = experiment.selected_summaries
-
-        if reset or experiment.summary_frames is None:
-            logging.debug("No summary frames found")
-            logging.debug("Re-loading")
-            experiment.summary_frames = _load_summaries(experiment)
-
-        farm = helper.join_summaries(experiment.summary_frames, selected_summaries)
-        farms.append(farm)
-    barn = "batch_dir"
-
-    return farms, barn
-
-
-def _load_summaries(experiment):
-    summary_frames = {}
-    for label in experiment.cell_names:
-        # TODO: replace this with direct lookup from hdf5?
-        summary_frames[label] = experiment.data[label].data.summary
-    return summary_frames
-
-
-def dq_dv_engine(**kwargs):
-    """engine that performs incremental analysis of the cycle-data"""
-    warnings.warn(
-        "This utility function will be seriously changed soon and possibly removed",
-        category=DeprecationWarning,
-    )
-    farms = None
-    barn = "raw_dir"
-    raise NotImplementedError
-
-
-def _query(reader_method, cell_ids, column_name=None):
-    if not any(cell_ids):
-        logging.debug("Received empty cell_ids")
-        return []
-
-    try:
-        if column_name is None:
-            result = [reader_method(cell_id) for cell_id in cell_ids]
-        else:
-            result = [reader_method(column_name, cell_id) for cell_id in cell_ids]
-    except Exception as e:
-        logging.debug(f"Error in querying db.")
-        logging.debug(e)
-        result = [None for _ in range(len(cell_ids))]
-    return result
-
-
-def sql_db_engine(*args, **kwargs) -> pd.DataFrame:
-    print("sql_db_engine")
-    print(f"args: {args}")
-    print(f"kwargs: {kwargs}")
-    return pd.DataFrame()
-
-
-# TODO-246: load area
-def simple_db_engine(
-    reader=None,
-    cell_ids=None,
-    file_list=None,
-    pre_path=None,
-    include_key=False,
-    include_individual_arguments=True,
-    additional_column_names=None,
-    batch_name=None,
-    **kwargs,
-):
-    """Engine that gets values from the db for given set of cell IDs.
-
-    The simple_db_engine looks up values for mass, names, etc. from
-    the db using the reader object. In addition, it searches for the
-    corresponding raw files / data.
-
-    Args:
-        reader: a reader object (defaults to dbreader.Reader)
-        cell_ids: keys (cell IDs) (assumes that the db has already been filtered, if not, use batch_name).
-        file_list: file list to send to filefinder (instead of searching in folders for files).
-        pre_path: prepended path to send to filefinder.
-        include_key: include the key col in the pages (the cell IDs).
-        include_individual_arguments: include the argument column in the pages.
-        additional_column_names: list of additional column names to include in the pages.
-        batch_name: name of the batch (used if cell_ids are not given)
-        **kwargs: sent to filefinder
-
-    Returns:
-        pages (pandas.DataFrame)
-    """
-
-    new_version = False
-
-    # This is not really a proper Do-er engine. But not sure where to put it.
-    if reader is None:
-        reader = dbreader.Reader()
-        logging.debug("No reader provided. Creating one myself.")
-
-    if cell_ids is None:
-        pages_dict = reader.from_batch(
-            batch_name=batch_name,
-            include_key=include_key,
-            include_individual_arguments=include_individual_arguments,
-        )
-
-    else:
-        pages_dict = dict()
-        pages_dict[hdr_journal["filename"]] = _query(reader.get_cell_name, cell_ids)
-        if include_key:
-            pages_dict[hdr_journal["id_key"]] = cell_ids
-
-        if include_individual_arguments:
-            pages_dict[hdr_journal["argument"]] = _query(reader.get_args, cell_ids)
-
-        pages_dict[hdr_journal["mass"]] = _query(reader.get_mass, cell_ids)
-        pages_dict[hdr_journal["total_mass"]] = _query(reader.get_total_mass, cell_ids)
-        pages_dict[hdr_journal["loading"]] = _query(reader.get_loading, cell_ids)
-        pages_dict[hdr_journal["nom_cap"]] = _query(reader.get_nom_cap, cell_ids)
-        pages_dict[hdr_journal["area"]] = _query(reader.get_area, cell_ids)
-        pages_dict[hdr_journal["experiment"]] = _query(
-            reader.get_experiment_type, cell_ids
-        )
-        pages_dict[hdr_journal["fixed"]] = _query(reader.inspect_hd5f_fixed, cell_ids)
-        pages_dict[hdr_journal["label"]] = _query(reader.get_label, cell_ids)
-        pages_dict[hdr_journal["cell_type"]] = _query(reader.get_cell_type, cell_ids)
-        pages_dict[hdr_journal["instrument"]] = _query(reader.get_instrument, cell_ids)
-        pages_dict[hdr_journal["raw_file_names"]] = []
-        pages_dict[hdr_journal["cellpy_file_name"]] = []
-        pages_dict[hdr_journal["comment"]] = _query(reader.get_comment, cell_ids)
-        pages_dict[hdr_journal["group"]] = _query(reader.get_group, cell_ids)
-
-        if additional_column_names is not None:
-            for k in additional_column_names:
-                try:
-                    pages_dict[k] = _query(reader.get_by_column_label, cell_ids, k)
-                except Exception as e:
-                    logging.info(f"Could not retrieve from column {k} ({e})")
-
-        logging.debug(f"created info-dict from {reader.db_file}:")
-
-    for key in list(pages_dict.keys()):
-        logging.debug("%s: %s" % (key, str(pages_dict[key])))
-
-    _groups = pages_dict[hdr_journal["group"]]
-    groups = helper.fix_groups(_groups)
-    pages_dict[hdr_journal["group"]] = groups
-
-    my_timer_start = time.time()
-    pages_dict = helper.find_files(
-        pages_dict, file_list=file_list, pre_path=pre_path, **kwargs
-    )
-    my_timer_end = time.time()
-    if (my_timer_end - my_timer_start) > 5.0:
-        logging.critical(
-            "The function _find_files was very slow. "
-            "Save your journal so you don't have to run it again! "
-            "You can load it again using the from_journal(journal_name) method."
-        )
-
-    pages = pd.DataFrame(pages_dict)
-    try:
-        pages = pages.sort_values([hdr_journal.group, hdr_journal.filename])
-    except TypeError as e:
-        _report_suspected_duplicate_id(
-            e,
-            "sort the values",
-            pages[[hdr_journal.group, hdr_journal.filename]],
-        )
-
-    pages = helper.make_unique_groups(pages)
-
-    try:
-        pages[hdr_journal.label] = pages[hdr_journal.filename].apply(
-            helper.create_labels
-        )
-    except AttributeError as e:
-        _report_suspected_duplicate_id(
-            e, "make labels", pages[[hdr_journal.label, hdr_journal.filename]]
-        )
-
-    else:
-        # TODO: check if drop=False works [#index]
-        pages.set_index(hdr_journal["filename"], inplace=True)  # edit this to allow for
-        # non-numeric index-names (for tab completion and python-box)
-    return pages
-
-
-def _report_suspected_duplicate_id(e, what="do it", on=None):
-    logging.warning(f"could not {what}")
-    logging.warning(f"{on}")
-    logging.warning("maybe you have a corrupted db?")
-    logging.warning(
-        "typically happens if the cell_id is not unique (several rows or records in "
-        "your db has the same cell_id or key)"
-    )
-    logging.warning(e)
+"""Engines are functions that are used by the Do-ers.
+
+    Keyword Args: experiments, farms, barn, optionals
+    Returns: farms, barn
+"""
+
+import logging
+import time
+import warnings
+
+import pandas as pd
+
+from cellpy import dbreader
+from cellpy.parameters.internal_settings import get_headers_journal, get_headers_summary
+from cellpy.utils.batch_tools import batch_helpers as helper
+
+hdr_journal = get_headers_journal()
+hdr_summary = get_headers_summary()
+
+SELECTED_SUMMARIES = [
+    hdr_summary["discharge_capacity_gravimetric"],
+    hdr_summary["charge_capacity_gravimetric"],
+    hdr_summary["coulombic_efficiency"],
+    hdr_summary["cumulated_coulombic_efficiency"],
+    hdr_summary["ir_discharge"],
+    hdr_summary["ir_charge"],
+    hdr_summary["end_voltage_discharge"],
+    hdr_summary["end_voltage_charge"],
+    hdr_summary["charge_c_rate"],
+    hdr_summary["discharge_c_rate"],
+]
+
+
+def cycles_engine(**kwargs):
+    """engine to extract cycles"""
+    logging.debug("cycles_engine::Not finished yet (sorry).")
+    warnings.warn(
+        "This utility function will be seriously changed soon and possibly removed",
+        category=DeprecationWarning,
+    )
+    # raise NotImplementedError
+
+    experiments = kwargs["experiments"]
+
+    farms = []
+    barn = "raw_dir"  # Its a murder in the red barn - murder in the red barn
+
+    for experiment in experiments:
+        farms.append([])
+        if experiment.all_in_memory:
+            logging.debug("all in memory")
+            for key in experiment.cell_data_frames:
+                logging.debug(f"extracting cycles from {key}")
+                # extract cycles here and send it to the farm
+        else:
+            logging.debug("dont have it in memory - need to lookup in the files")
+            for key in experiment.cell_data_frames:
+                logging.debug(f"looking up cellpyfile for {key}")
+                # extract cycles here and send it to the farm
+
+    return farms, barn
+
+
+def raw_data_engine(**kwargs):
+    """engine to extract raw data"""
+    warnings.warn(
+        "This utility function will be seriously changed soon and possibly removed",
+        category=DeprecationWarning,
+    )
+    logging.debug("cycles_engine")
+    farms = None
+    barn = "raw_dir"
+    raise NotImplementedError
+
+
+def summary_engine(**kwargs):
+    """engine to extract summary data"""
+    logging.debug("summary_engine")
+    # farms = kwargs["farms"]
+
+    farms = []
+    experiments = kwargs.pop("experiments")
+    reset = kwargs.pop("reset", False)
+
+    for experiment in experiments:
+        if experiment.selected_summaries is None:
+            selected_summaries = SELECTED_SUMMARIES
+        else:
+            selected_summaries = experiment.selected_summaries
+
+        if reset or experiment.summary_frames is None:
+            logging.debug("No summary frames found")
+            logging.debug("Re-loading")
+            experiment.summary_frames = _load_summaries(experiment)
+
+        farm = helper.join_summaries(experiment.summary_frames, selected_summaries)
+        farms.append(farm)
+    barn = "batch_dir"
+
+    return farms, barn
+
+
+def _load_summaries(experiment):
+    summary_frames = {}
+    for label in experiment.cell_names:
+        # TODO: replace this with direct lookup from hdf5?
+        summary_frames[label] = experiment.data[label].data.summary
+    return summary_frames
+
+
+def dq_dv_engine(**kwargs):
+    """engine that performs incremental analysis of the cycle-data"""
+    warnings.warn(
+        "This utility function will be seriously changed soon and possibly removed",
+        category=DeprecationWarning,
+    )
+    farms = None
+    barn = "raw_dir"
+    raise NotImplementedError
+
+
+def _query(reader_method, cell_ids, column_name=None):
+    if not any(cell_ids):
+        logging.debug("Received empty cell_ids")
+        return []
+
+    try:
+        if column_name is None:
+            result = [reader_method(cell_id) for cell_id in cell_ids]
+        else:
+            result = [reader_method(column_name, cell_id) for cell_id in cell_ids]
+    except Exception as e:
+        logging.debug(f"Error in querying db.")
+        logging.debug(e)
+        result = [None for _ in range(len(cell_ids))]
+    return result
+
+
+def sql_db_engine(*args, **kwargs) -> pd.DataFrame:
+    print("sql_db_engine")
+    print(f"args: {args}")
+    print(f"kwargs: {kwargs}")
+    return pd.DataFrame()
+
+
+# TODO-246: load area
+def simple_db_engine(
+    reader=None,
+    cell_ids=None,
+    file_list=None,
+    pre_path=None,
+    include_key=False,
+    include_individual_arguments=True,
+    additional_column_names=None,
+    batch_name=None,
+    **kwargs,
+):
+    """Engine that gets values from the db for given set of cell IDs.
+
+    The simple_db_engine looks up values for mass, names, etc. from
+    the db using the reader object. In addition, it searches for the
+    corresponding raw files / data.
+
+    Args:
+        reader: a reader object (defaults to dbreader.Reader)
+        cell_ids: keys (cell IDs) (assumes that the db has already been filtered, if not, use batch_name).
+        file_list: file list to send to filefinder (instead of searching in folders for files).
+        pre_path: prepended path to send to filefinder.
+        include_key: include the key col in the pages (the cell IDs).
+        include_individual_arguments: include the argument column in the pages.
+        additional_column_names: list of additional column names to include in the pages.
+        batch_name: name of the batch (used if cell_ids are not given)
+        **kwargs: sent to filefinder
+
+    Returns:
+        pages (pandas.DataFrame)
+    """
+
+    new_version = False
+
+    # This is not really a proper Do-er engine. But not sure where to put it.
+    logging.debug("simple_db_engine")
+    if reader is None:
+        reader = dbreader.Reader()
+        logging.debug("No reader provided. Creating one myself.")
+
+    if cell_ids is None:
+        pages_dict = reader.from_batch(
+            batch_name=batch_name,
+            include_key=include_key,
+            include_individual_arguments=include_individual_arguments,
+        )
+
+    else:
+        pages_dict = dict()
+        pages_dict[hdr_journal["filename"]] = _query(reader.get_cell_name, cell_ids)
+        if include_key:
+            pages_dict[hdr_journal["id_key"]] = cell_ids
+
+        if include_individual_arguments:
+            pages_dict[hdr_journal["argument"]] = _query(reader.get_args, cell_ids)
+
+        pages_dict[hdr_journal["mass"]] = _query(reader.get_mass, cell_ids)
+        pages_dict[hdr_journal["total_mass"]] = _query(reader.get_total_mass, cell_ids)
+        pages_dict[hdr_journal["loading"]] = _query(reader.get_loading, cell_ids)
+        pages_dict[hdr_journal["nom_cap"]] = _query(reader.get_nom_cap, cell_ids)
+        pages_dict[hdr_journal["area"]] = _query(reader.get_area, cell_ids)
+        pages_dict[hdr_journal["experiment"]] = _query(
+            reader.get_experiment_type, cell_ids
+        )
+        pages_dict[hdr_journal["fixed"]] = _query(reader.inspect_hd5f_fixed, cell_ids)
+        pages_dict[hdr_journal["label"]] = _query(reader.get_label, cell_ids)
+        pages_dict[hdr_journal["cell_type"]] = _query(reader.get_cell_type, cell_ids)
+        pages_dict[hdr_journal["instrument"]] = _query(reader.get_instrument, cell_ids)
+        pages_dict[hdr_journal["raw_file_names"]] = []
+        pages_dict[hdr_journal["cellpy_file_name"]] = []
+        pages_dict[hdr_journal["comment"]] = _query(reader.get_comment, cell_ids)
+        pages_dict[hdr_journal["group"]] = _query(reader.get_group, cell_ids)
+
+        if additional_column_names is not None:
+            for k in additional_column_names:
+                try:
+                    pages_dict[k] = _query(reader.get_by_column_label, cell_ids, k)
+                except Exception as e:
+                    logging.info(f"Could not retrieve from column {k} ({e})")
+
+        logging.debug(f"created info-dict from {reader.db_file}:")
+
+    for key in list(pages_dict.keys()):
+        logging.debug("%s: %s" % (key, str(pages_dict[key])))
+
+    _groups = pages_dict[hdr_journal["group"]]
+    groups = helper.fix_groups(_groups)
+    pages_dict[hdr_journal["group"]] = groups
+
+    my_timer_start = time.time()
+    pages_dict = helper.find_files(
+        pages_dict, file_list=file_list, pre_path=pre_path, **kwargs
+    )
+    my_timer_end = time.time()
+    if (my_timer_end - my_timer_start) > 5.0:
+        logging.critical(
+            "The function _find_files was very slow. "
+            "Save your journal so you don't have to run it again! "
+            "You can load it again using the from_journal(journal_name) method."
+        )
+
+    pages = pd.DataFrame(pages_dict)
+    try:
+        pages = pages.sort_values([hdr_journal.group, hdr_journal.filename])
+    except TypeError as e:
+        _report_suspected_duplicate_id(
+            e,
+            "sort the values",
+            pages[[hdr_journal.group, hdr_journal.filename]],
+        )
+
+    pages = helper.make_unique_groups(pages)
+
+    try:
+        pages[hdr_journal.label] = pages[hdr_journal.filename].apply(
+            helper.create_labels
+        )
+    except AttributeError as e:
+        _report_suspected_duplicate_id(
+            e, "make labels", pages[[hdr_journal.label, hdr_journal.filename]]
+        )
+
+    else:
+        # TODO: check if drop=False works [#index]
+        pages.set_index(hdr_journal["filename"], inplace=True)  # edit this to allow for
+        # non-numeric index-names (for tab completion and python-box)
+    return pages
+
+
+def _report_suspected_duplicate_id(e, what="do it", on=None):
+    logging.warning(f"could not {what}")
+    logging.warning(f"{on}")
+    logging.warning("maybe you have a corrupted db?")
+    logging.warning(
+        "typically happens if the cell_id is not unique (several rows or records in "
+        "your db has the same cell_id or key)"
+    )
+    logging.warning(e)
```

### Comparing `cellpy-1.0.0a0/cellpy/utils/batch_tools/sqlite_from_excel_db.py` & `cellpy-1.0.0a3/cellpy/utils/batch_tools/sqlite_from_excel_db.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/cellpy/utils/collectors.py` & `cellpy-1.0.0a3/cellpy/utils/collectors.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/cellpy/utils/collectors_old.py` & `cellpy-1.0.0a3/cellpy/utils/collectors_old.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/cellpy/utils/data/20160805_test001_45_cc.h5` & `cellpy-1.0.0a3/cellpy/utils/data/20160805_test001_45_cc.h5`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/cellpy/utils/data/raw/20160805_test001_45_cc_01.res` & `cellpy-1.0.0a3/cellpy/utils/data/raw/20160805_test001_45_cc_01.res`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/cellpy/utils/easyplot.py` & `cellpy-1.0.0a3/cellpy/utils/easyplot.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/cellpy/utils/example_data.py` & `cellpy-1.0.0a3/cellpy/utils/example_data.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/cellpy/utils/helpers.py` & `cellpy-1.0.0a3/cellpy/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/cellpy/utils/ica.py` & `cellpy-1.0.0a3/cellpy/utils/ica.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/cellpy/utils/ocv_rlx.py` & `cellpy-1.0.0a3/cellpy/utils/ocv_rlx.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/cellpy/utils/plotutils.py` & `cellpy-1.0.0a3/cellpy/utils/plotutils.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/cellpy/utils/processor.py` & `cellpy-1.0.0a3/cellpy/utils/processor.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/cellpy.egg-info/PKG-INFO` & `cellpy-1.0.0a3/cellpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellpy
-Version: 1.0.0a0
+Version: 1.0.0a3
 Summary: Extract and manipulate data from battery data testers.
 Home-page: https://github.com/jepegit/cellpy
 Author: Jan Petter Maehlen
 Author-email: jepe@ife.no
 License: MIT license
 Keywords: cellpy
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cellpy-1.0.0a0/cellpy.egg-info/SOURCES.txt` & `cellpy-1.0.0a3/cellpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/Makefile` & `cellpy-1.0.0a3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_6_0.png` & `cellpy-1.0.0a3/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_6_0.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_7_0.png` & `cellpy-1.0.0a3/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_7_0.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_8_0.png` & `cellpy-1.0.0a3/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_8_0.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_simple_plot_2_0.png` & `cellpy-1.0.0a3/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_simple_plot_2_0.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_6_0.png` & `cellpy-1.0.0a3/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_6_0.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_7_0.png` & `cellpy-1.0.0a3/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_7_0.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_8_0.png` & `cellpy-1.0.0a3/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_8_0.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_simple_plot_2_0.png` & `cellpy-1.0.0a3/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_simple_plot_2_0.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/_build/_images/graphviz-22185705e237fa530df24e4af50cb25833165e25.png` & `cellpy-1.0.0a3/docs/_build/_images/graphviz-22185705e237fa530df24e4af50cb25833165e25.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/_build/_images/graphviz-246f2486cd940f2ea40a07f847c86c22b2607ca8.png` & `cellpy-1.0.0a3/docs/_build/_images/graphviz-246f2486cd940f2ea40a07f847c86c22b2607ca8.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/_build/_images/graphviz-42e9bc826d476a3d361a7f410e989ed34dc1aa85.png` & `cellpy-1.0.0a3/docs/_build/_images/graphviz-42e9bc826d476a3d361a7f410e989ed34dc1aa85.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/_build/_images/graphviz-619216a42370fd49669c083549129b8470c8fae1.png` & `cellpy-1.0.0a3/docs/_build/_images/graphviz-619216a42370fd49669c083549129b8470c8fae1.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/_build/_images/graphviz-6412a7c74952b4793798e9032f5bc4e7a1ab70c1.png` & `cellpy-1.0.0a3/docs/_build/_images/graphviz-6412a7c74952b4793798e9032f5bc4e7a1ab70c1.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/_build/_images/graphviz-6deb64a460668e8ef9bf0ca653314119adeeae66.png` & `cellpy-1.0.0a3/docs/_build/_images/graphviz-6deb64a460668e8ef9bf0ca653314119adeeae66.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/_build/_images/graphviz-83b62e03ef369ff0a30f027892dba95b91ea8b6c.png` & `cellpy-1.0.0a3/docs/_build/_images/graphviz-83b62e03ef369ff0a30f027892dba95b91ea8b6c.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/_build/_images/graphviz-8ec82d564b1a6ea5b95a36a4a213f7a78aaedc63.png` & `cellpy-1.0.0a3/docs/_build/_images/graphviz-8ec82d564b1a6ea5b95a36a4a213f7a78aaedc63.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/_build/_images/graphviz-ce8a9fe2ba01194aed847e0248d749db4093aca1.png` & `cellpy-1.0.0a3/docs/_build/_images/graphviz-ce8a9fe2ba01194aed847e0248d749db4093aca1.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/_build/_images/graphviz-e94a5352318e02fcc5ef1f813e02a526c39af791.png` & `cellpy-1.0.0a3/docs/_build/_images/graphviz-e94a5352318e02fcc5ef1f813e02a526c39af791.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/_build/_images/templates_jupyterlab_001.png` & `cellpy-1.0.0a3/docs/_build/_images/templates_jupyterlab_001.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/_build/_images/tutorials_utils_plotting_fig1.png` & `cellpy-1.0.0a3/docs/_build/_images/tutorials_utils_plotting_fig1.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/_build/_images/tutorials_utils_plotting_fig2.png` & `cellpy-1.0.0a3/docs/_build/_images/tutorials_utils_plotting_fig2.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/adapted_readme.rst` & `cellpy-1.0.0a3/docs/adapted_readme.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/conf.py` & `cellpy-1.0.0a3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/developers_guide/dev_cellpy_data_structure.rst` & `cellpy-1.0.0a3/docs/developers_guide/dev_cellpy_data_structure.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/developers_guide/dev_cellpy_folder_structure.rst` & `cellpy-1.0.0a3/docs/developers_guide/dev_cellpy_folder_structure.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/developers_guide/dev_cellpy_packaging_pypi.rst` & `cellpy-1.0.0a3/docs/developers_guide/dev_cellpy_packaging_pypi.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/developers_guide/dev_cellpy_setup.rst` & `cellpy-1.0.0a3/docs/developers_guide/dev_cellpy_setup.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/developers_guide/dev_conda_package.rst` & `cellpy-1.0.0a3/docs/developers_guide/dev_conda_package.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/developers_guide/dev_docs.rst` & `cellpy-1.0.0a3/docs/developers_guide/dev_docs.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/developers_guide/dev_loaders_and_instruments.rst` & `cellpy-1.0.0a3/docs/developers_guide/dev_loaders_and_instruments.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/developers_guide/dev_various.rst` & `cellpy-1.0.0a3/docs/developers_guide/dev_various.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/examples_and_tutorials/basic_interactions/01_getting_started_tutorial.rst` & `cellpy-1.0.0a3/docs/examples_and_tutorials/basic_interactions/01_getting_started_tutorial.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/examples_and_tutorials/basic_interactions/02_read_cell_data.rst` & `cellpy-1.0.0a3/docs/examples_and_tutorials/basic_interactions/02_read_cell_data.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/examples_and_tutorials/basic_interactions/03_more_about_get.rst` & `cellpy-1.0.0a3/docs/examples_and_tutorials/basic_interactions/03_more_about_get.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/examples_and_tutorials/basic_interactions/04_other_interactions.rst` & `cellpy-1.0.0a3/docs/examples_and_tutorials/basic_interactions/04_other_interactions.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/examples_and_tutorials/basic_interactions/05_configuring.rst` & `cellpy-1.0.0a3/docs/examples_and_tutorials/basic_interactions/05_configuring.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/examples_and_tutorials/basic_interactions/06_pandas.rst` & `cellpy-1.0.0a3/docs/examples_and_tutorials/basic_interactions/06_pandas.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/examples_and_tutorials/basic_interactions/07_data_mining.rst` & `cellpy-1.0.0a3/docs/examples_and_tutorials/basic_interactions/07_data_mining.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/examples_and_tutorials/basic_interactions/08_the_cellpy_cmd.rst` & `cellpy-1.0.0a3/docs/examples_and_tutorials/basic_interactions/08_the_cellpy_cmd.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/examples_and_tutorials/notebooks/images/templates_jupyterlab_001.png` & `cellpy-1.0.0a3/docs/examples_and_tutorials/notebooks/images/templates_jupyterlab_001.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/examples_and_tutorials/notebooks/images/templates_jupyterlab_002.png` & `cellpy-1.0.0a3/docs/examples_and_tutorials/notebooks/images/templates_jupyterlab_002.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/examples_and_tutorials/tips_and_tricks.rst` & `cellpy-1.0.0a3/docs/examples_and_tutorials/tips_and_tricks.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/examples_and_tutorials/utils/batch.rst` & `cellpy-1.0.0a3/docs/examples_and_tutorials/utils/batch.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/examples_and_tutorials/utils/figures/tutorials_utils_plotting_fig1.png` & `cellpy-1.0.0a3/docs/examples_and_tutorials/utils/figures/tutorials_utils_plotting_fig1.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/examples_and_tutorials/utils/figures/tutorials_utils_plotting_fig2.png` & `cellpy-1.0.0a3/docs/examples_and_tutorials/utils/figures/tutorials_utils_plotting_fig2.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/examples_and_tutorials/utils/ica.rst` & `cellpy-1.0.0a3/docs/examples_and_tutorials/utils/ica.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/examples_and_tutorials/utils/plotting.rst` & `cellpy-1.0.0a3/docs/examples_and_tutorials/utils/plotting.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/examples_and_tutorials/utils/tut_ocv_rlx.rst` & `cellpy-1.0.0a3/docs/examples_and_tutorials/utils/tut_ocv_rlx.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/figures/cellpy-icon-bw.png` & `cellpy-1.0.0a3/docs/figures/cellpy-icon-bw.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/figures/cellpy-logo-v1.png` & `cellpy-1.0.0a3/docs/figures/cellpy-logo-v1.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/index.rst` & `cellpy-1.0.0a3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/main_description/formats.rst` & `cellpy-1.0.0a3/docs/main_description/formats.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/main_description/installation.rst` & `cellpy-1.0.0a3/docs/main_description/installation.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/main_description/usage.rst` & `cellpy-1.0.0a3/docs/main_description/usage.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/make.bat` & `cellpy-1.0.0a3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/source/cellpy.parameters.rst` & `cellpy-1.0.0a3/docs/source/cellpy.parameters.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/source/cellpy.readers.instruments.configurations.rst` & `cellpy-1.0.0a3/docs/source/cellpy.readers.instruments.configurations.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/source/cellpy.readers.instruments.loader_specific_modules.rst` & `cellpy-1.0.0a3/docs/source/cellpy.readers.instruments.loader_specific_modules.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/source/cellpy.readers.instruments.processors.rst` & `cellpy-1.0.0a3/docs/source/cellpy.readers.instruments.processors.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/source/cellpy.readers.instruments.rst` & `cellpy-1.0.0a3/docs/source/cellpy.readers.instruments.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/source/cellpy.readers.rst` & `cellpy-1.0.0a3/docs/source/cellpy.readers.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/source/cellpy.rst` & `cellpy-1.0.0a3/docs/source/cellpy.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/source/cellpy.utils.batch_tools.rst` & `cellpy-1.0.0a3/docs/source/cellpy.utils.batch_tools.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/docs/source/cellpy.utils.rst` & `cellpy-1.0.0a3/docs/source/cellpy.utils.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a0/setup.py` & `cellpy-1.0.0a3/setup.py`

 * *Files identical despite different names*

