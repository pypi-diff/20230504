# Comparing `tmp/diameter-synthesis-0.5.3.tar.gz` & `tmp/diameter-synthesis-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diameter-synthesis-0.5.3.tar", last modified: Mon Mar 13 19:31:29 2023, max compression
+gzip compressed data, was "diameter-synthesis-0.5.4.tar", last modified: Thu May  4 10:07:33 2023, max compression
```

## Comparing `diameter-synthesis-0.5.3.tar` & `diameter-synthesis-0.5.4.tar`

### file list

```diff
@@ -1,121 +1,129 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 19:31:29.153217 diameter-synthesis-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/.auto-changelog
--rw-r--r--   0 runner    (1001) docker     (123)     9694 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/.auto-changelog-template.hbs
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/.codespellignorelines
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/.codespellrc
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/.copier-answers.yml
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 19:31:29.141217 diameter-synthesis-0.5.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 19:31:29.145218 diameter-synthesis-0.5.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/.github/workflows/commitlint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/.github/workflows/publish-sdist.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/.github/workflows/run-tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)    26553 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    35150 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-03-13 19:31:29.153217 diameter-synthesis-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/commitlint.config.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 19:31:29.145218 diameter-synthesis-0.5.3/diameter_synthesis/
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/diameter_synthesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19727 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/diameter_synthesis/build_diameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/diameter_synthesis/build_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/diameter_synthesis/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7299 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/diameter_synthesis/distribution_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/diameter_synthesis/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/diameter_synthesis/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     9102 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/diameter_synthesis/morph_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    23236 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/diameter_synthesis/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 19:31:29.145218 diameter-synthesis-0.5.3/diameter_synthesis/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/diameter_synthesis/schemas/config.json
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/diameter_synthesis/schemas/model_params.json
--rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/diameter_synthesis/simpler_diametrizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/diameter_synthesis/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/diameter_synthesis/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 19:31:29.145218 diameter-synthesis-0.5.3/diameter_synthesis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-03-13 19:31:28.000000 diameter-synthesis-0.5.3/diameter_synthesis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-03-13 19:31:29.000000 diameter-synthesis-0.5.3/diameter_synthesis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 19:31:28.000000 diameter-synthesis-0.5.3/diameter_synthesis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-13 19:31:28.000000 diameter-synthesis-0.5.3/diameter_synthesis.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-03-13 19:31:28.000000 diameter-synthesis-0.5.3/diameter_synthesis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-13 19:31:28.000000 diameter-synthesis-0.5.3/diameter_synthesis.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 19:31:29.145218 diameter-synthesis-0.5.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 19:31:29.145218 diameter-synthesis-0.5.3/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/docs/source/api_ref.rst
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/docs/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/docs/source/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/docs/source/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/docs/source/params_and_distrs.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 19:31:29.145218 diameter-synthesis-0.5.3/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/examples/diametrizer_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/examples/get_morphologies.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/examples/model_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/examples/rediametrize_single_neuron.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      740 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/examples/run.sh
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/package.json
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-13 19:31:29.153217 diameter-synthesis-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 19:31:29.149217 diameter-synthesis-0.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10368 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 19:31:29.149217 diameter-synthesis-0.5.3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    90432 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/tests/data/C030796A-P3.h5
--rw-r--r--   0 runner    (1001) docker     (123)    90432 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/tests/data/C030796A-P3_diametrized.h5
--rw-r--r--   0 runner    (1001) docker     (123)    21120 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/tests/data/C030796A-P3_lite.h5
--rw-r--r--   0 runner    (1001) docker     (123)    21216 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/tests/data/C030796A-P3_lite_diametrized.h5
--rw-r--r--   0 runner    (1001) docker     (123)    21216 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/tests/data/C030796A-P3_lite_diametrized_1_sample.h5
--rw-r--r--   0 runner    (1001) docker     (123)    21216 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/tests/data/C030796A-P3_lite_diametrized_astrocyte.h5
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/tests/data/astro_model_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/tests/data/astro_model_params.json
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/tests/data/config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/tests/data/model_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/tests/data/model_params.json
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/tests/data/neurondb.dat
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/tests/data/simpler_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/tests/data/simpler_model_data.json
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/tests/data/simpler_model_params.json
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/tests/data/simpler_morph_diametrized.asc
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/tests/data/small_morph_apical_diametrized.asc
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/tests/data/small_morph_diametrized.asc
--rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/tests/data/small_morph_several_apical_diametrized.asc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 19:31:29.149217 diameter-synthesis-0.5.3/tests/expected_images/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 19:31:29.141217 diameter-synthesis-0.5.3/tests/expected_images/test_cumulative_analysis/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 19:31:29.149217 diameter-synthesis-0.5.3/tests/expected_images/test_cumulative_analysis/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)    16095 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/tests/expected_images/test_cumulative_analysis/analysis/L5_TPC_A_cumulative_section_path_distances_areas.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 19:31:29.149217 diameter-synthesis-0.5.3/tests/expected_images/test_cumulative_analysis/analysis/L5_TPC_A_cumulative_section_path_distances_areas_individual/
--rw-r--r--   0 runner    (1001) docker     (123)    15483 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/tests/expected_images/test_cumulative_analysis/analysis/L5_TPC_A_cumulative_section_path_distances_areas_individual/0_L5_TPC_A_cumulative_section_path_distances_areas_C030796A-P3_lite.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    15834 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/tests/expected_images/test_cumulative_analysis/analysis/L5_TPC_A_cumulative_section_path_distances_volumes.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 19:31:29.149217 diameter-synthesis-0.5.3/tests/expected_images/test_cumulative_analysis/analysis/L5_TPC_A_cumulative_section_path_distances_volumes_individual/
--rw-r--r--   0 runner    (1001) docker     (123)    15285 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/tests/expected_images/test_cumulative_analysis/analysis/L5_TPC_A_cumulative_section_path_distances_volumes_individual/0_L5_TPC_A_cumulative_section_path_distances_volumes_C030796A-P3_lite.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 19:31:29.149217 diameter-synthesis-0.5.3/tests/expected_images/test_make_cumulative_figures/
--rw-r--r--   0 runner    (1001) docker     (123)    23980 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/tests/expected_images/test_make_cumulative_figures/cumulative_segment_radial_distances_volumes.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 19:31:29.149217 diameter-synthesis-0.5.3/tests/expected_images/test_make_cumulative_figures/cumulative_segment_radial_distances_volumes_individual/
--rw-r--r--   0 runner    (1001) docker     (123)    23424 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/tests/expected_images/test_make_cumulative_figures/cumulative_segment_radial_distances_volumes_individual/0_cumulative_segment_radial_distances_volumes.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    23980 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/tests/expected_images/test_plot_cumulative_distribution.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    56388 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/tests/expected_images/test_plot_diameter_diff_div.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    56388 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/tests/expected_images/test_plot_diameter_diff_mult.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    11650 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/tests/expected_images/test_plot_distribution_fit.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    34588 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/tests/expected_images/test_violin_analysis.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    10716 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/tests/test_build_diameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/tests/test_build_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7133 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/tests/test_distribution_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     7839 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/tests/test_main_and_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7536 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/tests/test_morph_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/tests/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/tests/test_simpler_diametrizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/tests/test_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/tests/testing_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-03-13 19:31:25.000000 diameter-synthesis-0.5.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:07:33.821376 diameter-synthesis-0.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/.auto-changelog
+-rw-r--r--   0 runner    (1001) docker     (123)    10972 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/.auto-changelog-template.hbs
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/.codespellignorelines
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/.codespellrc
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:07:33.801376 diameter-synthesis-0.5.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:07:33.805376 diameter-synthesis-0.5.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/.github/ISSUE_TEMPLATE/feature_request.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/.github/ISSUE_TEMPLATE/how_to_use.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:07:33.805376 diameter-synthesis-0.5.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/.github/workflows/commitlint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/.github/workflows/publish-sdist.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/.github/workflows/run-tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    27268 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35150 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-05-04 10:07:33.821376 diameter-synthesis-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/commitlint.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:07:33.805376 diameter-synthesis-0.5.4/diameter_synthesis/
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/diameter_synthesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19725 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/diameter_synthesis/build_diameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8965 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/diameter_synthesis/build_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/diameter_synthesis/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7299 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/diameter_synthesis/distribution_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/diameter_synthesis/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/diameter_synthesis/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9102 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/diameter_synthesis/morph_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23272 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/diameter_synthesis/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:07:33.809376 diameter-synthesis-0.5.4/diameter_synthesis/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/diameter_synthesis/schemas/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/diameter_synthesis/schemas/model_params.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/diameter_synthesis/simpler_diametrizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/diameter_synthesis/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/diameter_synthesis/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:07:33.809376 diameter-synthesis-0.5.4/diameter_synthesis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-05-04 10:07:33.000000 diameter-synthesis-0.5.4/diameter_synthesis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-05-04 10:07:33.000000 diameter-synthesis-0.5.4/diameter_synthesis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 10:07:33.000000 diameter-synthesis-0.5.4/diameter_synthesis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-04 10:07:33.000000 diameter-synthesis-0.5.4/diameter_synthesis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-04 10:07:33.000000 diameter-synthesis-0.5.4/diameter_synthesis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-04 10:07:33.000000 diameter-synthesis-0.5.4/diameter_synthesis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:07:33.809376 diameter-synthesis-0.5.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:07:33.809376 diameter-synthesis-0.5.4/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/docs/source/api_ref.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/docs/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/docs/source/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/docs/source/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/docs/source/params_and_distrs.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:07:33.809376 diameter-synthesis-0.5.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/examples/diametrizer_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/examples/get_morphologies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/examples/model_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/examples/rediametrize_single_neuron.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      740 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/examples/run.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 10:07:33.821376 diameter-synthesis-0.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:07:33.813376 diameter-synthesis-0.5.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10368 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:07:33.817376 diameter-synthesis-0.5.4/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    90432 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/data/C030796A-P3.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    90432 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/data/C030796A-P3_diametrized.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    21120 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/data/C030796A-P3_lite.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    21216 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/data/C030796A-P3_lite_diametrized.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    21216 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/data/C030796A-P3_lite_diametrized_1_sample.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    21216 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/data/C030796A-P3_lite_diametrized_astrocyte.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/data/astro_model_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/data/astro_model_params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/data/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/data/model_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/data/model_params.json
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/data/neurondb.dat
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/data/simpler_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/data/simpler_model_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/data/simpler_model_params.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/data/simpler_morph_diametrized.asc
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/data/small_morph_apical_diametrized.asc
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/data/small_morph_diametrized.asc
+-rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/data/small_morph_several_apical_diametrized.asc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:07:33.817376 diameter-synthesis-0.5.4/tests/expected_images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:07:33.797376 diameter-synthesis-0.5.4/tests/expected_images/test_cumulative_analysis/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:07:33.817376 diameter-synthesis-0.5.4/tests/expected_images/test_cumulative_analysis/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)    16095 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/expected_images/test_cumulative_analysis/analysis/L5_TPC_A_cumulative_section_path_distances_areas.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:07:33.817376 diameter-synthesis-0.5.4/tests/expected_images/test_cumulative_analysis/analysis/L5_TPC_A_cumulative_section_path_distances_areas_individual/
+-rw-r--r--   0 runner    (1001) docker     (123)    15483 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/expected_images/test_cumulative_analysis/analysis/L5_TPC_A_cumulative_section_path_distances_areas_individual/0_L5_TPC_A_cumulative_section_path_distances_areas_C030796A-P3_lite.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    15834 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/expected_images/test_cumulative_analysis/analysis/L5_TPC_A_cumulative_section_path_distances_volumes.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:07:33.817376 diameter-synthesis-0.5.4/tests/expected_images/test_cumulative_analysis/analysis/L5_TPC_A_cumulative_section_path_distances_volumes_individual/
+-rw-r--r--   0 runner    (1001) docker     (123)    15285 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/expected_images/test_cumulative_analysis/analysis/L5_TPC_A_cumulative_section_path_distances_volumes_individual/0_L5_TPC_A_cumulative_section_path_distances_volumes_C030796A-P3_lite.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:07:33.817376 diameter-synthesis-0.5.4/tests/expected_images/test_make_cumulative_figures/
+-rw-r--r--   0 runner    (1001) docker     (123)    23980 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/expected_images/test_make_cumulative_figures/cumulative_segment_radial_distances_volumes.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:07:33.817376 diameter-synthesis-0.5.4/tests/expected_images/test_make_cumulative_figures/cumulative_segment_radial_distances_volumes_individual/
+-rw-r--r--   0 runner    (1001) docker     (123)    23424 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/expected_images/test_make_cumulative_figures/cumulative_segment_radial_distances_volumes_individual/0_cumulative_segment_radial_distances_volumes.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    23980 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/expected_images/test_plot_cumulative_distribution.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    56388 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/expected_images/test_plot_diameter_diff_div.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    56388 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/expected_images/test_plot_diameter_diff_mult.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    11650 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/expected_images/test_plot_distribution_fit.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    34588 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/expected_images/test_violin_analysis.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    10716 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/test_build_diameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/test_build_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7133 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/test_distribution_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7536 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/test_morph_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/test_simpler_diametrizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/test_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/testing_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tox.ini
```

### Comparing `diameter-synthesis-0.5.3/.auto-changelog` & `diameter-synthesis-0.5.4/.auto-changelog`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'ignoreCommitPattern'": "'Release:? [0-9]+\\\\.[0-9]+\\\\.[0-9]+|Update "*

 * *                          "CHANGELOG.*|.*\\\\[skip-changelog\\\\].*|\\\\[pre-commit.ci\\\\]'"}*

```diff
@@ -1,12 +1,12 @@
 {
     "backfillLimit": false,
     "commitLimit": false,
     "commitUrl": "https://github.com/BlueBrain/diameter-synthesis/commit/{id}",
     "compareUrl": "https://github.com/BlueBrain/diameter-synthesis/compare/{from}..{to}",
-    "ignoreCommitPattern": "Release [0-9]+\\.[0-9]+\\.[0-9]+|Update CHANGELOG.*|.*\\[skip-changelog\\].*|\\[pre-commit.ci\\]",
+    "ignoreCommitPattern": "Release:? [0-9]+\\.[0-9]+\\.[0-9]+|Update CHANGELOG.*|.*\\[skip-changelog\\].*|\\[pre-commit.ci\\]",
     "issueUrl": "https://github.com/BlueBrain/diameter-synthesis/issues/{id}",
     "mergeUrl": "https://github.com/BlueBrain/diameter-synthesis/pull/{id}",
     "output": "CHANGELOG.md",
     "startingVersion": "0.4.2",
     "template": ".auto-changelog-template.hbs"
 }
```

### Comparing `diameter-synthesis-0.5.3/.auto-changelog-template.hbs` & `diameter-synthesis-0.5.4/.auto-changelog-template.hbs`

 * *Files 13% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 • This template tries to follow conventional commits format https://www.conventionalcommits.org/en/v1.0.0/
 • The template uses regex to filter commit types into their own headings (this is more than just fixes and features headings)
 • It also uses the replaceText function in package.json to remove the commit type text from the message, because the headers are shown instead.
 • The text 'Breaking:' or 'Breaking changes:' can be located anywhere in the commit.
 • The types feat:, fix:, chore:, docs:, refactor:, test:, style:, perf: must be at the beginning of the commit subject with an : on end.
    • They can optionally have a scope set to outline the module or component that is affected eg feat(bldAssess):
 • There is a short hash on the end of every commit that is currently commented out so that change log did not grow too long (due to some system's file size limitations).  You can uncomment if you wish [`{{shorthash}}`]({{href}})
+
 Example Definitions
 • feat: A new feature
 • fix: A bug fix
 • perf: A code change that improves performance
 • refactor: A code change that neither fixes a bug nor adds a feature
 • style: Changes that do not affect the meaning of the code (white-space, formatting, spelling mistakes, missing semi-colons, etc)
 • test: Adding missing tests or correcting existing tests
@@ -26,14 +27,18 @@
          • For items that define a scope eg feat(bldAssess): We remove the 1st bracket and then re-add it so we can select the right piece of text
 {
   "name": "my-awesome-package",
   "auto-changelog": {
     "replaceText": {
       "([bB]reaking:)": "",
       "([bB]reaking change:)": "",
+      "(^[bB]uild:)": "",
+      "(^[bB]uild\\()": "\\(",
+      "(^[dD]eprecate:)": "",
+      "(^[dD]eprecate\\()": "\\(",
       "(^[fF]eat:)": "",
       "(^[fF]eat\\()": "\\(",
       "(^[fF]ix:)": "",
       "(^[fF]ix\\()": "\\(",
       "(^[cC]hore:)": "",
       "(^[cC]hore\\()": "\\(",
       "(^[dD]ocs:)": "",
@@ -55,15 +60,15 @@
  Regex reminders
  ^ = starts with
  \( = ( character (otherwise it is interpreted as a regex lookup group)
  * = zero or more of the previous character
  \s = whitespace
  . = any character except newline
  | = or
- [aA] = charcter a or character A
+ [aA] = character a or character A
  --}}
 
 
 {{#each releases}}
   {{#if href}}
     ## [{{title}}]({{href}})
   {{else}}
@@ -77,21 +82,29 @@
   {{/if}}
 
   {{! List commits that fix a given issues}}
   {{#each fixes}}
     - {{#if commit.breaking}}**Breaking change:** {{/if}}{{commit.subject}}{{#each fixes}} ({{author}}{{#if href}} - [#{{id}}]({{href}}){{/if}}){{/each}}
   {{/each}}
 
-  {{! List commits with 'breaking:' or 'Breaking change:' anywhere in the message under a heading}}
+  {{! List merge commits with 'breaking:' or 'Breaking change:' anywhere in the message under a heading}}
   {{#commit-list merges heading='### Breaking Changes :warning:' message='[bB]reaking [cC]hange:|[bB]reaking:' exclude='\[skip-changelog\]'}}
     - {{message}} @{{author}}  <!--[`#{{id}}`]({{href}}) -->
   {{/commit-list}}
 
   {{! List commits organised under a heading, but not those already listed in the breaking section }}
-      {{#commit-list merges heading='### New Features' message='^[fF]eat:|[fF]eat\(' exclude='[bB]reaking [cC]hange:|[bB]reaking:|\[skip-changelog\]'}}
+      {{#commit-list merges heading='### Build' message='^[bB]uild:|^[bB]uild\(' exclude='[bB]reaking [cC]hange:|[bB]reaking:|\[skip-changelog\]'}}
+        - {{message}} ({{author}}{{#if href}} - [#{{id}}]({{href}}){{/if}})
+      {{/commit-list}}
+
+      {{#commit-list merges heading='### Deprecated Features' message='^[dD]eprecate:|^[dD]eprecate\(' exclude='[bB]reaking [cC]hange:|[bB]reaking:|\[skip-changelog\]'}}
+        - {{message}} ({{author}}{{#if href}} - [#{{id}}]({{href}}){{/if}})
+      {{/commit-list}}
+
+      {{#commit-list merges heading='### New Features' message='^[fF]eat:|^[fF]eat\(' exclude='[bB]reaking [cC]hange:|[bB]reaking:|\[skip-changelog\]'}}
         - {{message}} ({{author}}{{#if href}} - [#{{id}}]({{href}}){{/if}})
       {{/commit-list}}
 
       {{#commit-list merges heading='### Fixes' message='^[fF]ix:|^[fF]ix\(' exclude='[bB]reaking [cC]hange:|[bB]reaking:|\[skip-changelog\]'}}
         - {{message}} ({{author}}{{#if href}} - [#{{id}}]({{href}}){{/if}})
       {{/commit-list}}
 
@@ -119,25 +132,33 @@
         - {{message}} ({{author}}{{#if href}} - [#{{id}}]({{href}}){{/if}})
       {{/commit-list}}
 
       {{#commit-list merges heading='### CI Improvements' message='^[cC][iI]:|^[cC][iI]\(' exclude='[bB]reaking [cC]hange:|[bB]reaking:|\[skip-changelog\]'}}
         - {{message}} ({{author}}{{#if href}} - [#{{id}}]({{href}}){{/if}})
       {{/commit-list}}
 
-      {{#commit-list merges heading='### Uncategorized Changes' exclude='[bB]reaking [cC]hange:|[bB]reaking:|^[fF]eat:|^[fF]eat\(|^[fF]ix:|^[fF]ix\(|^[cC]hore:|^[cC]hore\(|^[cC][iI]:|^[cC][iI]\(|^[dD]ocs:|^[dD]ocs\(|^[rR]efactor:|^[rR]efactor\(|^[tT]est:|^[tT]est\(|^[sS]tyle:|^[sS]tyle\(|^[pP]erf:|^[pP]erf\(|\[skip-changelog\]'}}
+      {{#commit-list merges heading='### General Changes' exclude='[bB]reaking [cC]hange:|[bB]reaking:|^[bB]uild:|^[bB]uild\(|^[dD]eprecate:|^[dD]eprecate\(|^[fF]eat:|^[fF]eat\(|^[fF]ix:|^[fF]ix\(|^[cC]hore:|^[cC]hore\(|^[cC][iI]:|^[cC][iI]\(|^[dD]ocs:|^[dD]ocs\(|^[rR]efactor:|^[rR]efactor\(|^[tT]est:|^[tT]est\(|^[sS]tyle:|^[sS]tyle\(|^[pP]erf:|^[pP]erf\(|\[skip-changelog\]'}}
         - {{message}} ({{author}}{{#if href}} - [#{{id}}]({{href}}){{/if}})
       {{/commit-list}}
 
   {{! List commits with 'breaking:' or 'Breaking change:' anywhere in the message under a heading}}
   {{#commit-list commits heading='### Breaking Changes :warning:' message='[bB]reaking [cC]hange:|[bB]reaking:' exclude='\[skip-changelog\]'}}
     - {{subject}} ({{author}}{{#if href}} - [{{shorthash}}]({{href}}){{/if}})
   {{/commit-list}}
 
   {{! List commits organised under a heading, but not those already listed in the breaking section }}
-      {{#commit-list commits heading='### New Features' message='^[fF]eat:|[fF]eat\(' exclude='[bB]reaking [cC]hange:|[bB]reaking:|\[skip-changelog\]'}}
+      {{#commit-list commits heading='### Build' message='^[bB]uild:|^[bB]uild\(' exclude='[bB]reaking [cC]hange:|[bB]reaking:|\[skip-changelog\]'}}
+        - {{subject}} ({{author}}{{#if href}} - [{{shorthash}}]({{href}}){{/if}})
+      {{/commit-list}}
+
+      {{#commit-list commits heading='### Deprecated Features' message='^[dD]eprecate:|^[dD]eprecate\(' exclude='[bB]reaking [cC]hange:|[bB]reaking:|\[skip-changelog\]'}}
+        - {{subject}} ({{author}}{{#if href}} - [{{shorthash}}]({{href}}){{/if}})
+      {{/commit-list}}
+
+      {{#commit-list commits heading='### New Features' message='^[fF]eat:|^[fF]eat\(' exclude='[bB]reaking [cC]hange:|[bB]reaking:|\[skip-changelog\]'}}
         - {{subject}} ({{author}}{{#if href}} - [{{shorthash}}]({{href}}){{/if}})
       {{/commit-list}}
 
       {{#commit-list commits heading='### Fixes' message='^[fF]ix:|^[fF]ix\(' exclude='[bB]reaking [cC]hange:|[bB]reaking:|\[skip-changelog\]'}}
         - {{subject}} ({{author}}{{#if href}} - [{{shorthash}}]({{href}}){{/if}})
       {{/commit-list}}
 
@@ -165,12 +186,12 @@
         - {{subject}} ({{author}}{{#if href}} - [{{shorthash}}]({{href}}){{/if}})
       {{/commit-list}}
 
       {{#commit-list commits heading='### CI Improvements' message='^[cC][iI]:|^[cC][iI]\(' exclude='[bB]reaking [cC]hange:|[bB]reaking:|\[skip-changelog\]'}}
         - {{subject}} ({{author}}{{#if href}} - [{{shorthash}}]({{href}}){{/if}})
       {{/commit-list}}
 
-      {{#commit-list commits heading='### Uncategorized Changes' exclude='[bB]reaking [cC]hange:|[bB]reaking:|^[fF]eat:|^[fF]eat\(|^[fF]ix:|^[fF]ix\(|^[cC]hore:|^[cC]hore\(|^[cC][iI]:|^[cC][iI]\(|^[dD]ocs:|^[dD]ocs\(|^[rR]efactor:|^[rR]efactor\(|^[tT]est:|^[tT]est\(|^[sS]tyle:|^[sS]tyle\(|^[pP]erf:|^[pP]erf\(|\[skip-changelog\]'}}
+      {{#commit-list commits heading='### General Changes' exclude='[bB]reaking [cC]hange:|[bB]reaking:|^[bB]uild:|^[bB]uild\(|^[dD]eprecate:|^[dD]eprecate\(|^[fF]eat:|^[fF]eat\(|^[fF]ix:|^[fF]ix\(|^[cC]hore:|^[cC]hore\(|^[cC][iI]:|^[cC][iI]\(|^[dD]ocs:|^[dD]ocs\(|^[rR]efactor:|^[rR]efactor\(|^[tT]est:|^[tT]est\(|^[sS]tyle:|^[sS]tyle\(|^[pP]erf:|^[pP]erf\(|\[skip-changelog\]'}}
         - {{subject}} ({{author}}{{#if href}} - [{{shorthash}}]({{href}}){{/if}})
       {{/commit-list}}
 
 {{/each}}
```

### Comparing `diameter-synthesis-0.5.3/.copier-answers.yml` & `diameter-synthesis-0.5.4/.copier-answers.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 # Changes here will be overwritten by Copier
 
-_commit: 0.1.7
+_commit: 0.1.43
 _src_path: git@bbpgitlab.epfl.ch:neuromath/python-template.git
 author_email: ''
 author_name: Blue Brain Project, EPFL
 copyright_license: GNU General Public License v3.0
 copyright_year: '2022'
+distribution_name: diameter-synthesis
 download_url: git@github.com:BlueBrain/diameter-synthesis.git
 init_git: false
 maintainer: Alexis Arnaudon (@arnaudon)
 package_name: diameter_synthesis
 project_description: Diametrize cells.
 project_name: diameter-synthesis
 project_url: https://diameter-synthesis.readthedocs.io
-repository: BlueBrain/diameter-synthesis
+repository_name: diameter-synthesis
+repository_namespace: BlueBrain
 repository_provider: github
+ssh_url: git@github.com:BlueBrain/diameter-synthesis.git
 support_py37: false
 team_name: ''
-today: 29 August 2022
 tracker_url: https://github.com/BlueBrain/diameter-synthesis/issues
+use_pyproject_toml: false
 version: 0.5.1
 
 # End of Copier answers
```

### Comparing `diameter-synthesis-0.5.3/.github/workflows/commitlint.yml` & `diameter-synthesis-0.5.4/.github/workflows/commitlint.yml`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     types: [edited, opened, reopened, synchronize]
 
 jobs:
   check-pr-title:
     name: Check PR title
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@master
-      - uses: actions/setup-node@v2
+      - uses: actions/checkout@v3
+      - uses: actions/setup-node@v3
         with:
-          node-version: '14'
+          node-version: '16'
       - run: npm install -g --force commitlint @commitlint/cli commitlint-plugin-cleanfeet
       - run: npm install conventional-changelog-conventionalcommits
       - run: touch .git/COMMIT_EDITMSG
-      - run: echo ${{ github.event.pull_request.title }} | commitlint
+      - run: echo "${{ github.event.pull_request.title }}" | commitlint
```

### Comparing `diameter-synthesis-0.5.3/.github/workflows/publish-sdist.yml` & `diameter-synthesis-0.5.4/.github/workflows/publish-sdist.yml`

 * *Files 20% similar despite different names*

```diff
@@ -6,22 +6,22 @@
       - '[0-9]+.[0-9]+.[0-9]+'
 
 jobs:
   build-n-publish:
     name: Build and publish on PyPI
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@master
+      - uses: actions/checkout@v3
       - name: Set up Python 3.8
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: 3.8
       - name: Build a wheel and a source tarball
         run: |
-          pip install setuptools>=42 wheel setuptools_scm[toml]>=3.4
-          python setup.py sdist bdist_wheel
+          pip install setuptools>=42 build setuptools_scm[toml]>=3.4
+          python -m build -o dist
       - name: Publish distribution package to PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           user: ${{ secrets.DEVPI_USER }}
           password: ${{ secrets.DEVPI_PASSWORD }}
           repository_url: ${{ secrets.DEVPI_URL }}
```

### Comparing `diameter-synthesis-0.5.3/.pre-commit-config.yaml` & `diameter-synthesis-0.5.4/.pre-commit-config.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 default_language_version:
   python: python3.8
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.3.0
+    rev: v4.4.0
     hooks:
       - id: check-added-large-files
       - id: check-case-conflict
       - id: check-merge-conflict
       - id: check-symlinks
       - id: check-yaml
       - id: debug-statements
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/alessandrojcm/commitlint-pre-commit-hook
-    rev: v9.0.0
+    rev: v9.5.0
     hooks:
         - id: commitlint
           stages:
             - commit-msg
           additional_dependencies: ['conventional-changelog-conventionalcommits']
   - repo: https://github.com/pycqa/isort
-    rev: 5.10.1
+    rev: 5.12.0
     hooks:
       - id: isort
   - repo: https://github.com/psf/black
-    rev: 22.6.0
+    rev: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.1.0
+    rev: v2.2.4
     hooks:
       - id: codespell
         args: ["-x", ".codespellignorelines"]
   - repo: https://github.com/PyCQA/pydocstyle
-    rev: 6.1.1
+    rev: 6.3.0
     hooks:
       - id: pydocstyle
-        additional_dependencies: ["toml"]
+        additional_dependencies: ["tomli"]
   - repo: https://github.com/PyCQA/flake8
-    rev: 5.0.4
+    rev: 6.0.0
     hooks:
       - id: flake8
```

### Comparing `diameter-synthesis-0.5.3/.pylintrc` & `diameter-synthesis-0.5.4/.pylintrc`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.3/CHANGELOG.md` & `diameter-synthesis-0.5.4/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,51 +1,75 @@
 # Changelog
 
+## [0.5.4](https://github.com/BlueBrain/diameter-synthesis/compare/0.5.3..0.5.4)
+
+> 4 May 2023
+
+### Fixes
+
+- Handle missing neurites in simpler model (Adrien Berchet - [#36](https://github.com/BlueBrain/diameter-synthesis/pull/36))
+
+### Chores And Housekeeping
+
+- Add templates for issues and pull requests (Adrien Berchet - [#37](https://github.com/BlueBrain/diameter-synthesis/pull/37))
+- Bump copier template (Adrien Berchet - [#34](https://github.com/BlueBrain/diameter-synthesis/pull/34))
+
+## [0.5.3](https://github.com/BlueBrain/diameter-synthesis/compare/0.5.2..0.5.3)
+
+> 6 September 2022
+
+### General Changes
+
+- Fixing small bug (Alexis Arnaudon - [#32](https://github.com/BlueBrain/diameter-synthesis/pull/32))
+
 ## [0.5.2](https://github.com/BlueBrain/diameter-synthesis/compare/0.5.1..0.5.2)
 
 > 31 August 2022
 
 ### Refactoring and Updates
 
 - Apply Copier template (Adrien Berchet - [#30](https://github.com/BlueBrain/diameter-synthesis/pull/30))
 
-### Uncategorized Changes
+### General Changes
 
 - Improve simpler diametrizer (Alexis Arnaudon - [#31](https://github.com/BlueBrain/diameter-synthesis/pull/31))
 
 ## [0.5.1](https://github.com/BlueBrain/diameter-synthesis/compare/0.5.0..0.5.1)
 
 > 22 August 2022
 
 ## [0.5.0](https://github.com/BlueBrain/diameter-synthesis/compare/0.4.2..0.5.0)
 
 > 19 August 2022
 
+### Build
+
+- Fix docutils requirement as the new M2R2 release fixes it (Adrien Berchet - [#24](https://github.com/BlueBrain/diameter-synthesis/pull/24))
+
 ### Chores And Housekeeping
 
 - Use importlib instead of pkg_resources (Adrien Berchet - [#27](https://github.com/BlueBrain/diameter-synthesis/pull/27))
 
 ### CI Improvements
 
 - Setup pre-commit and format files accordingly (Adrien Berchet - [#25](https://github.com/BlueBrain/diameter-synthesis/pull/25))
 
-### Uncategorized Changes
+### General Changes
 
 - Simpler rediametrize (Alexis Arnaudon - [#26](https://github.com/BlueBrain/diameter-synthesis/pull/26))
-- Fix docutils requirement as the new M2R2 release fixes it (Adrien Berchet - [#24](https://github.com/BlueBrain/diameter-synthesis/pull/24))
 - simpler diametrizer (Alexis Arnaudon - [#22](https://github.com/BlueBrain/diameter-synthesis/pull/22))
 - Updating copyright year (bbpgithubaudit - [#21](https://github.com/BlueBrain/diameter-synthesis/pull/21))
 - Update DOI to the final article (Adrien Berchet - [#19](https://github.com/BlueBrain/diameter-synthesis/pull/19))
 - fix ordering bug in assigning daughter diameters (Alexis Arnaudon - [#18](https://github.com/BlueBrain/diameter-synthesis/pull/18))
 
 ## [0.4.2](https://github.com/BlueBrain/diameter-synthesis/compare/0.4.1..0.4.2)
 
 > 3 March 2022
 
-### Uncategorized Changes
+### General Changes
 
 - Fix asymmetry of last children in apical diametrizer (Alexis Arnaudon - [#16](https://github.com/BlueBrain/diameter-synthesis/pull/16))
 
 <!-- auto-changelog-above -->
 
 ## [0.4.1](https://github.com/BlueBrain/diameter-synthesis/compare/0.3.3..0.4.1)
```

### Comparing `diameter-synthesis-0.5.3/CITATION.cff` & `diameter-synthesis-0.5.4/CITATION.cff`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.3/CONTRIBUTING.md` & `diameter-synthesis-0.5.4/CONTRIBUTING.md`

 * *Files 2% similar despite different names*

```diff
@@ -163,8 +163,8 @@
 
   ```shell
   git branch -D release_X.Y.Z
   ```
 
 After these steps the CI should automatically build the wheel and push it to pypi.
 
-[github]: https://github.com/BlueBrain/diameter-synthesis
+[github]: git@github.com:BlueBrain/diameter-synthesis.git
```

### Comparing `diameter-synthesis-0.5.3/LICENSE.txt` & `diameter-synthesis-0.5.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.3/PKG-INFO` & `diameter-synthesis-0.5.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,96 +1,99 @@
 Metadata-Version: 2.1
 Name: diameter-synthesis
-Version: 0.5.3
+Version: 0.5.4
 Summary: Diametrize cells.
 Home-page: https://diameter-synthesis.readthedocs.io
 Author: Blue Brain Project, EPFL
 License: GNU General Public License v3.0
 Project-URL: Tracker, https://github.com/BlueBrain/diameter-synthesis/issues
 Project-URL: Source, https://github.com/BlueBrain/diameter-synthesis
-Description: [![Version](https://img.shields.io/pypi/v/diameter-synthesis)](https://github.com/BlueBrain/diameter-synthesis/releases)
-        [![Build status](https://github.com/BlueBrain/diameter-synthesis/actions/workflows/run-tox.yml/badge.svg?branch=main)](https://github.com/BlueBrain/diameter-synthesis/actions)
-        [![Codecov.io](https://codecov.io/github/BlueBrain/diameter-synthesis/coverage.svg?branch=main)](https://codecov.io/github/BlueBrain/diameter-synthesis?branch=main)
-        [![License](https://img.shields.io/badge/License-GPLv3-blue)](https://github.com/BlueBrain/diameter-synthesis/blob/main/LICENSE.txt)
-        [![Documentation status](https://readthedocs.org/projects/diameter-synthesis/badge/?version=latest)](https://diameter-synthesis.readthedocs.io/)
-        [![DOI](https://img.shields.io/badge/DOI-10.1016/j.celrep.2022.110586-blue)](https://doi.org/10.1016/j.celrep.2022.110586)
-        
-        
-        # Diameter synthesis
-        
-        This code aims at generating synthetic diameters for neurons, with parameters learned from a set of biological neurons.
-        
-        
-        ## Installation
-        
-        Use pip:
-        
-        ```bash
-        pip install diameter-synthesis
-        ```
-        
-        ## Main usage
-        
-        ### Step 1: Building models
-        
-        In folder `example`, you first have to modify `create_jsons.py` to suit your needs.
-        
-        You have the following important parameters for the dict `extract_models_params`:
-        
-        - `morph_path`: path to morphology files
-        - `mtypes_sort`: how to learn distributions: `all` to use all together, `mtypes` to use by mtypes , `super_mtypes` to use home made cells types (see `diameter_types` below)
-        - `models`: to create several models (for now they are all the same, just different realisation of random numbers)
-        - `neurite_types`: types of neurite to learn parameters for
-        - `extra_params`: dict of additional model parameters
-        
-        ### Step 2: Building diameters
-        
-        Then simply run `./run_models.sh` to create the models (saved in a json file).
-        
-        In `create_jsons.py`, the dict `generate_diameters_params` needs to be updated, too, with entries matching the previous dict.
-        The path in `new_morph_path` will be where the new morphologies will be saved.
-        
-        Then run `./run_diamters.sh` to generate diameters.
-        
-        
-        ## Additional scripts
-        
-        Several additional scripts in folder `scripts`:
-        
-        - `diameter-checks`: run the diameter-check code (bluepymm) on the biological and sampled cells
-        - `diameter_types`: cluster mtypes using distributions of surface areas (uses two privates repositories a the moment)
-        - `extract_morphometrics`: from bio and sample cells, extracts and plot distribution of surface area and diameter as a function of branch order and path lengths
-        - `extract_morphologies`: from a cell release, find the ones that can be run through diameter-check
-        - `plot_morphologies`: plot all morphologies in mtype folders
-        
-        
-        ## Examples
-        
-        The `examples` folder contains a simple example that will fetch morphologies from [neuromorpho.org](http://neuromorpho.org), learn a diameter model, rediametrize these morphologies, and perform some analysis of the results to compare original and diametrized morphologies.
-        This example can simply be run using the following command:
-        ```bash
-        ./run.sh
-        ```
-        
-        
-        ## Funding & Acknowledgment
-        
-        The development of this software was supported by funding to the Blue Brain Project, a research center of the École polytechnique fédérale de Lausanne (EPFL), from the Swiss government’s ETH Board of the Swiss Federal Institutes of Technology.
-        
-        For license and authors, see `LICENSE.txt` and `AUTHORS.md` respectively.
-        
-        Copyright © 2021-2022 Blue Brain Project/EPFL
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: plot
 Provides-Extra: test
+License-File: LICENSE.txt
+License-File: AUTHORS.md
+
+[![Version](https://img.shields.io/pypi/v/diameter-synthesis)](https://github.com/BlueBrain/diameter-synthesis/releases)
+[![Build status](https://github.com/BlueBrain/diameter-synthesis/actions/workflows/run-tox.yml/badge.svg?branch=main)](https://github.com/BlueBrain/diameter-synthesis/actions)
+[![Codecov.io](https://codecov.io/github/BlueBrain/diameter-synthesis/coverage.svg?branch=main)](https://codecov.io/github/BlueBrain/diameter-synthesis?branch=main)
+[![License](https://img.shields.io/badge/License-GPLv3-blue)](https://github.com/BlueBrain/diameter-synthesis/blob/main/LICENSE.txt)
+[![Documentation status](https://readthedocs.org/projects/diameter-synthesis/badge/?version=latest)](https://diameter-synthesis.readthedocs.io/)
+[![DOI](https://img.shields.io/badge/DOI-10.1016/j.celrep.2022.110586-blue)](https://doi.org/10.1016/j.celrep.2022.110586)
+
+
+# Diameter synthesis
+
+This code aims at generating synthetic diameters for neurons, with parameters learned from a set of biological neurons.
+
+
+## Installation
+
+Use pip:
+
+```bash
+pip install diameter-synthesis
+```
+
+## Main usage
+
+### Step 1: Building models
+
+In folder `example`, you first have to modify `create_jsons.py` to suit your needs.
+
+You have the following important parameters for the dict `extract_models_params`:
+
+- `morph_path`: path to morphology files
+- `mtypes_sort`: how to learn distributions: `all` to use all together, `mtypes` to use by mtypes , `super_mtypes` to use home made cells types (see `diameter_types` below)
+- `models`: to create several models (for now they are all the same, just different realisation of random numbers)
+- `neurite_types`: types of neurite to learn parameters for
+- `extra_params`: dict of additional model parameters
+
+### Step 2: Building diameters
+
+Then simply run `./run_models.sh` to create the models (saved in a json file).
+
+In `create_jsons.py`, the dict `generate_diameters_params` needs to be updated, too, with entries matching the previous dict.
+The path in `new_morph_path` will be where the new morphologies will be saved.
+
+Then run `./run_diamters.sh` to generate diameters.
+
+
+## Additional scripts
+
+Several additional scripts in folder `scripts`:
+
+- `diameter-checks`: run the diameter-check code (bluepymm) on the biological and sampled cells
+- `diameter_types`: cluster mtypes using distributions of surface areas (uses two privates repositories a the moment)
+- `extract_morphometrics`: from bio and sample cells, extracts and plot distribution of surface area and diameter as a function of branch order and path lengths
+- `extract_morphologies`: from a cell release, find the ones that can be run through diameter-check
+- `plot_morphologies`: plot all morphologies in mtype folders
+
+
+## Examples
+
+The `examples` folder contains a simple example that will fetch morphologies from [neuromorpho.org](http://neuromorpho.org), learn a diameter model, rediametrize these morphologies, and perform some analysis of the results to compare original and diametrized morphologies.
+This example can simply be run using the following command:
+```bash
+./run.sh
+```
+
+
+## Funding & Acknowledgment
+
+The development of this software was supported by funding to the Blue Brain Project, a research center of the École polytechnique fédérale de Lausanne (EPFL), from the Swiss government’s ETH Board of the Swiss Federal Institutes of Technology.
+
+For license and authors, see `LICENSE.txt` and `AUTHORS.md` respectively.
+
+Copyright © 2021-2022 Blue Brain Project/EPFL
```

### Comparing `diameter-synthesis-0.5.3/README.md` & `diameter-synthesis-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.3/commitlint.config.js` & `diameter-synthesis-0.5.4/commitlint.config.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -16,19 +16,21 @@
         'type-enum': [
             2,
             'always',
             [
                 'Build',
                 'Chore',
                 'CI',
+                'Deprecate',
                 'Docs',
                 'Feat',
                 'Fix',
                 'Perf',
                 'Refactor',
+                'Release',
                 'Revert',
                 'Style',
                 'Test',
             ],
         ],
     },
     prompt: {
@@ -87,14 +89,24 @@
                         emoji: '♻️',
                     },
                     Revert: {
                         description: 'Reverts a previous commit',
                         title: 'Reverts',
                         emoji: '🗑',
                     },
+                    Release: {
+                        description: 'Release commit',
+                        title: 'Release',
+                        emoji: '🎉',
+                    },
+                    Deprecate: {
+                        description: 'Deprecate a feature',
+                        title: 'Deprecations',
+                        emoji: '🗳',
+                    },
                 },
             },
             scope: {
                 description: 'What is the scope of this change (e.g. component or file name)',
             },
             subject: {
                 description: 'Write a short, imperative tense description of the change',
```

### Comparing `diameter-synthesis-0.5.3/diameter_synthesis/__init__.py` & `diameter-synthesis-0.5.4/diameter_synthesis/__init__.py`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.3/diameter_synthesis/build_diameters.py` & `diameter-synthesis-0.5.4/diameter_synthesis/build_diameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,14 @@
         if False in child_not_in_major:
             child_sort = np.argsort(child_not_in_major)
             apply_asymmetry = True
 
     reduction_factor = params_tree["reduction_factor_max"] + 1.0
     # try until we get a reduction of diameter in the branching
     while reduction_factor > params_tree["reduction_factor_max"]:
-
         sibling_ratio = _sample_sibling_ratio(
             params,
             params_tree["neurite_type"],
             apply_asymmetry=apply_asymmetry,
             mode=params_tree["mode_sibling"],
             rng=rng,
         )
@@ -359,15 +358,14 @@
     Args:
         model (str): model name.
 
     Returns:
         function: diametrizer with specific `params_tree`.
     """
     if model == "simpler":
-
         return simpler_diametrizer
 
     if model == "generic":
         params_tree = {}
         params_tree["mode_sibling"] = "threshold"
         params_tree["mode_diameter_power_relation"] = "threshold"
         params_tree["with_asymmetry"] = True
```

### Comparing `diameter-synthesis-0.5.3/diameter_synthesis/build_models.py` & `diameter-synthesis-0.5.4/diameter_synthesis/build_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,14 @@
         "terminal_diameters": {},
         "trunk_diameters": {},
         "tapers": {},
     }
 
     extra_params = config.copy()
     for neurite_type in config["neurite_types"]:
-
         extra_params["neurite_type"] = neurite_type
         extra_params["name"] = "sibling_ratios"
         all_models["sibling_ratios"][neurite_type] = fit_model(
             sampling_model["sibling_ratios"],
             all_data["sibling_ratios"][neurite_type],
             extra_params,
         )
```

### Comparing `diameter-synthesis-0.5.3/diameter_synthesis/cli.py` & `diameter-synthesis-0.5.4/diameter_synthesis/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Click app for the diameter-synthesis package."""
+"""Command Line Interface for the diameter_synthesis package."""
 
 # Copyright (C) 2021  Blue Brain Project, EPFL
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -28,40 +28,41 @@
 
 morphio.set_maximum_warnings(0)
 L = logging.getLogger(__name__)
 logging.basicConfig(level=os.environ.get("LOGLEVEL", "INFO"))
 
 
 @click.group()
-def cli():
+@click.version_option(prog_name="diameter-synthesis")
+def main():
     """Cli to learn and generate diameters of neurons."""
 
 
-@cli.command("run_models")
+@main.command("run_models")
 @click.argument("config_file", type=click.Path(exists=True))
 @click.option("--plot", is_flag=True)
 @click.option("--ext", default=".png")
 def run_models(config_file, plot=False, ext=".png"):
     """Run the model extraction from config file."""
     from .main import run_models
 
     run_models(config_file, plot=plot, ext=ext)
 
 
-@cli.command("run_diameters")
+@main.command("run_diameters")
 @click.argument("config_file", type=click.Path(exists=True))
 @click.argument("models_params_file", type=click.Path(exists=True))
 def run_diameters(config_file, models_params_file):
     """Build new diameters from config file and diameter model."""
     from .main import run_diameters
 
     run_diameters(config_file, models_params_file)
 
 
-@cli.command("plot_diff")
+@main.command("plot_diff")
 @click.option("--orig-path", help="Path to original cells", required=True)
 @click.option("--diam-path", help="Path to diametrized cells", required=True)
 @click.option("-o", "--out-dir", help="Directory to output the analysis results", required=True)
 @click.option("-n", "--ncells", default=10, help="Max number of cells to plot")
 @click.option("-e", "--ext", default=".png", help="Figures extension")
 def plot_diff(orig_path, diam_path, out_dir, ncells=None, ext=".png"):
     """Plot original and new neurons as well as their differences."""
@@ -90,15 +91,15 @@
             neurons = morphologies_dict[mtype]
 
         for neuron in tqdm(neurons):
             neuron_new = nm.load_morphology(Path(diam_path) / neuron.name)
             plot_diameter_diff(neuron, neuron_new, neurite_types, plot_folder_mtype, ext=ext)
 
 
-@cli.command("run_analysis")
+@main.command("run_analysis")
 @click.option("--orig-path", help="Path to original cells", required=True)
 @click.option("--diam-path", help="Path to diametrized cells", required=True)
 @click.option("--mtypes-file", help="Path to mtypes file", required=False)
 @click.option("-o", "--out-dir", help="Directory to output the analysis results", required=True)
 @click.option("--cumulative", help="Cumulative distribution plots", is_flag=True)
 @click.option("--individual", help="Output a plot for each neuron", is_flag=True)
 @click.option("--violin", help="Violin distribution plots", is_flag=True)
```

### Comparing `diameter-synthesis-0.5.3/diameter_synthesis/distribution_fitting.py` & `diameter-synthesis-0.5.4/diameter_synthesis/distribution_fitting.py`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.3/diameter_synthesis/exception.py` & `diameter-synthesis-0.5.4/diameter_synthesis/exception.py`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.3/diameter_synthesis/main.py` & `diameter-synthesis-0.5.4/diameter_synthesis/main.py`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.3/diameter_synthesis/morph_functions.py` & `diameter-synthesis-0.5.4/diameter_synthesis/morph_functions.py`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.3/diameter_synthesis/plotting.py` & `diameter-synthesis-0.5.4/diameter_synthesis/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -244,41 +244,40 @@
 
     def create_bins(step_size, max_value):
         bins = np.arange(0.0, max_value + step_size, step_size)
         bin_centers = 0.5 * step_size + bins[:-1]
         return bin_centers, bins
 
     def find_upper_bound(pairs):
+        # pylint: disable=nested-min-max
         return max(max(max(vals1), max(vals2)) for (vals1, _), (vals2, _) in pairs)
 
     def per_neurite_data(original_cells, diametrized_cells, neurite_types):
         for _, neurite_type in enumerate(neurite_types):
             data = list(create_paired_features(original_cells, diametrized_cells, neurite_type))
             if len(data[0][0][0]) > 0:
                 yield data
 
     assert len(original_cells) == len(diametrized_cells)
 
     n_cells = len(original_cells)
     iter_neurite_data = per_neurite_data(original_cells, diametrized_cells, neurite_types)
     for _, data_pairs in enumerate(iter_neurite_data):
-
         try:
             upper_bound = find_upper_bound(data_pairs)
         except BaseException:  # pylint: disable=broad-except
             L.exception("failed to find upper bound, most likely due to no data points")
             upper_bound = 200
 
         bin_centers, bins = create_bins(step_size, upper_bound)
 
         stats1 = np.empty((n_cells, len(bin_centers)), dtype=float)
         stats2 = np.empty_like(stats1)
 
         for i, ((metric1, data1), (metric2, data2)) in enumerate(data_pairs):
-
             res1 = stats.binned_statistic(
                 metric1, data1, statistic="sum", bins=bins, range=(0, upper_bound)
             )
             res2 = stats.binned_statistic(
                 metric2, data2, statistic="sum", bins=bins, range=(0, upper_bound)
             )
 
@@ -322,16 +321,15 @@
 
     data_generator = _create_data(
         feature1, feature2, original_cells, diametrized_cells, step_size, neurite_types
     )
 
     fig, axes = plt.subplots(3, 1, figsize=(5, 12))
 
-    for (bin_centers, stats1, stats2) in data_generator:
-
+    for bin_centers, stats1, stats2 in data_generator:
         means = stats1.mean(axis=0)
         color = "C0"
         axes[0].plot(bin_centers, means, c=color, linestyle="-", lw=3, label="original cells")
 
         if len(stats1) > 1:
             for st1 in stats1:
                 axes[0].plot(bin_centers, st1, c=color, linestyle="-", lw=0.5, alpha=0.2)
```

### Comparing `diameter-synthesis-0.5.3/diameter_synthesis/schemas/config.json` & `diameter-synthesis-0.5.4/diameter_synthesis/schemas/config.json`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.3/diameter_synthesis/schemas/model_params.json` & `diameter-synthesis-0.5.4/diameter_synthesis/schemas/model_params.json`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.3/diameter_synthesis/simpler_diametrizer.py` & `diameter-synthesis-0.5.4/diameter_synthesis/simpler_diametrizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,16 +32,16 @@
     """Build diameter model."""
     neurite_types = config.get("neurite_types")
     if neurite_types is None:
         neurite_types = ["basal_dendrite", "apical_dendrite"]
     if fit_orders is None:
         fit_orders = {"basal_dendrite": 1, "apical_dendrite": 2, "axon": 1}
 
-    coeffs = {}
-    residues = {}
+    coeffs = {n_type: [] for n_type in neurite_types}
+    residues = {n_type: None for n_type in neurite_types}
     all_diams = {n_type: [] for n_type in neurite_types}
     all_lengths = {n_type: [] for n_type in neurite_types}
 
     for neurite_type in neurite_types:
         for m in morphologies:
             diams = []
             lengths = []
@@ -52,19 +52,23 @@
                         diams.append(2 * np.mean(section.points[:, 3]))
                         tip_length = max(
                             section_path_length(_section, cache) for _section in section.ipreorder()
                         )
                         lengths.append(
                             tip_length - section_path_length(section, cache) + section.length
                         )
+            if not diams:
+                continue
             lengths = np.array(lengths)
             diams = np.array(diams)
             lengths /= lengths.max()
             all_lengths[neurite_type] += lengths.tolist()
             all_diams[neurite_type] += diams.tolist()
+        if not all_diams[neurite_type]:
+            continue
         p, extra = Polynomial.fit(
             all_lengths[neurite_type],
             all_diams[neurite_type],
             fit_orders[neurite_type],
             full=True,
         )
         residues[neurite_type] = float(extra[0][0])
```

### Comparing `diameter-synthesis-0.5.3/diameter_synthesis/utils.py` & `diameter-synthesis-0.5.4/diameter_synthesis/utils.py`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.3/diameter_synthesis/validators.py` & `diameter-synthesis-0.5.4/diameter_synthesis/validators.py`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.3/diameter_synthesis.egg-info/PKG-INFO` & `diameter-synthesis-0.5.4/diameter_synthesis.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,96 +1,99 @@
 Metadata-Version: 2.1
 Name: diameter-synthesis
-Version: 0.5.3
+Version: 0.5.4
 Summary: Diametrize cells.
 Home-page: https://diameter-synthesis.readthedocs.io
 Author: Blue Brain Project, EPFL
 License: GNU General Public License v3.0
 Project-URL: Tracker, https://github.com/BlueBrain/diameter-synthesis/issues
 Project-URL: Source, https://github.com/BlueBrain/diameter-synthesis
-Description: [![Version](https://img.shields.io/pypi/v/diameter-synthesis)](https://github.com/BlueBrain/diameter-synthesis/releases)
-        [![Build status](https://github.com/BlueBrain/diameter-synthesis/actions/workflows/run-tox.yml/badge.svg?branch=main)](https://github.com/BlueBrain/diameter-synthesis/actions)
-        [![Codecov.io](https://codecov.io/github/BlueBrain/diameter-synthesis/coverage.svg?branch=main)](https://codecov.io/github/BlueBrain/diameter-synthesis?branch=main)
-        [![License](https://img.shields.io/badge/License-GPLv3-blue)](https://github.com/BlueBrain/diameter-synthesis/blob/main/LICENSE.txt)
-        [![Documentation status](https://readthedocs.org/projects/diameter-synthesis/badge/?version=latest)](https://diameter-synthesis.readthedocs.io/)
-        [![DOI](https://img.shields.io/badge/DOI-10.1016/j.celrep.2022.110586-blue)](https://doi.org/10.1016/j.celrep.2022.110586)
-        
-        
-        # Diameter synthesis
-        
-        This code aims at generating synthetic diameters for neurons, with parameters learned from a set of biological neurons.
-        
-        
-        ## Installation
-        
-        Use pip:
-        
-        ```bash
-        pip install diameter-synthesis
-        ```
-        
-        ## Main usage
-        
-        ### Step 1: Building models
-        
-        In folder `example`, you first have to modify `create_jsons.py` to suit your needs.
-        
-        You have the following important parameters for the dict `extract_models_params`:
-        
-        - `morph_path`: path to morphology files
-        - `mtypes_sort`: how to learn distributions: `all` to use all together, `mtypes` to use by mtypes , `super_mtypes` to use home made cells types (see `diameter_types` below)
-        - `models`: to create several models (for now they are all the same, just different realisation of random numbers)
-        - `neurite_types`: types of neurite to learn parameters for
-        - `extra_params`: dict of additional model parameters
-        
-        ### Step 2: Building diameters
-        
-        Then simply run `./run_models.sh` to create the models (saved in a json file).
-        
-        In `create_jsons.py`, the dict `generate_diameters_params` needs to be updated, too, with entries matching the previous dict.
-        The path in `new_morph_path` will be where the new morphologies will be saved.
-        
-        Then run `./run_diamters.sh` to generate diameters.
-        
-        
-        ## Additional scripts
-        
-        Several additional scripts in folder `scripts`:
-        
-        - `diameter-checks`: run the diameter-check code (bluepymm) on the biological and sampled cells
-        - `diameter_types`: cluster mtypes using distributions of surface areas (uses two privates repositories a the moment)
-        - `extract_morphometrics`: from bio and sample cells, extracts and plot distribution of surface area and diameter as a function of branch order and path lengths
-        - `extract_morphologies`: from a cell release, find the ones that can be run through diameter-check
-        - `plot_morphologies`: plot all morphologies in mtype folders
-        
-        
-        ## Examples
-        
-        The `examples` folder contains a simple example that will fetch morphologies from [neuromorpho.org](http://neuromorpho.org), learn a diameter model, rediametrize these morphologies, and perform some analysis of the results to compare original and diametrized morphologies.
-        This example can simply be run using the following command:
-        ```bash
-        ./run.sh
-        ```
-        
-        
-        ## Funding & Acknowledgment
-        
-        The development of this software was supported by funding to the Blue Brain Project, a research center of the École polytechnique fédérale de Lausanne (EPFL), from the Swiss government’s ETH Board of the Swiss Federal Institutes of Technology.
-        
-        For license and authors, see `LICENSE.txt` and `AUTHORS.md` respectively.
-        
-        Copyright © 2021-2022 Blue Brain Project/EPFL
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: plot
 Provides-Extra: test
+License-File: LICENSE.txt
+License-File: AUTHORS.md
+
+[![Version](https://img.shields.io/pypi/v/diameter-synthesis)](https://github.com/BlueBrain/diameter-synthesis/releases)
+[![Build status](https://github.com/BlueBrain/diameter-synthesis/actions/workflows/run-tox.yml/badge.svg?branch=main)](https://github.com/BlueBrain/diameter-synthesis/actions)
+[![Codecov.io](https://codecov.io/github/BlueBrain/diameter-synthesis/coverage.svg?branch=main)](https://codecov.io/github/BlueBrain/diameter-synthesis?branch=main)
+[![License](https://img.shields.io/badge/License-GPLv3-blue)](https://github.com/BlueBrain/diameter-synthesis/blob/main/LICENSE.txt)
+[![Documentation status](https://readthedocs.org/projects/diameter-synthesis/badge/?version=latest)](https://diameter-synthesis.readthedocs.io/)
+[![DOI](https://img.shields.io/badge/DOI-10.1016/j.celrep.2022.110586-blue)](https://doi.org/10.1016/j.celrep.2022.110586)
+
+
+# Diameter synthesis
+
+This code aims at generating synthetic diameters for neurons, with parameters learned from a set of biological neurons.
+
+
+## Installation
+
+Use pip:
+
+```bash
+pip install diameter-synthesis
+```
+
+## Main usage
+
+### Step 1: Building models
+
+In folder `example`, you first have to modify `create_jsons.py` to suit your needs.
+
+You have the following important parameters for the dict `extract_models_params`:
+
+- `morph_path`: path to morphology files
+- `mtypes_sort`: how to learn distributions: `all` to use all together, `mtypes` to use by mtypes , `super_mtypes` to use home made cells types (see `diameter_types` below)
+- `models`: to create several models (for now they are all the same, just different realisation of random numbers)
+- `neurite_types`: types of neurite to learn parameters for
+- `extra_params`: dict of additional model parameters
+
+### Step 2: Building diameters
+
+Then simply run `./run_models.sh` to create the models (saved in a json file).
+
+In `create_jsons.py`, the dict `generate_diameters_params` needs to be updated, too, with entries matching the previous dict.
+The path in `new_morph_path` will be where the new morphologies will be saved.
+
+Then run `./run_diamters.sh` to generate diameters.
+
+
+## Additional scripts
+
+Several additional scripts in folder `scripts`:
+
+- `diameter-checks`: run the diameter-check code (bluepymm) on the biological and sampled cells
+- `diameter_types`: cluster mtypes using distributions of surface areas (uses two privates repositories a the moment)
+- `extract_morphometrics`: from bio and sample cells, extracts and plot distribution of surface area and diameter as a function of branch order and path lengths
+- `extract_morphologies`: from a cell release, find the ones that can be run through diameter-check
+- `plot_morphologies`: plot all morphologies in mtype folders
+
+
+## Examples
+
+The `examples` folder contains a simple example that will fetch morphologies from [neuromorpho.org](http://neuromorpho.org), learn a diameter model, rediametrize these morphologies, and perform some analysis of the results to compare original and diametrized morphologies.
+This example can simply be run using the following command:
+```bash
+./run.sh
+```
+
+
+## Funding & Acknowledgment
+
+The development of this software was supported by funding to the Blue Brain Project, a research center of the École polytechnique fédérale de Lausanne (EPFL), from the Swiss government’s ETH Board of the Swiss Federal Institutes of Technology.
+
+For license and authors, see `LICENSE.txt` and `AUTHORS.md` respectively.
+
+Copyright © 2021-2022 Blue Brain Project/EPFL
```

### Comparing `diameter-synthesis-0.5.3/diameter_synthesis.egg-info/SOURCES.txt` & `diameter-synthesis-0.5.4/diameter_synthesis.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 .auto-changelog
 .auto-changelog-template.hbs
 .codespellignorelines
 .codespellrc
 .copier-answers.yml
 .coveragerc
 .flake8
+.gitattributes
 .gitignore
 .pre-commit-config.yaml
 .pylintrc
 .readthedocs.yml
 AUTHORS.md
 CHANGELOG.md
 CITATION.cff
@@ -18,14 +19,20 @@
 README.md
 codecov.yml
 commitlint.config.js
 package.json
 pyproject.toml
 setup.py
 tox.ini
+.github/dependabot.yml
+.github/pull_request_template.md
+.github/ISSUE_TEMPLATE/bug_report.yaml
+.github/ISSUE_TEMPLATE/config.yml
+.github/ISSUE_TEMPLATE/feature_request.yaml
+.github/ISSUE_TEMPLATE/how_to_use.yaml
 .github/workflows/commitlint.yml
 .github/workflows/publish-sdist.yml
 .github/workflows/run-tox.yml
 diameter_synthesis/__init__.py
 diameter_synthesis/build_diameters.py
 diameter_synthesis/build_models.py
 diameter_synthesis/cli.py
@@ -58,16 +65,16 @@
 examples/model_config.json
 examples/rediametrize_single_neuron.py
 examples/run.sh
 tests/__init__.py
 tests/conftest.py
 tests/test_build_diameters.py
 tests/test_build_models.py
+tests/test_cli.py
 tests/test_distribution_fitting.py
-tests/test_main_and_cli.py
 tests/test_morph_functions.py
 tests/test_plotting.py
 tests/test_simpler_diametrizer.py
 tests/test_validator.py
 tests/testing_tools.py
 tests/data/C030796A-P3.h5
 tests/data/C030796A-P3_diametrized.h5
```

### Comparing `diameter-synthesis-0.5.3/docs/Makefile` & `diameter-synthesis-0.5.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.3/docs/source/conf.py` & `diameter-synthesis-0.5.4/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from importlib import metadata
 
 # -- Project information -----------------------------------------------------
 
 project = "diameter-synthesis"
 
 # The short X.Y version
-version = metadata.version("diameter_synthesis")
+version = metadata.version("diameter-synthesis")
 
 # The full version, including alpha/beta/rc tags
 release = version
 
 
 # -- General configuration ---------------------------------------------------
 
@@ -60,15 +60,15 @@
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 # html_static_path = ['_static']
 
 html_theme_options = {
-    "metadata_distribution": project,
+    "metadata_distribution": "diameter-synthesis",
 }
 
 html_title = "Diameter Synthesis"
 
 # If true, links to the reST sources are added to the pages.
 html_show_sourcelink = False
```

### Comparing `diameter-synthesis-0.5.3/examples/get_morphologies.py` & `diameter-synthesis-0.5.4/examples/get_morphologies.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Fetch some barrel morphologies from neuromorpho.org
+"""Fetch some barrel morphologies from neuromorpho.org.
 
 Copyright (C) 2021  Blue Brain Project, EPFL
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
@@ -36,21 +36,22 @@
     ctx.set_ciphers("DEFAULT@SECLEVEL=1")
     req = Request(url)
     response = urlopen(req, context=ctx)  # pylint: disable=consider-using-with
     return response
 
 
 def get_swc_by_neuron_index(neuronIndex, folder="morphologies"):
-    """Download a neuron by index and store it into a SWC file
-    Keyword arguments:
-    neronIndex -- the neuron index in the database
+    """Download a neuron by index and store it into a SWC file.
+
+    Args:
+        neuronIndex: the neuron index in the database
+        folder: the output folder (must already exist)
 
     Adapted from https://github.com/NeuroBox3D/neuromorpho/blob/master/rest_wrapper/rest_wrapper.py
     """
-
     url = "%s/api/neuron/id/%i" % (NEUROMORPHO_URL, neuronIndex)
     response = get_url(url)
     neuron_name = json.loads(response.read().decode("utf-8"))["neuron_name"]
     url = "%s/neuron_info.jsp?neuron_name=%s" % (NEUROMORPHO_URL, neuron_name)
     html = get_url(url).read().decode("utf-8")
     p = re.compile(r"<a href=dableFiles/(.*)>Morphology File \(Standardized\)</a>", re.MULTILINE)
     m = re.findall(p, html)
```

### Comparing `diameter-synthesis-0.5.3/examples/rediametrize_single_neuron.py` & `diameter-synthesis-0.5.4/examples/rediametrize_single_neuron.py`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.3/examples/run.sh` & `diameter-synthesis-0.5.4/examples/run.sh`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.3/package.json` & `diameter-synthesis-0.5.4/package.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9903846153846154%*

 * *Differences: {"'auto-changelog'": "{'replaceText': {'(^[dD]eprecate: ?)': '', '(^[dD]eprecate\\\\((.*)\\\\): "*

 * *                     "?)': '\\\\($2\\\\)'}}"}*

```diff
@@ -5,14 +5,16 @@
             "([bB]reaking: ?)": "",
             "(^[bB]uild: ?)": "",
             "(^[bB]uild\\((.*)\\): ?)": "\\($2\\)",
             "(^[cC][iI]: ?)": "",
             "(^[cC][iI]\\((.*)\\): ?)": "\\($2\\)",
             "(^[cC]hore: ?)": "",
             "(^[cC]hore\\((.*)\\): ?)": "\\($2\\)",
+            "(^[dD]eprecate: ?)": "",
+            "(^[dD]eprecate\\((.*)\\): ?)": "\\($2\\)",
             "(^[dD]ocs: ?)": "",
             "(^[dD]ocs\\((.*)\\): ?)": "\\($2\\)",
             "(^[fF]eat: ?)": "",
             "(^[fF]eat\\((.*)\\): ?)": "\\($2\\)",
             "(^[fF]ix: ?)": "",
             "(^[fF]ix\\((.*)\\): ?)": "\\($2\\)",
             "(^[pP]erf: ?)": "",
```

### Comparing `diameter-synthesis-0.5.3/setup.py` & `diameter-synthesis-0.5.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,80 +13,84 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 from pathlib import Path
 
-from setuptools import find_packages
+from setuptools import find_namespace_packages
 from setuptools import setup
 
 reqs = [
     "click>=7.0",
     "jsonschema>=3",
-    "matplotlib>=2.2.0",
-    "morphio>=2.3.4",
+    "matplotlib>=3.4",
+    "morphio>=3.3.4",
     "neurom>=3.0,<4.0",
-    "numpy>=1.15.0",
-    "pandas>=0.24.0",
-    "scipy>=0.13.3",
+    "numpy>=1.22.0",
+    "pandas>=1.0.5",
+    "scipy>=1.6",
 ]
 
 doc_reqs = [
     "m2r2",
     "sphinx",
     "sphinx-bluebrain-theme",
     "sphinx-jsonschema",
     "sphinx_click",
 ]
 
 test_reqs = [
     "diff_pdf_visually>=1.7.0",
-    "decorator",
-    "matplotlib",
-    "mock",
-    "pytest",
-    "pytest-cov",
-    "pytest-html",
-    "pytest-xdist",
+    "decorator>=4",
+    "mock>=3",
+    "pytest>=6",
+    "pytest-click>=1",
+    "pytest-console-scripts>=1.3",
+    "pytest-cov>=3",
+    "pytest-html>=2",
+    "pytest-xdist>=2",
 ]
 
 setup(
     name="diameter-synthesis",
     author="Blue Brain Project, EPFL",
     description="Diametrize cells.",
     long_description=Path("README.md").read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     url="https://diameter-synthesis.readthedocs.io",
     project_urls={
         "Tracker": "https://github.com/BlueBrain/diameter-synthesis/issues",
         "Source": "https://github.com/BlueBrain/diameter-synthesis",
     },
     license="GNU General Public License v3.0",
-    packages=find_packages(exclude=["tests"]),
+    packages=find_namespace_packages(include=["diameter_synthesis*"]),
     python_requires=">=3.8",
     use_scm_version=True,
     setup_requires=[
         "setuptools_scm",
     ],
     install_requires=reqs,
     extras_require={
         "docs": doc_reqs,
         "plot": "seaborn>=0.11.1",
         "test": test_reqs,
     },
-    tests_require=test_reqs,
     entry_points={
-        "console_scripts": ["diameter-synthesis=diameter_synthesis.cli:cli"],
+        "console_scripts": [
+            "diameter-synthesis=diameter_synthesis.cli:main",
+        ],
     },
+    include_package_data=True,
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Scientific/Engineering :: Bio-Informatics",
     ],
-    include_package_data=True,
 )
```

### Comparing `diameter-synthesis-0.5.3/tests/__init__.py` & `diameter-synthesis-0.5.4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.3/tests/conftest.py` & `diameter-synthesis-0.5.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.3/tests/data/C030796A-P3.h5` & `diameter-synthesis-0.5.4/tests/data/C030796A-P3.h5`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.3/tests/data/C030796A-P3_diametrized.h5` & `diameter-synthesis-0.5.4/tests/data/C030796A-P3_diametrized.h5`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.3/tests/data/C030796A-P3_lite.h5` & `diameter-synthesis-0.5.4/tests/data/C030796A-P3_lite.h5`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.3/tests/data/C030796A-P3_lite_diametrized.h5` & `diameter-synthesis-0.5.4/tests/data/C030796A-P3_lite_diametrized.h5`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.3/tests/data/C030796A-P3_lite_diametrized_1_sample.h5` & `diameter-synthesis-0.5.4/tests/data/C030796A-P3_lite_diametrized_1_sample.h5`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.3/tests/data/C030796A-P3_lite_diametrized_astrocyte.h5` & `diameter-synthesis-0.5.4/tests/data/C030796A-P3_lite_diametrized_astrocyte.h5`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.3/tests/data/astro_model_data.json` & `diameter-synthesis-0.5.4/tests/data/astro_model_data.json`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.3/tests/data/astro_model_params.json` & `diameter-synthesis-0.5.4/tests/data/astro_model_params.json`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.3/tests/data/model_data.json` & `diameter-synthesis-0.5.4/tests/data/model_data.json`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.3/tests/data/model_params.json` & `diameter-synthesis-0.5.4/tests/data/model_params.json`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.3/tests/data/simpler_model_data.json` & `diameter-synthesis-0.5.4/tests/data/simpler_model_data.json`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.3/tests/data/simpler_morph_diametrized.asc` & `diameter-synthesis-0.5.4/tests/data/simpler_morph_diametrized.asc`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.3/tests/data/small_morph_apical_diametrized.asc` & `diameter-synthesis-0.5.4/tests/data/small_morph_apical_diametrized.asc`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.3/tests/data/small_morph_diametrized.asc` & `diameter-synthesis-0.5.4/tests/data/small_morph_diametrized.asc`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.3/tests/data/small_morph_several_apical_diametrized.asc` & `diameter-synthesis-0.5.4/tests/data/small_morph_several_apical_diametrized.asc`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.3/tests/expected_images/test_cumulative_analysis/analysis/L5_TPC_A_cumulative_section_path_distances_areas.pdf` & `diameter-synthesis-0.5.4/tests/expected_images/test_cumulative_analysis/analysis/L5_TPC_A_cumulative_section_path_distances_areas.pdf`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.3/tests/expected_images/test_cumulative_analysis/analysis/L5_TPC_A_cumulative_section_path_distances_areas_individual/0_L5_TPC_A_cumulative_section_path_distances_areas_C030796A-P3_lite.pdf` & `diameter-synthesis-0.5.4/tests/expected_images/test_cumulative_analysis/analysis/L5_TPC_A_cumulative_section_path_distances_areas_individual/0_L5_TPC_A_cumulative_section_path_distances_areas_C030796A-P3_lite.pdf`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.3/tests/expected_images/test_cumulative_analysis/analysis/L5_TPC_A_cumulative_section_path_distances_volumes.pdf` & `diameter-synthesis-0.5.4/tests/expected_images/test_cumulative_analysis/analysis/L5_TPC_A_cumulative_section_path_distances_volumes.pdf`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.3/tests/expected_images/test_cumulative_analysis/analysis/L5_TPC_A_cumulative_section_path_distances_volumes_individual/0_L5_TPC_A_cumulative_section_path_distances_volumes_C030796A-P3_lite.pdf` & `diameter-synthesis-0.5.4/tests/expected_images/test_cumulative_analysis/analysis/L5_TPC_A_cumulative_section_path_distances_volumes_individual/0_L5_TPC_A_cumulative_section_path_distances_volumes_C030796A-P3_lite.pdf`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.3/tests/expected_images/test_make_cumulative_figures/cumulative_segment_radial_distances_volumes.pdf` & `diameter-synthesis-0.5.4/tests/expected_images/test_make_cumulative_figures/cumulative_segment_radial_distances_volumes.pdf`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.3/tests/expected_images/test_make_cumulative_figures/cumulative_segment_radial_distances_volumes_individual/0_cumulative_segment_radial_distances_volumes.pdf` & `diameter-synthesis-0.5.4/tests/expected_images/test_make_cumulative_figures/cumulative_segment_radial_distances_volumes_individual/0_cumulative_segment_radial_distances_volumes.pdf`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.3/tests/expected_images/test_plot_cumulative_distribution.pdf` & `diameter-synthesis-0.5.4/tests/expected_images/test_plot_cumulative_distribution.pdf`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.3/tests/expected_images/test_plot_diameter_diff_div.pdf` & `diameter-synthesis-0.5.4/tests/expected_images/test_plot_diameter_diff_div.pdf`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.3/tests/expected_images/test_plot_diameter_diff_mult.pdf` & `diameter-synthesis-0.5.4/tests/expected_images/test_plot_diameter_diff_mult.pdf`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.3/tests/expected_images/test_plot_distribution_fit.pdf` & `diameter-synthesis-0.5.4/tests/expected_images/test_plot_distribution_fit.pdf`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.3/tests/expected_images/test_violin_analysis.pdf` & `diameter-synthesis-0.5.4/tests/expected_images/test_violin_analysis.pdf`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.3/tests/test_build_diameters.py` & `diameter-synthesis-0.5.4/tests/test_build_diameters.py`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.3/tests/test_build_models.py` & `diameter-synthesis-0.5.4/tests/test_build_models.py`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.3/tests/test_distribution_fitting.py` & `diameter-synthesis-0.5.4/tests/test_distribution_fitting.py`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.3/tests/test_main_and_cli.py` & `diameter-synthesis-0.5.4/tests/test_cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Test the cli module."""
+"""Tests for the diameter_synthesis.cli module."""
 
 # Copyright (C) 2021  Blue Brain Project, EPFL
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -24,14 +24,36 @@
 
 from diameter_synthesis import cli
 from diameter_synthesis import main
 
 from .testing_tools import compare_dicts
 
 
+def test_cli(cli_runner):
+    # pylint: disable=unused-argument
+    """Test the CLI."""
+    result = cli_runner.invoke(
+        cli.main,
+        [
+            "--version",
+        ],
+    )
+    assert result.exit_code == 0
+    assert result.output.startswith("diameter-synthesis, version ")
+
+
+@pytest.mark.parametrize("command", ["run_models", "run_diameters", "plot_diff", "run_analysis"])
+def test_entry_points(script_runner, command):
+    """Test the entry points."""
+    ret = script_runner.run("diameter-synthesis", command)
+    assert not ret.success
+    assert f"Usage: diameter-synthesis {command}" in ret.stderr
+    assert ret.stdout == ""
+
+
 def test_run_models(tmpdir, single_pop_data_dir, single_pop_diametrized_data_dir, config):
     """Test the run_models entry point."""
     # Prepare inputs
     extract_models_params = config
     extract_models_params["mtypes_file"] = str(single_pop_data_dir / "neurondb.dat")
     extract_models_params["morph_path"] = str(single_pop_data_dir)
     extract_models_params["new_morph_path"] = str(single_pop_diametrized_data_dir)
@@ -42,15 +64,15 @@
 
     config_file = str(tmpdir / "diametrizer_params.json")
     with open(config_file, "w", encoding="utf-8") as json_file:
         json.dump(extract_models_params, json_file, sort_keys=True, indent=4)
 
     # Run with CLI
     runner = CliRunner()
-    runner.invoke(cli.cli, ["run_models", config_file], catch_exceptions=False)
+    runner.invoke(cli.main, ["run_models", config_file], catch_exceptions=False)
 
     # Check results
     with open(extract_models_params["models_params_file"], "r", encoding="utf-8") as json_file:
         res = json.load(json_file)
 
     assert list(res.keys()) == ["generic"]
     assert list(res["generic"].keys()) == ["L5_TPC:A"]
@@ -107,15 +129,15 @@
     model_params_file = str(tmpdir / "model_params.json")
     with open(model_params_file, "w", encoding="utf-8") as json_file:
         json.dump({"generic": {"L5_TPC:A": model_params}}, json_file, sort_keys=True, indent=4)
 
     # Run with CLI
     runner = CliRunner()
     runner.invoke(
-        cli.cli, ["run_diameters", config_file, model_params_file], catch_exceptions=False
+        cli.main, ["run_diameters", config_file, model_params_file], catch_exceptions=False
     )
 
     # Check results
     assert [i.name for i in res_path.iterdir()] == ["C030796A-P3_lite.h5"]
 
 
 def test_run_diametrize_single_neuron(neuron):
@@ -135,15 +157,15 @@
 def test_plot_diff(tmpdir, single_pop_data_dir, single_pop_diametrized_data_dir):
     """Test the plot_diff entry point."""
     res_path = Path(tmpdir / "figures")
 
     # Run with CLI
     runner = CliRunner()
     runner.invoke(
-        cli.cli,
+        cli.main,
         [
             "plot_diff",
             "--orig-path",
             str(single_pop_data_dir),
             "--diam-path",
             str(single_pop_diametrized_data_dir),
             "--out-dir",
@@ -161,15 +183,15 @@
 def test_run_analysis(tmpdir, single_pop_data_dir, single_pop_diametrized_data_dir):
     """Test the run_analysis entry point."""
     res_path = Path(tmpdir / "figures")
 
     # Run with CLI
     runner = CliRunner()
     runner.invoke(
-        cli.cli,
+        cli.main,
         [
             "run_analysis",
             "--orig-path",
             str(single_pop_data_dir),
             "--diam-path",
             str(single_pop_diametrized_data_dir),
             "--mtypes-file",
@@ -199,15 +221,15 @@
         "basal_dendrite/L5_TPC_A_cumulative_section_path_distances_areas_individual",
         "basal_dendrite/L5_TPC_A_cumulative_section_path_distances_volumes_individual",
     ]
 
     # Test with neither cumukative nor violin
     with pytest.raises(ValueError):
         runner.invoke(
-            cli.cli,
+            cli.main,
             [
                 "run_analysis",
                 "--orig-path",
                 str(single_pop_data_dir),
                 "--diam-path",
                 str(single_pop_diametrized_data_dir),
                 "--mtypes-file",
```

### Comparing `diameter-synthesis-0.5.3/tests/test_morph_functions.py` & `diameter-synthesis-0.5.4/tests/test_morph_functions.py`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.3/tests/test_plotting.py` & `diameter-synthesis-0.5.4/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.3/tests/test_validator.py` & `diameter-synthesis-0.5.4/tests/test_validator.py`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.3/tests/testing_tools.py` & `diameter-synthesis-0.5.4/tests/testing_tools.py`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.3/tox.ini` & `diameter-synthesis-0.5.4/tox.ini`

 * *Files 17% similar despite different names*

```diff
@@ -3,58 +3,68 @@
 files = {[base]name} tests docs/source/conf.py setup.py
 
 [tox]
 envlist =
     check-packaging
     lint
     docs
-    py{38,39}
+    min_versions
+    py{38,39,310,311}
     coverage
 
 minversion = 3.18
 
 [testenv]
 setenv =
     COVERAGE_FILE = {env:COVERAGE_FILE:.coverage-{envname}}
 extras =
     plot
     test
-commands = pytest \
-    -n {env:PYTEST_NPROCS:'auto'} \
-    --basetemp={envtmpdir} \
-    --cov={[base]name} \
-    --cov-branch \
-    --cov-fail-under=84 \
-    --no-cov-on-fail \
-    --cov-report term-missing \
-    --cov-report html:reports/coverage-{envname} \
-    --cov-report xml:reports/coverage-{envname}.xml \
-    --html reports/pytest-{envname}.html \
-    --junit-xml=reports/pytest-{envname}.xml \
-    --self-contained-html \
-    {posargs}
+deps =
+    min_versions: Requirements-Builder
+commands =
+    min_versions: requirements-builder --level=min --extras=test -o {envtmpdir}/requirements_min.txt setup.py
+    min_versions: pip install -r {envtmpdir}/requirements_min.txt
+    min_versions: pip freeze
+    pytest \
+        -n {env:PYTEST_NPROCS:'auto'} \
+        --basetemp={envtmpdir} \
+        --cov={[base]name} \
+        --cov-branch \
+        --cov-fail-under=80 \
+        --no-cov-on-fail \
+        --cov-report term-missing \
+        --cov-report html:reports/coverage-{envname} \
+        --cov-report xml:reports/coverage-{envname}.xml \
+        --html reports/pytest-{envname}.html \
+        --junit-xml=reports/pytest-{envname}.xml \
+        --self-contained-html \
+        {posargs}
 
 [testenv:coverage]
 skip_install = true
 deps = coverage
 allowlist_externals = /bin/bash
 commands =
     /bin/bash -c 'coverage combine .coverage-py*'
     coverage xml
     coverage report
 
 [testenv:check-packaging]
 skip_install = true
 deps =
-    wheel
+    build
     twine
 commands =
-    python setup.py sdist bdist_wheel -d {envtmpdir}/dist
+    python -m build -o {envtmpdir}/dist
     twine check {envtmpdir}/dist/*
 
+[testenv:min_versions]
+basepython = python3.8
+
 [testenv:lint]
 basepython = python3.8
 deps =
     pre-commit
     pylint
 commands =
     pre-commit run --all-files --show-diff-on-failure
@@ -63,21 +73,24 @@
 [testenv:format]
 basepython = python3.8
 skip_install = true
 deps =
     codespell
     pre-commit
 commands =
-    codespell -i 2 -x .codespellignorelines -w {[base]files} README.md CHANGELOG.md
+    codespell -i 3 -x .codespellignorelines -w {[base]files} README.md CHANGELOG.md docs/source
     pre-commit run --all-files
 
 [testenv:docs]
 changedir = docs
 extras = docs
-allowlist_externals = make
+allowlist_externals =
+    make
 # set warnings as errors using the -W sphinx option
 commands = make html SPHINXOPTS=-W
 
 [gh-actions]
 python =
-  3.8: py38, check-packaging, lint
-  3.9: py39, docs, coverage
+  3.8: py38, lint
+  3.9: py39, docs
+  3.10: py310, check-packaging
+  3.11: py311
```

