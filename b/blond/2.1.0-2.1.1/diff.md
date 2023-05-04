# Comparing `tmp/blond-2.1.0.tar.gz` & `tmp/blond-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blond-2.1.0.tar", last modified: Wed May  3 17:00:33 2023, max compression
+gzip compressed data, was "blond-2.1.1.tar", last modified: Thu May  4 09:50:52 2023, max compression
```

## Comparing `blond-2.1.0.tar` & `blond-2.1.1.tar`

### file list

```diff
@@ -1,312 +1,312 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:00:33.432000 blond-2.1.0/
--rw-r--r--   0 root         (0) root         (0)      399 2023-05-03 16:59:58.000000 blond-2.1.0/.coveragerc
--rw-r--r--   0 root         (0) root         (0)     6226 2023-05-03 16:59:58.000000 blond-2.1.0/.gitignore
--rw-r--r--   0 root         (0) root         (0)     2869 2023-05-03 16:59:58.000000 blond-2.1.0/.gitlab-ci.yml
--rw-r--r--   0 root         (0) root         (0)     1665 2023-05-03 16:59:58.000000 blond-2.1.0/CHANGELOG
--rw-r--r--   0 root         (0) root         (0)    35797 2023-05-03 16:59:58.000000 blond-2.1.0/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      339 2023-05-03 16:59:58.000000 blond-2.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    13244 2023-05-03 17:00:33.432000 blond-2.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12468 2023-05-03 16:59:58.000000 blond-2.1.0/README.md
--rw-r--r--   0 root         (0) root         (0)      794 2023-05-03 16:59:58.000000 blond-2.1.0/WARNINGS.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:00:33.376000 blond-2.1.0/__BENCHMARKS/
--rw-r--r--   0 root         (0) root         (0)       55 2023-05-03 16:59:58.000000 blond-2.1.0/__BENCHMARKS/.gitignore
--rw-r--r--   0 root         (0) root         (0)    16964 2023-05-03 16:59:58.000000 blond-2.1.0/__BENCHMARKS/BM1_OTFB_Vind_beam_1.py
--rw-r--r--   0 root         (0) root         (0)     4291 2023-05-03 16:59:58.000000 blond-2.1.0/__BENCHMARKS/BM2_OTFB_no_beam.py
--rw-r--r--   0 root         (0) root         (0)     1270 2023-05-03 16:59:58.000000 blond-2.1.0/__BENCHMARKS/BM3_OTFB_moving_average.py
--rw-r--r--   0 root         (0) root         (0)     7415 2023-05-03 16:59:58.000000 blond-2.1.0/__BENCHMARKS/BM4_OTFB_with_beam.py
--rw-r--r--   0 root         (0) root         (0)     8956 2023-05-03 16:59:58.000000 blond-2.1.0/__BENCHMARKS/BM5_OTFB_feedforward.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:00:33.368000 blond-2.1.0/__EXAMPLES/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:00:33.380000 blond-2.1.0/__EXAMPLES/gpu_main_files/
--rw-r--r--   0 root         (0) root         (0)     5807 2023-05-03 16:59:58.000000 blond-2.1.0/__EXAMPLES/gpu_main_files/EX_01_Acceleration.py
--rw-r--r--   0 root         (0) root         (0)     8578 2023-05-03 16:59:58.000000 blond-2.1.0/__EXAMPLES/gpu_main_files/EX_02_Main_long_ps_booster.py
--rw-r--r--   0 root         (0) root         (0)     6581 2023-05-03 16:59:58.000000 blond-2.1.0/__EXAMPLES/gpu_main_files/EX_03_RFnoise.py
--rw-r--r--   0 root         (0) root         (0)     7056 2023-05-03 16:59:58.000000 blond-2.1.0/__EXAMPLES/gpu_main_files/EX_04_Stationary_multistation.py
--rw-r--r--   0 root         (0) root         (0)    14174 2023-05-03 16:59:58.000000 blond-2.1.0/__EXAMPLES/gpu_main_files/EX_05_Wake_impedance.py
--rw-r--r--   0 root         (0) root         (0)     7328 2023-05-03 16:59:58.000000 blond-2.1.0/__EXAMPLES/gpu_main_files/EX_07_Ions.py
--rw-r--r--   0 root         (0) root         (0)     5041 2023-05-03 16:59:58.000000 blond-2.1.0/__EXAMPLES/gpu_main_files/EX_08_Phase_Loop.py
--rw-r--r--   0 root         (0) root         (0)     5582 2023-05-03 16:59:58.000000 blond-2.1.0/__EXAMPLES/gpu_main_files/EX_09_Radial_Loop.py
--rw-r--r--   0 root         (0) root         (0)     5941 2023-05-03 16:59:58.000000 blond-2.1.0/__EXAMPLES/gpu_main_files/EX_10_Fixed_frequency.py
--rw-r--r--   0 root         (0) root         (0)     5953 2023-05-03 16:59:58.000000 blond-2.1.0/__EXAMPLES/gpu_main_files/EX_16_impedance_test.py
--rw-r--r--   0 root         (0) root         (0)     9212 2023-05-03 16:59:58.000000 blond-2.1.0/__EXAMPLES/gpu_main_files/EX_17_multi_turn_wake.py
--rw-r--r--   0 root         (0) root         (0)     8115 2023-05-03 16:59:58.000000 blond-2.1.0/__EXAMPLES/gpu_main_files/EX_18_robinson_instability.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:00:33.380000 blond-2.1.0/__EXAMPLES/input_files/
--rw-r--r--   0 root         (0) root         (0)    11866 2023-05-03 16:59:58.000000 blond-2.1.0/__EXAMPLES/input_files/EX_02_Ekicker_1.4GeV.txt
--rw-r--r--   0 root         (0) root         (0)    16868 2023-05-03 16:59:58.000000 blond-2.1.0/__EXAMPLES/input_files/EX_02_Finemet.txt
--rw-r--r--   0 root         (0) root         (0)     1043 2023-05-03 16:59:58.000000 blond-2.1.0/__EXAMPLES/input_files/EX_05_new_HQ_table.dat
--rw-r--r--   0 root         (0) root         (0)    11976 2023-05-03 16:59:58.000000 blond-2.1.0/__EXAMPLES/input_files/EX_06_Source_TOF_P.csv
--rw-r--r--   0 root         (0) root         (0)      170 2023-05-03 16:59:58.000000 blond-2.1.0/__EXAMPLES/input_files/EX_06_voltage_program_LHC25_c02.txt
--rw-r--r--   0 root         (0) root         (0)      316 2023-05-03 16:59:58.000000 blond-2.1.0/__EXAMPLES/input_files/EX_06_voltage_program_LHC25_c04.txt
--rw-r--r--   0 root         (0) root         (0)      101 2023-05-03 16:59:58.000000 blond-2.1.0/__EXAMPLES/input_files/EX_06_voltage_program_LHC25_c16.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:00:33.384000 blond-2.1.0/__EXAMPLES/main_files/
--rw-r--r--   0 root         (0) root         (0)     4668 2023-05-03 16:59:58.000000 blond-2.1.0/__EXAMPLES/main_files/EX_01_Acceleration.py
--rw-r--r--   0 root         (0) root         (0)     7353 2023-05-03 16:59:58.000000 blond-2.1.0/__EXAMPLES/main_files/EX_02_Main_long_ps_booster.py
--rw-r--r--   0 root         (0) root         (0)     5605 2023-05-03 16:59:58.000000 blond-2.1.0/__EXAMPLES/main_files/EX_03_RFnoise.py
--rw-r--r--   0 root         (0) root         (0)     5413 2023-05-03 16:59:58.000000 blond-2.1.0/__EXAMPLES/main_files/EX_04_Stationary_multistation.py
--rw-r--r--   0 root         (0) root         (0)    11556 2023-05-03 16:59:58.000000 blond-2.1.0/__EXAMPLES/main_files/EX_05_Wake_impedance.py
--rw-r--r--   0 root         (0) root         (0)     3396 2023-05-03 16:59:58.000000 blond-2.1.0/__EXAMPLES/main_files/EX_06_Preprocess.py
--rw-r--r--   0 root         (0) root         (0)     6400 2023-05-03 16:59:58.000000 blond-2.1.0/__EXAMPLES/main_files/EX_07_Ions.py
--rw-r--r--   0 root         (0) root         (0)     4348 2023-05-03 16:59:58.000000 blond-2.1.0/__EXAMPLES/main_files/EX_08_Phase_Loop.py
--rw-r--r--   0 root         (0) root         (0)     4864 2023-05-03 16:59:58.000000 blond-2.1.0/__EXAMPLES/main_files/EX_09_Radial_Loop.py
--rw-r--r--   0 root         (0) root         (0)     4938 2023-05-03 16:59:58.000000 blond-2.1.0/__EXAMPLES/main_files/EX_10_Fixed_frequency.py
--rw-r--r--   0 root         (0) root         (0)     4651 2023-05-03 16:59:58.000000 blond-2.1.0/__EXAMPLES/main_files/EX_11_comparison_music_fourier_analytical.py
--rw-r--r--   0 root         (0) root         (0)    11630 2023-05-03 16:59:58.000000 blond-2.1.0/__EXAMPLES/main_files/EX_12_synchrotron_frequency_distribution.py
--rw-r--r--   0 root         (0) root         (0)    10276 2023-05-03 16:59:58.000000 blond-2.1.0/__EXAMPLES/main_files/EX_13_synchrotron_radiation.py
--rw-r--r--   0 root         (0) root         (0)     4639 2023-05-03 16:59:58.000000 blond-2.1.0/__EXAMPLES/main_files/EX_14_sparse_slicing.py
--rw-r--r--   0 root         (0) root         (0)     4665 2023-05-03 16:59:58.000000 blond-2.1.0/__EXAMPLES/main_files/EX_15_sparse_multi_bunch.py
--rw-r--r--   0 root         (0) root         (0)     5447 2023-05-03 16:59:58.000000 blond-2.1.0/__EXAMPLES/main_files/EX_16_impedance_test.py
--rw-r--r--   0 root         (0) root         (0)     7736 2023-05-03 16:59:58.000000 blond-2.1.0/__EXAMPLES/main_files/EX_17_multi_turn_wake.py
--rw-r--r--   0 root         (0) root         (0)     7438 2023-05-03 16:59:58.000000 blond-2.1.0/__EXAMPLES/main_files/EX_18_robinson_instability.py
--rw-r--r--   0 root         (0) root         (0)     6098 2023-05-03 16:59:58.000000 blond-2.1.0/__EXAMPLES/main_files/EX_19_bunch_generation.py
--rw-r--r--   0 root         (0) root         (0)     6646 2023-05-03 16:59:58.000000 blond-2.1.0/__EXAMPLES/main_files/EX_20_bunch_generation_multibunch.py
--rw-r--r--   0 root         (0) root         (0)     3132 2023-05-03 16:59:58.000000 blond-2.1.0/__EXAMPLES/main_files/EX_21_bunch_distribution.py
--rwxr-xr-x   0 root         (0) root         (0)     4029 2023-05-03 16:59:58.000000 blond-2.1.0/__EXAMPLES/main_files/EX_22_Coherent_Radiation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:00:33.388000 blond-2.1.0/__EXAMPLES/mpi_main_files/
--rw-r--r--   0 root         (0) root         (0)     5008 2023-05-03 16:59:58.000000 blond-2.1.0/__EXAMPLES/mpi_main_files/EX_01_Acceleration.py
--rw-r--r--   0 root         (0) root         (0)     7618 2023-05-03 16:59:58.000000 blond-2.1.0/__EXAMPLES/mpi_main_files/EX_02_Main_long_ps_booster.py
--rw-r--r--   0 root         (0) root         (0)     5932 2023-05-03 16:59:58.000000 blond-2.1.0/__EXAMPLES/mpi_main_files/EX_03_RFnoise.py
--rw-r--r--   0 root         (0) root         (0)     5703 2023-05-03 16:59:58.000000 blond-2.1.0/__EXAMPLES/mpi_main_files/EX_04_Stationary_multistation.py
--rw-r--r--   0 root         (0) root         (0)    12098 2023-05-03 16:59:58.000000 blond-2.1.0/__EXAMPLES/mpi_main_files/EX_05_Wake_impedance.py
--rw-r--r--   0 root         (0) root         (0)     6688 2023-05-03 16:59:58.000000 blond-2.1.0/__EXAMPLES/mpi_main_files/EX_07_Ions.py
--rw-r--r--   0 root         (0) root         (0)     4632 2023-05-03 16:59:58.000000 blond-2.1.0/__EXAMPLES/mpi_main_files/EX_08_Phase_Loop.py
--rw-r--r--   0 root         (0) root         (0)     5181 2023-05-03 16:59:58.000000 blond-2.1.0/__EXAMPLES/mpi_main_files/EX_09_Radial_Loop.py
--rw-r--r--   0 root         (0) root         (0)     5255 2023-05-03 16:59:58.000000 blond-2.1.0/__EXAMPLES/mpi_main_files/EX_10_Fixed_frequency.py
--rw-r--r--   0 root         (0) root         (0)     5659 2023-05-03 16:59:58.000000 blond-2.1.0/__EXAMPLES/mpi_main_files/EX_16_impedance_test.py
--rw-r--r--   0 root         (0) root         (0)     7914 2023-05-03 16:59:58.000000 blond-2.1.0/__EXAMPLES/mpi_main_files/EX_18_robinson_instability.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:00:33.388000 blond-2.1.0/__doc/
--rw-r--r--   0 root         (0) root         (0)      603 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/Makefile
--rw-r--r--   0 root         (0) root         (0)     5664 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/conf.py
--rw-r--r--   0 root         (0) root         (0)     1162 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/index.rst
--rw-r--r--   0 root         (0) root         (0)      809 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:00:33.396000 blond-2.1.0/__doc/modules/
--rwxr-xr-x   0 root         (0) root         (0)   135010 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/modules/ACS_cavity_loop.png
--rwxr-xr-x   0 root         (0) root         (0)   185223 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/modules/ACS_cavity_loop.svg
--rwxr-xr-x   0 root         (0) root         (0)     1144 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/modules/RF_noise.gle
--rwxr-xr-x   0 root         (0) root         (0)    81234 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/modules/RF_noise.png
--rwxr-xr-x   0 root         (0) root         (0)   176302 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/modules/SPS_OTFB.png
--rwxr-xr-x   0 root         (0) root         (0)   655573 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/modules/SPS_OTFB.svg
--rw-r--r--   0 root         (0) root         (0)     1002 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/modules/beam.rst
--rw-r--r--   0 root         (0) root         (0)      177 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/modules/compile.rst
--rw-r--r--   0 root         (0) root         (0)    51317 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/modules/csr_impedance_real.png
--rw-r--r--   0 root         (0) root         (0)    19684 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/modules/equations_of_motion.rst
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/modules/impedances.rst
--rw-r--r--   0 root         (0) root         (0)      754 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/modules/input_parameters.rst
--rwxr-xr-x   0 root         (0) root         (0)     7100 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/modules/lhc_cavity_loop.rst
--rw-r--r--   0 root         (0) root         (0)    20259 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/modules/llrf.rst
--rw-r--r--   0 root         (0) root         (0)      191 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/modules/monitors.rst
--rw-r--r--   0 root         (0) root         (0)      977 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/modules/plots.rst
--rwxr-xr-x   0 root         (0) root         (0)     1050 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/modules/ring_and_RFstation.gle
--rwxr-xr-x   0 root         (0) root         (0)    84423 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/modules/ring_and_RFstation.png
--rwxr-xr-x   0 root         (0) root         (0)       39 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/modules/sample.dat
--rwxr-xr-x   0 root         (0) root         (0)       77 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/modules/sample2.dat
--rwxr-xr-x   0 root         (0) root         (0)    14087 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/modules/sps_cavity_loop.rst
--rw-r--r--   0 root         (0) root         (0)      269 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/modules/synchrotron_radiation.rst
--rw-r--r--   0 root         (0) root         (0)     1166 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/modules/toolbox.rst
--rw-r--r--   0 root         (0) root         (0)      344 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/modules/trackers.rst
--rw-r--r--   0 root         (0) root         (0)      484 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/modules/utils.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:00:33.368000 blond-2.1.0/__doc/themes/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:00:33.396000 blond-2.1.0/__doc/themes/sphinx_rtd_theme/
--rw-r--r--   0 root         (0) root         (0)      324 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/themes/sphinx_rtd_theme/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3740 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/themes/sphinx_rtd_theme/breadcrumbs.html
--rw-r--r--   0 root         (0) root         (0)     1978 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/themes/sphinx_rtd_theme/footer.html
--rw-r--r--   0 root         (0) root         (0)     7063 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/themes/sphinx_rtd_theme/layout.html
--rw-r--r--   0 root         (0) root         (0)     7526 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/themes/sphinx_rtd_theme/layout_old.html
--rw-r--r--   0 root         (0) root         (0)     1530 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/themes/sphinx_rtd_theme/search.html
--rw-r--r--   0 root         (0) root         (0)      365 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/themes/sphinx_rtd_theme/searchbox.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:00:33.372000 blond-2.1.0/__doc/themes/sphinx_rtd_theme/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:00:33.396000 blond-2.1.0/__doc/themes/sphinx_rtd_theme/static/css/
--rw-r--r--   0 root         (0) root         (0)     3381 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/themes/sphinx_rtd_theme/static/css/badge_only.css
--rw-r--r--   0 root         (0) root         (0)     3153 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/themes/sphinx_rtd_theme/static/css/badge_only.css.map
--rw-r--r--   0 root         (0) root         (0)   114281 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/themes/sphinx_rtd_theme/static/css/theme.css
--rw-r--r--   0 root         (0) root         (0)    67610 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/themes/sphinx_rtd_theme/static/css/theme.css.map
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:00:33.404000 blond-2.1.0/__doc/themes/sphinx_rtd_theme/static/fonts/
--rw-r--r--   0 root         (0) root         (0)   124988 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/themes/sphinx_rtd_theme/static/fonts/FontAwesome.otf
--rw-r--r--   0 root         (0) root         (0)   109948 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/themes/sphinx_rtd_theme/static/fonts/Inconsolata-Bold.ttf
--rw-r--r--   0 root         (0) root         (0)    96964 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/themes/sphinx_rtd_theme/static/fonts/Inconsolata-Regular.ttf
--rw-r--r--   0 root         (0) root         (0)   656544 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/themes/sphinx_rtd_theme/static/fonts/Lato-Bold.ttf
--rw-r--r--   0 root         (0) root         (0)   656568 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/themes/sphinx_rtd_theme/static/fonts/Lato-Regular.ttf
--rw-r--r--   0 root         (0) root         (0)   170616 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/themes/sphinx_rtd_theme/static/fonts/RobotoSlab-Bold.ttf
--rw-r--r--   0 root         (0) root         (0)   169064 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/themes/sphinx_rtd_theme/static/fonts/RobotoSlab-Regular.ttf
--rw-r--r--   0 root         (0) root         (0)    76518 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.eot
--rw-r--r--   0 root         (0) root         (0)   391622 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.svg
--rw-r--r--   0 root         (0) root         (0)   152796 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 root         (0) root         (0)    90412 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.woff
--rw-r--r--   0 root         (0) root         (0)    71896 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.woff2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:00:33.404000 blond-2.1.0/__doc/themes/sphinx_rtd_theme/static/js/
--rw-r--r--   0 root         (0) root         (0)     2457 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/themes/sphinx_rtd_theme/static/js/copybutton.js
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/themes/sphinx_rtd_theme/static/js/copybutton.js~
--rw-r--r--   0 root         (0) root         (0)    15414 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/themes/sphinx_rtd_theme/static/js/modernizr.min.js
--rw-r--r--   0 root         (0) root         (0)     6477 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/themes/sphinx_rtd_theme/static/js/theme.js
--rw-r--r--   0 root         (0) root         (0)      260 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/themes/sphinx_rtd_theme/theme.conf
--rw-r--r--   0 root         (0) root         (0)     1299 2023-05-03 16:59:58.000000 blond-2.1.0/__doc/themes/sphinx_rtd_theme/versions.html
--rw-r--r--   0 root         (0) root         (0)     1380 2023-05-03 16:59:58.000000 blond-2.1.0/appveyor.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:00:33.404000 blond-2.1.0/blond/
--rw-r--r--   0 root         (0) root         (0)     1199 2023-05-03 16:59:58.000000 blond-2.1.0/blond/__init__.py
--rw-r--r--   0 root         (0) root         (0)      160 2023-05-03 17:00:28.000000 blond-2.1.0/blond/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:00:33.408000 blond-2.1.0/blond/beam/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 16:59:58.000000 blond-2.1.0/blond/beam/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20461 2023-05-03 16:59:58.000000 blond-2.1.0/blond/beam/beam.py
--rw-r--r--   0 root         (0) root         (0)     3685 2023-05-03 16:59:58.000000 blond-2.1.0/blond/beam/coasting_beam.py
--rw-r--r--   0 root         (0) root         (0)    41527 2023-05-03 16:59:58.000000 blond-2.1.0/blond/beam/distributions.py
--rw-r--r--   0 root         (0) root         (0)    39107 2023-05-03 16:59:58.000000 blond-2.1.0/blond/beam/distributions_multibunch.py
--rw-r--r--   0 root         (0) root         (0)    24385 2023-05-03 16:59:58.000000 blond-2.1.0/blond/beam/profile.py
--rw-r--r--   0 root         (0) root         (0)     5740 2023-05-03 16:59:58.000000 blond-2.1.0/blond/beam/sparse_histogram.cpp
--rw-r--r--   0 root         (0) root         (0)     4804 2023-05-03 16:59:58.000000 blond-2.1.0/blond/beam/sparse_slices.py
--rw-r--r--   0 root         (0) root         (0)    11638 2023-05-03 16:59:58.000000 blond-2.1.0/blond/compile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:00:33.412000 blond-2.1.0/blond/cpp_routines/
--rw-r--r--   0 root         (0) root         (0)     3088 2023-05-03 16:59:58.000000 blond-2.1.0/blond/cpp_routines/beam_phase.cpp
--rw-r--r--   0 root         (0) root         (0)    29022 2023-05-03 16:59:58.000000 blond-2.1.0/blond/cpp_routines/blondmath.cpp
--rw-r--r--   0 root         (0) root         (0)    13334 2023-05-03 16:59:58.000000 blond-2.1.0/blond/cpp_routines/blondmath.h
--rw-r--r--   0 root         (0) root         (0)     1316 2023-05-03 16:59:58.000000 blond-2.1.0/blond/cpp_routines/cos.h
--rw-r--r--   0 root         (0) root         (0)     5747 2023-05-03 16:59:58.000000 blond-2.1.0/blond/cpp_routines/drift.cpp
--rw-r--r--   0 root         (0) root         (0)     4376 2023-05-03 16:59:58.000000 blond-2.1.0/blond/cpp_routines/exp.h
--rw-r--r--   0 root         (0) root         (0)     4661 2023-05-03 16:59:58.000000 blond-2.1.0/blond/cpp_routines/fast_resonator.cpp
--rw-r--r--   0 root         (0) root         (0)    29481 2023-05-03 16:59:58.000000 blond-2.1.0/blond/cpp_routines/fft.cpp
--rw-r--r--   0 root         (0) root         (0)     4419 2023-05-03 16:59:58.000000 blond-2.1.0/blond/cpp_routines/fft.h
--rw-r--r--   0 root         (0) root         (0)    10013 2023-05-03 16:59:58.000000 blond-2.1.0/blond/cpp_routines/histogram.cpp
--rw-r--r--   0 root         (0) root         (0)     3493 2023-05-03 16:59:58.000000 blond-2.1.0/blond/cpp_routines/kick.cpp
--rwxr-xr-x   0 root         (0) root         (0)   126096 2023-05-03 17:00:33.000000 blond-2.1.0/blond/cpp_routines/libblond.so
--rw-r--r--   0 root         (0) root         (0)     6406 2023-05-03 16:59:58.000000 blond-2.1.0/blond/cpp_routines/linear_interp_kick.cpp
--rw-r--r--   0 root         (0) root         (0)    15181 2023-05-03 16:59:58.000000 blond-2.1.0/blond/cpp_routines/music_track.cpp
--rw-r--r--   0 root         (0) root         (0)      169 2023-05-03 16:59:58.000000 blond-2.1.0/blond/cpp_routines/openmp.cpp
--rw-r--r--   0 root         (0) root         (0)      245 2023-05-03 16:59:58.000000 blond-2.1.0/blond/cpp_routines/openmp.h
--rw-r--r--   0 root         (0) root         (0)     1960 2023-05-03 16:59:58.000000 blond-2.1.0/blond/cpp_routines/sin.h
--rw-r--r--   0 root         (0) root         (0)     5871 2023-05-03 16:59:58.000000 blond-2.1.0/blond/cpp_routines/sincos.h
--rw-r--r--   0 root         (0) root         (0)     7480 2023-05-03 16:59:58.000000 blond-2.1.0/blond/cpp_routines/vdtcore_common.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:00:33.412000 blond-2.1.0/blond/gpu/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 16:59:58.000000 blond-2.1.0/blond/gpu/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:00:33.412000 blond-2.1.0/blond/gpu/cuda_kernels/
--rw-r--r--   0 root         (0) root         (0)    14390 2023-05-03 16:59:58.000000 blond-2.1.0/blond/gpu/cuda_kernels/kernels_double.cu
--rw-r--r--   0 root         (0) root         (0)    14135 2023-05-03 16:59:58.000000 blond-2.1.0/blond/gpu/cuda_kernels/kernels_single.cu
--rw-r--r--   0 root         (0) root         (0)    10769 2023-05-03 16:59:58.000000 blond-2.1.0/blond/gpu/cupy_butils_wrap.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:00:33.412000 blond-2.1.0/blond/impedances/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 16:59:58.000000 blond-2.1.0/blond/impedances/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39560 2023-05-03 16:59:58.000000 blond-2.1.0/blond/impedances/impedance.py
--rw-r--r--   0 root         (0) root         (0)    45892 2023-05-03 16:59:58.000000 blond-2.1.0/blond/impedances/impedance_sources.py
--rw-r--r--   0 root         (0) root         (0)     3541 2023-05-03 16:59:58.000000 blond-2.1.0/blond/impedances/induced_voltage_analytical.py
--rw-r--r--   0 root         (0) root         (0)    12228 2023-05-03 16:59:58.000000 blond-2.1.0/blond/impedances/music.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:00:33.412000 blond-2.1.0/blond/input_parameters/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 16:59:58.000000 blond-2.1.0/blond/input_parameters/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24903 2023-05-03 16:59:58.000000 blond-2.1.0/blond/input_parameters/rf_parameters.py
--rw-r--r--   0 root         (0) root         (0)    20249 2023-05-03 16:59:58.000000 blond-2.1.0/blond/input_parameters/rf_parameters_options.py
--rw-r--r--   0 root         (0) root         (0)    17272 2023-05-03 16:59:58.000000 blond-2.1.0/blond/input_parameters/ring.py
--rw-r--r--   0 root         (0) root         (0)    22443 2023-05-03 16:59:58.000000 blond-2.1.0/blond/input_parameters/ring_options.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:00:33.416000 blond-2.1.0/blond/llrf/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 16:59:58.000000 blond-2.1.0/blond/llrf/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22090 2023-05-03 16:59:58.000000 blond-2.1.0/blond/llrf/beam_feedback.py
--rw-r--r--   0 root         (0) root         (0)    36313 2023-05-03 16:59:58.000000 blond-2.1.0/blond/llrf/cavity_feedback.py
--rw-r--r--   0 root         (0) root         (0)    14383 2023-05-03 16:59:58.000000 blond-2.1.0/blond/llrf/impulse_response.py
--rw-r--r--   0 root         (0) root         (0)     2337 2023-05-03 16:59:58.000000 blond-2.1.0/blond/llrf/notch_filter.py
--rw-r--r--   0 root         (0) root         (0)     7257 2023-05-03 16:59:58.000000 blond-2.1.0/blond/llrf/offset_frequency.py
--rw-r--r--   0 root         (0) root         (0)     4394 2023-05-03 16:59:58.000000 blond-2.1.0/blond/llrf/rf_modulation.py
--rw-r--r--   0 root         (0) root         (0)    15759 2023-05-03 16:59:58.000000 blond-2.1.0/blond/llrf/rf_noise.py
--rw-r--r--   0 root         (0) root         (0)    18814 2023-05-03 16:59:58.000000 blond-2.1.0/blond/llrf/signal_processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:00:33.416000 blond-2.1.0/blond/monitors/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 16:59:58.000000 blond-2.1.0/blond/monitors/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20936 2023-05-03 16:59:58.000000 blond-2.1.0/blond/monitors/monitors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:00:33.416000 blond-2.1.0/blond/plots/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 16:59:58.000000 blond-2.1.0/blond/plots/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11025 2023-05-03 16:59:58.000000 blond-2.1.0/blond/plots/plot.py
--rw-r--r--   0 root         (0) root         (0)    10004 2023-05-03 16:59:58.000000 blond-2.1.0/blond/plots/plot_beams.py
--rw-r--r--   0 root         (0) root         (0)     4777 2023-05-03 16:59:58.000000 blond-2.1.0/blond/plots/plot_impedance.py
--rw-r--r--   0 root         (0) root         (0)    14165 2023-05-03 16:59:58.000000 blond-2.1.0/blond/plots/plot_llrf.py
--rw-r--r--   0 root         (0) root         (0)     1210 2023-05-03 16:59:58.000000 blond-2.1.0/blond/plots/plot_parameters.py
--rw-r--r--   0 root         (0) root         (0)     2725 2023-05-03 16:59:58.000000 blond-2.1.0/blond/plots/plot_slices.py
--rw-r--r--   0 root         (0) root         (0)     6671 2023-05-03 16:59:58.000000 blond-2.1.0/blond/sanity_check.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:00:33.416000 blond-2.1.0/blond/synchrotron_radiation/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 16:59:58.000000 blond-2.1.0/blond/synchrotron_radiation/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5364 2023-05-03 16:59:58.000000 blond-2.1.0/blond/synchrotron_radiation/synchrotron_radiation.cpp
--rw-r--r--   0 root         (0) root         (0)     8111 2023-05-03 16:59:58.000000 blond-2.1.0/blond/synchrotron_radiation/synchrotron_radiation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:00:33.420000 blond-2.1.0/blond/toolbox/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 16:59:58.000000 blond-2.1.0/blond/toolbox/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5221 2023-05-03 16:59:58.000000 blond-2.1.0/blond/toolbox/action.py
--rw-r--r--   0 root         (0) root         (0)     7570 2023-05-03 16:59:58.000000 blond-2.1.0/blond/toolbox/diffusion.py
--rw-r--r--   0 root         (0) root         (0)     7484 2023-05-03 16:59:58.000000 blond-2.1.0/blond/toolbox/filters_and_fitting.py
--rw-r--r--   0 root         (0) root         (0)     2070 2023-05-03 16:59:58.000000 blond-2.1.0/blond/toolbox/logger.py
--rw-r--r--   0 root         (0) root         (0)     3377 2023-05-03 16:59:58.000000 blond-2.1.0/blond/toolbox/next_regular.py
--rw-r--r--   0 root         (0) root         (0)    21008 2023-05-03 16:59:58.000000 blond-2.1.0/blond/toolbox/parameter_scaling.py
--rw-r--r--   0 root         (0) root         (0)     2358 2023-05-03 16:59:58.000000 blond-2.1.0/blond/toolbox/tomoscope.cpp
--rw-r--r--   0 root         (0) root         (0)     4877 2023-05-03 16:59:58.000000 blond-2.1.0/blond/toolbox/tomoscope.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:00:33.420000 blond-2.1.0/blond/trackers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 16:59:58.000000 blond-2.1.0/blond/trackers/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26351 2023-05-03 16:59:58.000000 blond-2.1.0/blond/trackers/tracker.py
--rw-r--r--   0 root         (0) root         (0)    31233 2023-05-03 16:59:58.000000 blond-2.1.0/blond/trackers/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:00:33.424000 blond-2.1.0/blond/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 16:59:58.000000 blond-2.1.0/blond/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8233 2023-05-03 16:59:58.000000 blond-2.1.0/blond/utils/bmath.py
--rw-r--r--   0 root         (0) root         (0)    48243 2023-05-03 16:59:58.000000 blond-2.1.0/blond/utils/butils_wrap.py
--rw-r--r--   0 root         (0) root         (0)     3467 2023-05-03 16:59:58.000000 blond-2.1.0/blond/utils/data_check.py
--rw-r--r--   0 root         (0) root         (0)     1965 2023-05-03 16:59:58.000000 blond-2.1.0/blond/utils/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     4145 2023-05-03 16:59:58.000000 blond-2.1.0/blond/utils/input_parser.py
--rw-r--r--   0 root         (0) root         (0)    14206 2023-05-03 16:59:58.000000 blond-2.1.0/blond/utils/mpi_config.py
--rw-r--r--   0 root         (0) root         (0)     1021 2023-05-03 16:59:58.000000 blond-2.1.0/blond/utils/profile_mock.py
--rw-r--r--   0 root         (0) root         (0)     3914 2023-05-03 16:59:58.000000 blond-2.1.0/blond/utils/track_iteration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:00:33.404000 blond-2.1.0/blond.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13244 2023-05-03 17:00:33.000000 blond-2.1.0/blond.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9882 2023-05-03 17:00:33.000000 blond-2.1.0/blond.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 17:00:33.000000 blond-2.1.0/blond.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 17:00:28.000000 blond-2.1.0/blond.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      226 2023-05-03 17:00:33.000000 blond-2.1.0/blond.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-03 17:00:33.000000 blond-2.1.0/blond.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      207 2023-05-03 16:59:58.000000 blond-2.1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       42 2023-05-03 16:59:58.000000 blond-2.1.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 17:00:33.432000 blond-2.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     4450 2023-05-03 16:59:58.000000 blond-2.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:00:33.376000 blond-2.1.0/unittests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:00:33.424000 blond-2.1.0/unittests/beam_profile/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 16:59:58.000000 blond-2.1.0/unittests/beam_profile/__init__.py
--rw-r--r--   0 root         (0) root         (0)   800196 2023-05-03 16:59:58.000000 blond-2.1.0/unittests/beam_profile/dt_coordinates.npz
--rw-r--r--   0 root         (0) root         (0)    12422 2023-05-03 16:59:58.000000 blond-2.1.0/unittests/beam_profile/test_beam_profile_object.py
--rw-r--r--   0 root         (0) root         (0)     7221 2023-05-03 16:59:58.000000 blond-2.1.0/unittests/beam_profile/test_sparse_profile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:00:33.424000 blond-2.1.0/unittests/beams/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 16:59:58.000000 blond-2.1.0/unittests/beams/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14105 2023-05-03 16:59:58.000000 blond-2.1.0/unittests/beams/test_beam_object.py
--rw-r--r--   0 root         (0) root         (0)     5659 2023-05-03 16:59:58.000000 blond-2.1.0/unittests/beams/test_coasting_beam.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:00:33.424000 blond-2.1.0/unittests/general/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 16:59:58.000000 blond-2.1.0/unittests/general/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16184 2023-05-03 16:59:58.000000 blond-2.1.0/unittests/general/test_separatrix_bigaussian.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:00:33.424000 blond-2.1.0/unittests/gpu/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 16:59:58.000000 blond-2.1.0/unittests/gpu/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5011 2023-05-03 16:59:58.000000 blond-2.1.0/unittests/gpu/test_ffts.py
--rw-r--r--   0 root         (0) root         (0)    16996 2023-05-03 16:59:58.000000 blond-2.1.0/unittests/gpu/test_impedance.py
--rw-r--r--   0 root         (0) root         (0)    22133 2023-05-03 16:59:58.000000 blond-2.1.0/unittests/gpu/test_physics_kernels.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:00:33.424000 blond-2.1.0/unittests/impedances/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 16:59:58.000000 blond-2.1.0/unittests/impedances/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4475 2023-05-03 16:59:58.000000 blond-2.1.0/unittests/impedances/test_impedance.py
--rwxr-xr-x   0 root         (0) root         (0)     4940 2023-05-03 16:59:58.000000 blond-2.1.0/unittests/impedances/test_impedance_sources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:00:33.428000 blond-2.1.0/unittests/input_parameters/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 16:59:58.000000 blond-2.1.0/unittests/input_parameters/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2695 2023-05-03 16:59:58.000000 blond-2.1.0/unittests/input_parameters/test_preprocess.py
--rw-r--r--   0 root         (0) root         (0)    10862 2023-05-03 16:59:58.000000 blond-2.1.0/unittests/input_parameters/test_rf_params_object.py
--rw-r--r--   0 root         (0) root         (0)     7576 2023-05-03 16:59:58.000000 blond-2.1.0/unittests/input_parameters/test_ring.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:00:33.428000 blond-2.1.0/unittests/integration/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 16:59:58.000000 blond-2.1.0/unittests/integration/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4307 2023-05-03 16:59:58.000000 blond-2.1.0/unittests/integration/test_examples.py
--rw-r--r--   0 root         (0) root         (0)     3047 2023-05-03 16:59:58.000000 blond-2.1.0/unittests/integration/test_gpu_examples.py
--rw-r--r--   0 root         (0) root         (0)     3043 2023-05-03 16:59:58.000000 blond-2.1.0/unittests/integration/test_mpi_examples.py
--rw-r--r--   0 root         (0) root         (0)     4116 2023-05-03 16:59:58.000000 blond-2.1.0/unittests/integration/test_validate_gpu.py
--rw-r--r--   0 root         (0) root         (0)     4005 2023-05-03 16:59:58.000000 blond-2.1.0/unittests/integration/test_validate_mpi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:00:33.428000 blond-2.1.0/unittests/llrf/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 16:59:58.000000 blond-2.1.0/unittests/llrf/__init__.py
--rw-r--r--   0 root         (0) root         (0)    74048 2023-05-03 16:59:58.000000 blond-2.1.0/unittests/llrf/ref_DV_MOD_FR.npy
--rw-r--r--   0 root         (0) root         (0)    74048 2023-05-03 16:59:58.000000 blond-2.1.0/unittests/llrf/ref_DV_MOD_FRF.npy
--rw-r--r--   0 root         (0) root         (0)    74048 2023-05-03 16:59:58.000000 blond-2.1.0/unittests/llrf/ref_V_IND_COARSE_GEN.npy
--rw-r--r--   0 root         (0) root         (0)     8741 2023-05-03 16:59:58.000000 blond-2.1.0/unittests/llrf/test_beam_feedback.py
--rw-r--r--   0 root         (0) root         (0)    31675 2023-05-03 16:59:58.000000 blond-2.1.0/unittests/llrf/test_cavity_feedback.py
--rw-r--r--   0 root         (0) root         (0)    40554 2023-05-03 16:59:58.000000 blond-2.1.0/unittests/llrf/test_impulse_response.py
--rw-r--r--   0 root         (0) root         (0)     3649 2023-05-03 16:59:58.000000 blond-2.1.0/unittests/llrf/test_offset_frequency.py
--rw-r--r--   0 root         (0) root         (0)     8157 2023-05-03 16:59:58.000000 blond-2.1.0/unittests/llrf/test_rf_modulation.py
--rw-r--r--   0 root         (0) root         (0)    31838 2023-05-03 16:59:58.000000 blond-2.1.0/unittests/llrf/test_signal_processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:00:33.428000 blond-2.1.0/unittests/synchrotron_radiation/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 16:59:58.000000 blond-2.1.0/unittests/synchrotron_radiation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32615 2023-05-03 16:59:58.000000 blond-2.1.0/unittests/synchrotron_radiation/test_synch_rad.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:00:33.432000 blond-2.1.0/unittests/trackers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 16:59:58.000000 blond-2.1.0/unittests/trackers/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17866 2023-05-03 16:59:58.000000 blond-2.1.0/unittests/trackers/comparison_drift.py
--rw-r--r--   0 root         (0) root         (0)    19415 2023-05-03 16:59:58.000000 blond-2.1.0/unittests/trackers/test_drift.py
--rw-r--r--   0 root         (0) root         (0)    10188 2023-05-03 16:59:58.000000 blond-2.1.0/unittests/trackers/test_tracker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:00:33.432000 blond-2.1.0/unittests/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 16:59:58.000000 blond-2.1.0/unittests/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21108 2023-05-03 16:59:58.000000 blond-2.1.0/unittests/utils/test_blondmath.py
--rw-r--r--   0 root         (0) root         (0)     3790 2023-05-03 16:59:58.000000 blond-2.1.0/unittests/utils/test_data_check.py
--rw-r--r--   0 root         (0) root         (0)     9952 2023-05-03 16:59:58.000000 blond-2.1.0/unittests/utils/test_ffts.py
--rw-r--r--   0 root         (0) root         (0)     5103 2023-05-03 16:59:58.000000 blond-2.1.0/unittests/utils/test_iteration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.628000 blond-2.1.1/
+-rw-r--r--   0 root         (0) root         (0)      399 2023-05-04 09:50:22.000000 blond-2.1.1/.coveragerc
+-rw-r--r--   0 root         (0) root         (0)     6226 2023-05-04 09:50:22.000000 blond-2.1.1/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     2869 2023-05-04 09:50:22.000000 blond-2.1.1/.gitlab-ci.yml
+-rw-r--r--   0 root         (0) root         (0)     1665 2023-05-04 09:50:22.000000 blond-2.1.1/CHANGELOG
+-rw-r--r--   0 root         (0) root         (0)    35797 2023-05-04 09:50:22.000000 blond-2.1.1/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      339 2023-05-04 09:50:22.000000 blond-2.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    13244 2023-05-04 09:50:52.628000 blond-2.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12468 2023-05-04 09:50:22.000000 blond-2.1.1/README.md
+-rw-r--r--   0 root         (0) root         (0)      794 2023-05-04 09:50:22.000000 blond-2.1.1/WARNINGS.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.592000 blond-2.1.1/__BENCHMARKS/
+-rw-r--r--   0 root         (0) root         (0)       55 2023-05-04 09:50:22.000000 blond-2.1.1/__BENCHMARKS/.gitignore
+-rw-r--r--   0 root         (0) root         (0)    16964 2023-05-04 09:50:22.000000 blond-2.1.1/__BENCHMARKS/BM1_OTFB_Vind_beam_1.py
+-rw-r--r--   0 root         (0) root         (0)     4291 2023-05-04 09:50:22.000000 blond-2.1.1/__BENCHMARKS/BM2_OTFB_no_beam.py
+-rw-r--r--   0 root         (0) root         (0)     1270 2023-05-04 09:50:22.000000 blond-2.1.1/__BENCHMARKS/BM3_OTFB_moving_average.py
+-rw-r--r--   0 root         (0) root         (0)     7415 2023-05-04 09:50:22.000000 blond-2.1.1/__BENCHMARKS/BM4_OTFB_with_beam.py
+-rw-r--r--   0 root         (0) root         (0)     8956 2023-05-04 09:50:22.000000 blond-2.1.1/__BENCHMARKS/BM5_OTFB_feedforward.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.584000 blond-2.1.1/__EXAMPLES/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.592000 blond-2.1.1/__EXAMPLES/gpu_main_files/
+-rw-r--r--   0 root         (0) root         (0)     5807 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/gpu_main_files/EX_01_Acceleration.py
+-rw-r--r--   0 root         (0) root         (0)     8578 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/gpu_main_files/EX_02_Main_long_ps_booster.py
+-rw-r--r--   0 root         (0) root         (0)     6581 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/gpu_main_files/EX_03_RFnoise.py
+-rw-r--r--   0 root         (0) root         (0)     7056 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/gpu_main_files/EX_04_Stationary_multistation.py
+-rw-r--r--   0 root         (0) root         (0)    14174 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/gpu_main_files/EX_05_Wake_impedance.py
+-rw-r--r--   0 root         (0) root         (0)     7328 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/gpu_main_files/EX_07_Ions.py
+-rw-r--r--   0 root         (0) root         (0)     5041 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/gpu_main_files/EX_08_Phase_Loop.py
+-rw-r--r--   0 root         (0) root         (0)     5582 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/gpu_main_files/EX_09_Radial_Loop.py
+-rw-r--r--   0 root         (0) root         (0)     5941 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/gpu_main_files/EX_10_Fixed_frequency.py
+-rw-r--r--   0 root         (0) root         (0)     5953 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/gpu_main_files/EX_16_impedance_test.py
+-rw-r--r--   0 root         (0) root         (0)     9212 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/gpu_main_files/EX_17_multi_turn_wake.py
+-rw-r--r--   0 root         (0) root         (0)     8115 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/gpu_main_files/EX_18_robinson_instability.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.592000 blond-2.1.1/__EXAMPLES/input_files/
+-rw-r--r--   0 root         (0) root         (0)    11866 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/input_files/EX_02_Ekicker_1.4GeV.txt
+-rw-r--r--   0 root         (0) root         (0)    16868 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/input_files/EX_02_Finemet.txt
+-rw-r--r--   0 root         (0) root         (0)     1043 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/input_files/EX_05_new_HQ_table.dat
+-rw-r--r--   0 root         (0) root         (0)    11976 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/input_files/EX_06_Source_TOF_P.csv
+-rw-r--r--   0 root         (0) root         (0)      170 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/input_files/EX_06_voltage_program_LHC25_c02.txt
+-rw-r--r--   0 root         (0) root         (0)      316 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/input_files/EX_06_voltage_program_LHC25_c04.txt
+-rw-r--r--   0 root         (0) root         (0)      101 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/input_files/EX_06_voltage_program_LHC25_c16.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.596000 blond-2.1.1/__EXAMPLES/main_files/
+-rw-r--r--   0 root         (0) root         (0)     4668 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/main_files/EX_01_Acceleration.py
+-rw-r--r--   0 root         (0) root         (0)     7353 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/main_files/EX_02_Main_long_ps_booster.py
+-rw-r--r--   0 root         (0) root         (0)     5605 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/main_files/EX_03_RFnoise.py
+-rw-r--r--   0 root         (0) root         (0)     5413 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/main_files/EX_04_Stationary_multistation.py
+-rw-r--r--   0 root         (0) root         (0)    11556 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/main_files/EX_05_Wake_impedance.py
+-rw-r--r--   0 root         (0) root         (0)     3396 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/main_files/EX_06_Preprocess.py
+-rw-r--r--   0 root         (0) root         (0)     6400 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/main_files/EX_07_Ions.py
+-rw-r--r--   0 root         (0) root         (0)     4348 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/main_files/EX_08_Phase_Loop.py
+-rw-r--r--   0 root         (0) root         (0)     4864 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/main_files/EX_09_Radial_Loop.py
+-rw-r--r--   0 root         (0) root         (0)     4938 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/main_files/EX_10_Fixed_frequency.py
+-rw-r--r--   0 root         (0) root         (0)     4651 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/main_files/EX_11_comparison_music_fourier_analytical.py
+-rw-r--r--   0 root         (0) root         (0)    11630 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/main_files/EX_12_synchrotron_frequency_distribution.py
+-rw-r--r--   0 root         (0) root         (0)    10276 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/main_files/EX_13_synchrotron_radiation.py
+-rw-r--r--   0 root         (0) root         (0)     4639 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/main_files/EX_14_sparse_slicing.py
+-rw-r--r--   0 root         (0) root         (0)     4665 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/main_files/EX_15_sparse_multi_bunch.py
+-rw-r--r--   0 root         (0) root         (0)     5447 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/main_files/EX_16_impedance_test.py
+-rw-r--r--   0 root         (0) root         (0)     7736 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/main_files/EX_17_multi_turn_wake.py
+-rw-r--r--   0 root         (0) root         (0)     7438 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/main_files/EX_18_robinson_instability.py
+-rw-r--r--   0 root         (0) root         (0)     6098 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/main_files/EX_19_bunch_generation.py
+-rw-r--r--   0 root         (0) root         (0)     6646 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/main_files/EX_20_bunch_generation_multibunch.py
+-rw-r--r--   0 root         (0) root         (0)     3132 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/main_files/EX_21_bunch_distribution.py
+-rwxr-xr-x   0 root         (0) root         (0)     4029 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/main_files/EX_22_Coherent_Radiation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.596000 blond-2.1.1/__EXAMPLES/mpi_main_files/
+-rw-r--r--   0 root         (0) root         (0)     5008 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/mpi_main_files/EX_01_Acceleration.py
+-rw-r--r--   0 root         (0) root         (0)     7618 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/mpi_main_files/EX_02_Main_long_ps_booster.py
+-rw-r--r--   0 root         (0) root         (0)     5932 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/mpi_main_files/EX_03_RFnoise.py
+-rw-r--r--   0 root         (0) root         (0)     5703 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/mpi_main_files/EX_04_Stationary_multistation.py
+-rw-r--r--   0 root         (0) root         (0)    12098 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/mpi_main_files/EX_05_Wake_impedance.py
+-rw-r--r--   0 root         (0) root         (0)     6688 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/mpi_main_files/EX_07_Ions.py
+-rw-r--r--   0 root         (0) root         (0)     4632 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/mpi_main_files/EX_08_Phase_Loop.py
+-rw-r--r--   0 root         (0) root         (0)     5181 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/mpi_main_files/EX_09_Radial_Loop.py
+-rw-r--r--   0 root         (0) root         (0)     5255 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/mpi_main_files/EX_10_Fixed_frequency.py
+-rw-r--r--   0 root         (0) root         (0)     5659 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/mpi_main_files/EX_16_impedance_test.py
+-rw-r--r--   0 root         (0) root         (0)     7914 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/mpi_main_files/EX_18_robinson_instability.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.596000 blond-2.1.1/__doc/
+-rw-r--r--   0 root         (0) root         (0)      603 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/Makefile
+-rw-r--r--   0 root         (0) root         (0)     5664 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/conf.py
+-rw-r--r--   0 root         (0) root         (0)     1162 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/index.rst
+-rw-r--r--   0 root         (0) root         (0)      809 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/make.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.600000 blond-2.1.1/__doc/modules/
+-rwxr-xr-x   0 root         (0) root         (0)   135010 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/modules/ACS_cavity_loop.png
+-rwxr-xr-x   0 root         (0) root         (0)   185223 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/modules/ACS_cavity_loop.svg
+-rwxr-xr-x   0 root         (0) root         (0)     1144 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/modules/RF_noise.gle
+-rwxr-xr-x   0 root         (0) root         (0)    81234 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/modules/RF_noise.png
+-rwxr-xr-x   0 root         (0) root         (0)   176302 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/modules/SPS_OTFB.png
+-rwxr-xr-x   0 root         (0) root         (0)   655573 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/modules/SPS_OTFB.svg
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/modules/beam.rst
+-rw-r--r--   0 root         (0) root         (0)      177 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/modules/compile.rst
+-rw-r--r--   0 root         (0) root         (0)    51317 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/modules/csr_impedance_real.png
+-rw-r--r--   0 root         (0) root         (0)    19684 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/modules/equations_of_motion.rst
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/modules/impedances.rst
+-rw-r--r--   0 root         (0) root         (0)      754 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/modules/input_parameters.rst
+-rwxr-xr-x   0 root         (0) root         (0)     7100 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/modules/lhc_cavity_loop.rst
+-rw-r--r--   0 root         (0) root         (0)    20259 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/modules/llrf.rst
+-rw-r--r--   0 root         (0) root         (0)      191 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/modules/monitors.rst
+-rw-r--r--   0 root         (0) root         (0)      977 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/modules/plots.rst
+-rwxr-xr-x   0 root         (0) root         (0)     1050 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/modules/ring_and_RFstation.gle
+-rwxr-xr-x   0 root         (0) root         (0)    84423 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/modules/ring_and_RFstation.png
+-rwxr-xr-x   0 root         (0) root         (0)       39 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/modules/sample.dat
+-rwxr-xr-x   0 root         (0) root         (0)       77 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/modules/sample2.dat
+-rwxr-xr-x   0 root         (0) root         (0)    14087 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/modules/sps_cavity_loop.rst
+-rw-r--r--   0 root         (0) root         (0)      269 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/modules/synchrotron_radiation.rst
+-rw-r--r--   0 root         (0) root         (0)     1166 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/modules/toolbox.rst
+-rw-r--r--   0 root         (0) root         (0)      344 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/modules/trackers.rst
+-rw-r--r--   0 root         (0) root         (0)      484 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/modules/utils.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.584000 blond-2.1.1/__doc/themes/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.604000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/
+-rw-r--r--   0 root         (0) root         (0)      324 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3740 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/breadcrumbs.html
+-rw-r--r--   0 root         (0) root         (0)     1978 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/footer.html
+-rw-r--r--   0 root         (0) root         (0)     7063 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/layout.html
+-rw-r--r--   0 root         (0) root         (0)     7526 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/layout_old.html
+-rw-r--r--   0 root         (0) root         (0)     1530 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/search.html
+-rw-r--r--   0 root         (0) root         (0)      365 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/searchbox.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.588000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.604000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/css/
+-rw-r--r--   0 root         (0) root         (0)     3381 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/css/badge_only.css
+-rw-r--r--   0 root         (0) root         (0)     3153 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/css/badge_only.css.map
+-rw-r--r--   0 root         (0) root         (0)   114281 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/css/theme.css
+-rw-r--r--   0 root         (0) root         (0)    67610 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/css/theme.css.map
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.608000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/fonts/
+-rw-r--r--   0 root         (0) root         (0)   124988 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/fonts/FontAwesome.otf
+-rw-r--r--   0 root         (0) root         (0)   109948 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/fonts/Inconsolata-Bold.ttf
+-rw-r--r--   0 root         (0) root         (0)    96964 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/fonts/Inconsolata-Regular.ttf
+-rw-r--r--   0 root         (0) root         (0)   656544 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/fonts/Lato-Bold.ttf
+-rw-r--r--   0 root         (0) root         (0)   656568 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/fonts/Lato-Regular.ttf
+-rw-r--r--   0 root         (0) root         (0)   170616 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/fonts/RobotoSlab-Bold.ttf
+-rw-r--r--   0 root         (0) root         (0)   169064 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/fonts/RobotoSlab-Regular.ttf
+-rw-r--r--   0 root         (0) root         (0)    76518 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 root         (0) root         (0)   391622 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 root         (0) root         (0)   152796 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 root         (0) root         (0)    90412 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 root         (0) root         (0)    71896 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.woff2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.608000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/js/
+-rw-r--r--   0 root         (0) root         (0)     2457 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/js/copybutton.js
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/js/copybutton.js~
+-rw-r--r--   0 root         (0) root         (0)    15414 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/js/modernizr.min.js
+-rw-r--r--   0 root         (0) root         (0)     6477 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/js/theme.js
+-rw-r--r--   0 root         (0) root         (0)      260 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/theme.conf
+-rw-r--r--   0 root         (0) root         (0)     1299 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/versions.html
+-rw-r--r--   0 root         (0) root         (0)     1380 2023-05-04 09:50:22.000000 blond-2.1.1/appveyor.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.608000 blond-2.1.1/blond/
+-rw-r--r--   0 root         (0) root         (0)     1199 2023-05-04 09:50:22.000000 blond-2.1.1/blond/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      160 2023-05-04 09:50:48.000000 blond-2.1.1/blond/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.612000 blond-2.1.1/blond/beam/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 09:50:22.000000 blond-2.1.1/blond/beam/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20461 2023-05-04 09:50:22.000000 blond-2.1.1/blond/beam/beam.py
+-rw-r--r--   0 root         (0) root         (0)     3685 2023-05-04 09:50:22.000000 blond-2.1.1/blond/beam/coasting_beam.py
+-rw-r--r--   0 root         (0) root         (0)    41527 2023-05-04 09:50:22.000000 blond-2.1.1/blond/beam/distributions.py
+-rw-r--r--   0 root         (0) root         (0)    39107 2023-05-04 09:50:22.000000 blond-2.1.1/blond/beam/distributions_multibunch.py
+-rw-r--r--   0 root         (0) root         (0)    24385 2023-05-04 09:50:22.000000 blond-2.1.1/blond/beam/profile.py
+-rw-r--r--   0 root         (0) root         (0)     5740 2023-05-04 09:50:22.000000 blond-2.1.1/blond/beam/sparse_histogram.cpp
+-rw-r--r--   0 root         (0) root         (0)     4804 2023-05-04 09:50:22.000000 blond-2.1.1/blond/beam/sparse_slices.py
+-rw-r--r--   0 root         (0) root         (0)    11654 2023-05-04 09:50:22.000000 blond-2.1.1/blond/compile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.612000 blond-2.1.1/blond/cpp_routines/
+-rw-r--r--   0 root         (0) root         (0)     3088 2023-05-04 09:50:22.000000 blond-2.1.1/blond/cpp_routines/beam_phase.cpp
+-rw-r--r--   0 root         (0) root         (0)    29022 2023-05-04 09:50:22.000000 blond-2.1.1/blond/cpp_routines/blondmath.cpp
+-rw-r--r--   0 root         (0) root         (0)    13334 2023-05-04 09:50:22.000000 blond-2.1.1/blond/cpp_routines/blondmath.h
+-rw-r--r--   0 root         (0) root         (0)     1316 2023-05-04 09:50:22.000000 blond-2.1.1/blond/cpp_routines/cos.h
+-rw-r--r--   0 root         (0) root         (0)     5747 2023-05-04 09:50:22.000000 blond-2.1.1/blond/cpp_routines/drift.cpp
+-rw-r--r--   0 root         (0) root         (0)     4376 2023-05-04 09:50:22.000000 blond-2.1.1/blond/cpp_routines/exp.h
+-rw-r--r--   0 root         (0) root         (0)     4661 2023-05-04 09:50:22.000000 blond-2.1.1/blond/cpp_routines/fast_resonator.cpp
+-rw-r--r--   0 root         (0) root         (0)    29481 2023-05-04 09:50:22.000000 blond-2.1.1/blond/cpp_routines/fft.cpp
+-rw-r--r--   0 root         (0) root         (0)     4419 2023-05-04 09:50:22.000000 blond-2.1.1/blond/cpp_routines/fft.h
+-rw-r--r--   0 root         (0) root         (0)    10013 2023-05-04 09:50:22.000000 blond-2.1.1/blond/cpp_routines/histogram.cpp
+-rw-r--r--   0 root         (0) root         (0)     3493 2023-05-04 09:50:22.000000 blond-2.1.1/blond/cpp_routines/kick.cpp
+-rwxr-xr-x   0 root         (0) root         (0)   126096 2023-05-04 09:50:52.000000 blond-2.1.1/blond/cpp_routines/libblond.so
+-rw-r--r--   0 root         (0) root         (0)     6406 2023-05-04 09:50:22.000000 blond-2.1.1/blond/cpp_routines/linear_interp_kick.cpp
+-rw-r--r--   0 root         (0) root         (0)    15181 2023-05-04 09:50:22.000000 blond-2.1.1/blond/cpp_routines/music_track.cpp
+-rw-r--r--   0 root         (0) root         (0)      169 2023-05-04 09:50:22.000000 blond-2.1.1/blond/cpp_routines/openmp.cpp
+-rw-r--r--   0 root         (0) root         (0)      245 2023-05-04 09:50:22.000000 blond-2.1.1/blond/cpp_routines/openmp.h
+-rw-r--r--   0 root         (0) root         (0)     1960 2023-05-04 09:50:22.000000 blond-2.1.1/blond/cpp_routines/sin.h
+-rw-r--r--   0 root         (0) root         (0)     5871 2023-05-04 09:50:22.000000 blond-2.1.1/blond/cpp_routines/sincos.h
+-rw-r--r--   0 root         (0) root         (0)     7480 2023-05-04 09:50:22.000000 blond-2.1.1/blond/cpp_routines/vdtcore_common.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.612000 blond-2.1.1/blond/gpu/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 09:50:22.000000 blond-2.1.1/blond/gpu/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.612000 blond-2.1.1/blond/gpu/cuda_kernels/
+-rw-r--r--   0 root         (0) root         (0)    14390 2023-05-04 09:50:22.000000 blond-2.1.1/blond/gpu/cuda_kernels/kernels_double.cu
+-rw-r--r--   0 root         (0) root         (0)    14135 2023-05-04 09:50:22.000000 blond-2.1.1/blond/gpu/cuda_kernels/kernels_single.cu
+-rw-r--r--   0 root         (0) root         (0)    10769 2023-05-04 09:50:22.000000 blond-2.1.1/blond/gpu/cupy_butils_wrap.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.616000 blond-2.1.1/blond/impedances/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 09:50:22.000000 blond-2.1.1/blond/impedances/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39560 2023-05-04 09:50:22.000000 blond-2.1.1/blond/impedances/impedance.py
+-rw-r--r--   0 root         (0) root         (0)    45892 2023-05-04 09:50:22.000000 blond-2.1.1/blond/impedances/impedance_sources.py
+-rw-r--r--   0 root         (0) root         (0)     3541 2023-05-04 09:50:22.000000 blond-2.1.1/blond/impedances/induced_voltage_analytical.py
+-rw-r--r--   0 root         (0) root         (0)    12228 2023-05-04 09:50:22.000000 blond-2.1.1/blond/impedances/music.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.616000 blond-2.1.1/blond/input_parameters/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 09:50:22.000000 blond-2.1.1/blond/input_parameters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24903 2023-05-04 09:50:22.000000 blond-2.1.1/blond/input_parameters/rf_parameters.py
+-rw-r--r--   0 root         (0) root         (0)    20249 2023-05-04 09:50:22.000000 blond-2.1.1/blond/input_parameters/rf_parameters_options.py
+-rw-r--r--   0 root         (0) root         (0)    17272 2023-05-04 09:50:22.000000 blond-2.1.1/blond/input_parameters/ring.py
+-rw-r--r--   0 root         (0) root         (0)    22443 2023-05-04 09:50:22.000000 blond-2.1.1/blond/input_parameters/ring_options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.616000 blond-2.1.1/blond/llrf/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 09:50:22.000000 blond-2.1.1/blond/llrf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22090 2023-05-04 09:50:22.000000 blond-2.1.1/blond/llrf/beam_feedback.py
+-rw-r--r--   0 root         (0) root         (0)    36313 2023-05-04 09:50:22.000000 blond-2.1.1/blond/llrf/cavity_feedback.py
+-rw-r--r--   0 root         (0) root         (0)    14383 2023-05-04 09:50:22.000000 blond-2.1.1/blond/llrf/impulse_response.py
+-rw-r--r--   0 root         (0) root         (0)     2337 2023-05-04 09:50:22.000000 blond-2.1.1/blond/llrf/notch_filter.py
+-rw-r--r--   0 root         (0) root         (0)     7257 2023-05-04 09:50:22.000000 blond-2.1.1/blond/llrf/offset_frequency.py
+-rw-r--r--   0 root         (0) root         (0)     4394 2023-05-04 09:50:22.000000 blond-2.1.1/blond/llrf/rf_modulation.py
+-rw-r--r--   0 root         (0) root         (0)    15759 2023-05-04 09:50:22.000000 blond-2.1.1/blond/llrf/rf_noise.py
+-rw-r--r--   0 root         (0) root         (0)    18814 2023-05-04 09:50:22.000000 blond-2.1.1/blond/llrf/signal_processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.616000 blond-2.1.1/blond/monitors/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 09:50:22.000000 blond-2.1.1/blond/monitors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20936 2023-05-04 09:50:22.000000 blond-2.1.1/blond/monitors/monitors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.616000 blond-2.1.1/blond/plots/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 09:50:22.000000 blond-2.1.1/blond/plots/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11025 2023-05-04 09:50:22.000000 blond-2.1.1/blond/plots/plot.py
+-rw-r--r--   0 root         (0) root         (0)    10004 2023-05-04 09:50:22.000000 blond-2.1.1/blond/plots/plot_beams.py
+-rw-r--r--   0 root         (0) root         (0)     4777 2023-05-04 09:50:22.000000 blond-2.1.1/blond/plots/plot_impedance.py
+-rw-r--r--   0 root         (0) root         (0)    14165 2023-05-04 09:50:22.000000 blond-2.1.1/blond/plots/plot_llrf.py
+-rw-r--r--   0 root         (0) root         (0)     1210 2023-05-04 09:50:22.000000 blond-2.1.1/blond/plots/plot_parameters.py
+-rw-r--r--   0 root         (0) root         (0)     2725 2023-05-04 09:50:22.000000 blond-2.1.1/blond/plots/plot_slices.py
+-rw-r--r--   0 root         (0) root         (0)     6671 2023-05-04 09:50:22.000000 blond-2.1.1/blond/sanity_check.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.616000 blond-2.1.1/blond/synchrotron_radiation/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 09:50:22.000000 blond-2.1.1/blond/synchrotron_radiation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5364 2023-05-04 09:50:22.000000 blond-2.1.1/blond/synchrotron_radiation/synchrotron_radiation.cpp
+-rw-r--r--   0 root         (0) root         (0)     8111 2023-05-04 09:50:22.000000 blond-2.1.1/blond/synchrotron_radiation/synchrotron_radiation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.620000 blond-2.1.1/blond/toolbox/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 09:50:22.000000 blond-2.1.1/blond/toolbox/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5221 2023-05-04 09:50:22.000000 blond-2.1.1/blond/toolbox/action.py
+-rw-r--r--   0 root         (0) root         (0)     7570 2023-05-04 09:50:22.000000 blond-2.1.1/blond/toolbox/diffusion.py
+-rw-r--r--   0 root         (0) root         (0)     7484 2023-05-04 09:50:22.000000 blond-2.1.1/blond/toolbox/filters_and_fitting.py
+-rw-r--r--   0 root         (0) root         (0)     2070 2023-05-04 09:50:22.000000 blond-2.1.1/blond/toolbox/logger.py
+-rw-r--r--   0 root         (0) root         (0)     3377 2023-05-04 09:50:22.000000 blond-2.1.1/blond/toolbox/next_regular.py
+-rw-r--r--   0 root         (0) root         (0)    21008 2023-05-04 09:50:22.000000 blond-2.1.1/blond/toolbox/parameter_scaling.py
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-05-04 09:50:22.000000 blond-2.1.1/blond/toolbox/tomoscope.cpp
+-rw-r--r--   0 root         (0) root         (0)     4877 2023-05-04 09:50:22.000000 blond-2.1.1/blond/toolbox/tomoscope.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.620000 blond-2.1.1/blond/trackers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 09:50:22.000000 blond-2.1.1/blond/trackers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26351 2023-05-04 09:50:22.000000 blond-2.1.1/blond/trackers/tracker.py
+-rw-r--r--   0 root         (0) root         (0)    31233 2023-05-04 09:50:22.000000 blond-2.1.1/blond/trackers/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.620000 blond-2.1.1/blond/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 09:50:22.000000 blond-2.1.1/blond/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8233 2023-05-04 09:50:22.000000 blond-2.1.1/blond/utils/bmath.py
+-rw-r--r--   0 root         (0) root         (0)    48243 2023-05-04 09:50:22.000000 blond-2.1.1/blond/utils/butils_wrap.py
+-rw-r--r--   0 root         (0) root         (0)     3467 2023-05-04 09:50:22.000000 blond-2.1.1/blond/utils/data_check.py
+-rw-r--r--   0 root         (0) root         (0)     1965 2023-05-04 09:50:22.000000 blond-2.1.1/blond/utils/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     4145 2023-05-04 09:50:22.000000 blond-2.1.1/blond/utils/input_parser.py
+-rw-r--r--   0 root         (0) root         (0)    14206 2023-05-04 09:50:22.000000 blond-2.1.1/blond/utils/mpi_config.py
+-rw-r--r--   0 root         (0) root         (0)     1021 2023-05-04 09:50:22.000000 blond-2.1.1/blond/utils/profile_mock.py
+-rw-r--r--   0 root         (0) root         (0)     3914 2023-05-04 09:50:22.000000 blond-2.1.1/blond/utils/track_iteration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.608000 blond-2.1.1/blond.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13244 2023-05-04 09:50:52.000000 blond-2.1.1/blond.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9882 2023-05-04 09:50:52.000000 blond-2.1.1/blond.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 09:50:52.000000 blond-2.1.1/blond.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 09:50:48.000000 blond-2.1.1/blond.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      226 2023-05-04 09:50:52.000000 blond-2.1.1/blond.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-04 09:50:52.000000 blond-2.1.1/blond.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      207 2023-05-04 09:50:22.000000 blond-2.1.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       42 2023-05-04 09:50:22.000000 blond-2.1.1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-04 09:50:52.628000 blond-2.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     4446 2023-05-04 09:50:22.000000 blond-2.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.588000 blond-2.1.1/unittests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.620000 blond-2.1.1/unittests/beam_profile/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/beam_profile/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   800196 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/beam_profile/dt_coordinates.npz
+-rw-r--r--   0 root         (0) root         (0)    12422 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/beam_profile/test_beam_profile_object.py
+-rw-r--r--   0 root         (0) root         (0)     7221 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/beam_profile/test_sparse_profile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.620000 blond-2.1.1/unittests/beams/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/beams/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14105 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/beams/test_beam_object.py
+-rw-r--r--   0 root         (0) root         (0)     5659 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/beams/test_coasting_beam.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.620000 blond-2.1.1/unittests/general/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/general/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16184 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/general/test_separatrix_bigaussian.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.624000 blond-2.1.1/unittests/gpu/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/gpu/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5011 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/gpu/test_ffts.py
+-rw-r--r--   0 root         (0) root         (0)    16996 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/gpu/test_impedance.py
+-rw-r--r--   0 root         (0) root         (0)    22133 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/gpu/test_physics_kernels.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.624000 blond-2.1.1/unittests/impedances/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/impedances/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4475 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/impedances/test_impedance.py
+-rwxr-xr-x   0 root         (0) root         (0)     4940 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/impedances/test_impedance_sources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.624000 blond-2.1.1/unittests/input_parameters/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/input_parameters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2695 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/input_parameters/test_preprocess.py
+-rw-r--r--   0 root         (0) root         (0)    10862 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/input_parameters/test_rf_params_object.py
+-rw-r--r--   0 root         (0) root         (0)     7576 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/input_parameters/test_ring.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.624000 blond-2.1.1/unittests/integration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/integration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4307 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/integration/test_examples.py
+-rw-r--r--   0 root         (0) root         (0)     3047 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/integration/test_gpu_examples.py
+-rw-r--r--   0 root         (0) root         (0)     3043 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/integration/test_mpi_examples.py
+-rw-r--r--   0 root         (0) root         (0)     4116 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/integration/test_validate_gpu.py
+-rw-r--r--   0 root         (0) root         (0)     4005 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/integration/test_validate_mpi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.624000 blond-2.1.1/unittests/llrf/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/llrf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    74048 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/llrf/ref_DV_MOD_FR.npy
+-rw-r--r--   0 root         (0) root         (0)    74048 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/llrf/ref_DV_MOD_FRF.npy
+-rw-r--r--   0 root         (0) root         (0)    74048 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/llrf/ref_V_IND_COARSE_GEN.npy
+-rw-r--r--   0 root         (0) root         (0)     8741 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/llrf/test_beam_feedback.py
+-rw-r--r--   0 root         (0) root         (0)    31675 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/llrf/test_cavity_feedback.py
+-rw-r--r--   0 root         (0) root         (0)    40554 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/llrf/test_impulse_response.py
+-rw-r--r--   0 root         (0) root         (0)     3649 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/llrf/test_offset_frequency.py
+-rw-r--r--   0 root         (0) root         (0)     8157 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/llrf/test_rf_modulation.py
+-rw-r--r--   0 root         (0) root         (0)    31838 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/llrf/test_signal_processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.624000 blond-2.1.1/unittests/synchrotron_radiation/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/synchrotron_radiation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32615 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/synchrotron_radiation/test_synch_rad.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.628000 blond-2.1.1/unittests/trackers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/trackers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17866 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/trackers/comparison_drift.py
+-rw-r--r--   0 root         (0) root         (0)    19415 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/trackers/test_drift.py
+-rw-r--r--   0 root         (0) root         (0)    10188 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/trackers/test_tracker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.628000 blond-2.1.1/unittests/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21108 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/utils/test_blondmath.py
+-rw-r--r--   0 root         (0) root         (0)     3790 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/utils/test_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     9952 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/utils/test_ffts.py
+-rw-r--r--   0 root         (0) root         (0)     5103 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/utils/test_iteration.py
```

### Comparing `blond-2.1.0/.gitignore` & `blond-2.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/.gitlab-ci.yml` & `blond-2.1.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/CHANGELOG` & `blond-2.1.1/CHANGELOG`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/LICENSE.txt` & `blond-2.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/PKG-INFO` & `blond-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: blond
-Version: 2.1.0
+Version: 2.1.1
 Summary: CERN code for simulating longitudinal beam dynamics in synchrotrons.
 Home-page: https://gitlab.cern.ch/blond/BLonD
 Author: Helga Timko et al.
 Author-email: helga.timko@cern.ch
 Maintainer: Konstantinos Iliakis
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: core
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: all
 License-File: LICENSE.txt
```

### Comparing `blond-2.1.0/README.md` & `blond-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/WARNINGS.txt` & `blond-2.1.1/WARNINGS.txt`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__BENCHMARKS/BM1_OTFB_Vind_beam_1.py` & `blond-2.1.1/__BENCHMARKS/BM1_OTFB_Vind_beam_1.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__BENCHMARKS/BM2_OTFB_no_beam.py` & `blond-2.1.1/__BENCHMARKS/BM2_OTFB_no_beam.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__BENCHMARKS/BM3_OTFB_moving_average.py` & `blond-2.1.1/__BENCHMARKS/BM3_OTFB_moving_average.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__BENCHMARKS/BM4_OTFB_with_beam.py` & `blond-2.1.1/__BENCHMARKS/BM4_OTFB_with_beam.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__BENCHMARKS/BM5_OTFB_feedforward.py` & `blond-2.1.1/__BENCHMARKS/BM5_OTFB_feedforward.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__EXAMPLES/gpu_main_files/EX_01_Acceleration.py` & `blond-2.1.1/__EXAMPLES/gpu_main_files/EX_01_Acceleration.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__EXAMPLES/gpu_main_files/EX_02_Main_long_ps_booster.py` & `blond-2.1.1/__EXAMPLES/gpu_main_files/EX_02_Main_long_ps_booster.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__EXAMPLES/gpu_main_files/EX_03_RFnoise.py` & `blond-2.1.1/__EXAMPLES/gpu_main_files/EX_03_RFnoise.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__EXAMPLES/gpu_main_files/EX_04_Stationary_multistation.py` & `blond-2.1.1/__EXAMPLES/gpu_main_files/EX_04_Stationary_multistation.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__EXAMPLES/gpu_main_files/EX_05_Wake_impedance.py` & `blond-2.1.1/__EXAMPLES/gpu_main_files/EX_05_Wake_impedance.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__EXAMPLES/gpu_main_files/EX_07_Ions.py` & `blond-2.1.1/__EXAMPLES/gpu_main_files/EX_07_Ions.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__EXAMPLES/gpu_main_files/EX_08_Phase_Loop.py` & `blond-2.1.1/__EXAMPLES/gpu_main_files/EX_08_Phase_Loop.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__EXAMPLES/gpu_main_files/EX_09_Radial_Loop.py` & `blond-2.1.1/__EXAMPLES/gpu_main_files/EX_09_Radial_Loop.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__EXAMPLES/gpu_main_files/EX_10_Fixed_frequency.py` & `blond-2.1.1/__EXAMPLES/gpu_main_files/EX_10_Fixed_frequency.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__EXAMPLES/gpu_main_files/EX_16_impedance_test.py` & `blond-2.1.1/__EXAMPLES/gpu_main_files/EX_16_impedance_test.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__EXAMPLES/gpu_main_files/EX_17_multi_turn_wake.py` & `blond-2.1.1/__EXAMPLES/gpu_main_files/EX_17_multi_turn_wake.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__EXAMPLES/gpu_main_files/EX_18_robinson_instability.py` & `blond-2.1.1/__EXAMPLES/gpu_main_files/EX_18_robinson_instability.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__EXAMPLES/input_files/EX_02_Ekicker_1.4GeV.txt` & `blond-2.1.1/__EXAMPLES/input_files/EX_02_Ekicker_1.4GeV.txt`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__EXAMPLES/input_files/EX_02_Finemet.txt` & `blond-2.1.1/__EXAMPLES/input_files/EX_02_Finemet.txt`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__EXAMPLES/input_files/EX_05_new_HQ_table.dat` & `blond-2.1.1/__EXAMPLES/input_files/EX_05_new_HQ_table.dat`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__EXAMPLES/input_files/EX_06_Source_TOF_P.csv` & `blond-2.1.1/__EXAMPLES/input_files/EX_06_Source_TOF_P.csv`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__EXAMPLES/main_files/EX_01_Acceleration.py` & `blond-2.1.1/__EXAMPLES/main_files/EX_01_Acceleration.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__EXAMPLES/main_files/EX_02_Main_long_ps_booster.py` & `blond-2.1.1/__EXAMPLES/main_files/EX_02_Main_long_ps_booster.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__EXAMPLES/main_files/EX_03_RFnoise.py` & `blond-2.1.1/__EXAMPLES/main_files/EX_03_RFnoise.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__EXAMPLES/main_files/EX_04_Stationary_multistation.py` & `blond-2.1.1/__EXAMPLES/main_files/EX_04_Stationary_multistation.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__EXAMPLES/main_files/EX_05_Wake_impedance.py` & `blond-2.1.1/__EXAMPLES/main_files/EX_05_Wake_impedance.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__EXAMPLES/main_files/EX_06_Preprocess.py` & `blond-2.1.1/__EXAMPLES/main_files/EX_06_Preprocess.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__EXAMPLES/main_files/EX_07_Ions.py` & `blond-2.1.1/__EXAMPLES/main_files/EX_07_Ions.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__EXAMPLES/main_files/EX_08_Phase_Loop.py` & `blond-2.1.1/__EXAMPLES/main_files/EX_08_Phase_Loop.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__EXAMPLES/main_files/EX_09_Radial_Loop.py` & `blond-2.1.1/__EXAMPLES/main_files/EX_09_Radial_Loop.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__EXAMPLES/main_files/EX_10_Fixed_frequency.py` & `blond-2.1.1/__EXAMPLES/main_files/EX_10_Fixed_frequency.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__EXAMPLES/main_files/EX_11_comparison_music_fourier_analytical.py` & `blond-2.1.1/__EXAMPLES/main_files/EX_11_comparison_music_fourier_analytical.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__EXAMPLES/main_files/EX_12_synchrotron_frequency_distribution.py` & `blond-2.1.1/__EXAMPLES/main_files/EX_12_synchrotron_frequency_distribution.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__EXAMPLES/main_files/EX_13_synchrotron_radiation.py` & `blond-2.1.1/__EXAMPLES/main_files/EX_13_synchrotron_radiation.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__EXAMPLES/main_files/EX_14_sparse_slicing.py` & `blond-2.1.1/__EXAMPLES/main_files/EX_14_sparse_slicing.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__EXAMPLES/main_files/EX_15_sparse_multi_bunch.py` & `blond-2.1.1/__EXAMPLES/main_files/EX_15_sparse_multi_bunch.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__EXAMPLES/main_files/EX_16_impedance_test.py` & `blond-2.1.1/__EXAMPLES/main_files/EX_16_impedance_test.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__EXAMPLES/main_files/EX_17_multi_turn_wake.py` & `blond-2.1.1/__EXAMPLES/main_files/EX_17_multi_turn_wake.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__EXAMPLES/main_files/EX_18_robinson_instability.py` & `blond-2.1.1/__EXAMPLES/main_files/EX_18_robinson_instability.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__EXAMPLES/main_files/EX_19_bunch_generation.py` & `blond-2.1.1/__EXAMPLES/main_files/EX_19_bunch_generation.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__EXAMPLES/main_files/EX_20_bunch_generation_multibunch.py` & `blond-2.1.1/__EXAMPLES/main_files/EX_20_bunch_generation_multibunch.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__EXAMPLES/main_files/EX_21_bunch_distribution.py` & `blond-2.1.1/__EXAMPLES/main_files/EX_21_bunch_distribution.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__EXAMPLES/main_files/EX_22_Coherent_Radiation.py` & `blond-2.1.1/__EXAMPLES/main_files/EX_22_Coherent_Radiation.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__EXAMPLES/mpi_main_files/EX_01_Acceleration.py` & `blond-2.1.1/__EXAMPLES/mpi_main_files/EX_01_Acceleration.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__EXAMPLES/mpi_main_files/EX_02_Main_long_ps_booster.py` & `blond-2.1.1/__EXAMPLES/mpi_main_files/EX_02_Main_long_ps_booster.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__EXAMPLES/mpi_main_files/EX_03_RFnoise.py` & `blond-2.1.1/__EXAMPLES/mpi_main_files/EX_03_RFnoise.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__EXAMPLES/mpi_main_files/EX_04_Stationary_multistation.py` & `blond-2.1.1/__EXAMPLES/mpi_main_files/EX_04_Stationary_multistation.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__EXAMPLES/mpi_main_files/EX_05_Wake_impedance.py` & `blond-2.1.1/__EXAMPLES/mpi_main_files/EX_05_Wake_impedance.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__EXAMPLES/mpi_main_files/EX_07_Ions.py` & `blond-2.1.1/__EXAMPLES/mpi_main_files/EX_07_Ions.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__EXAMPLES/mpi_main_files/EX_08_Phase_Loop.py` & `blond-2.1.1/__EXAMPLES/mpi_main_files/EX_08_Phase_Loop.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__EXAMPLES/mpi_main_files/EX_09_Radial_Loop.py` & `blond-2.1.1/__EXAMPLES/mpi_main_files/EX_09_Radial_Loop.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__EXAMPLES/mpi_main_files/EX_10_Fixed_frequency.py` & `blond-2.1.1/__EXAMPLES/mpi_main_files/EX_10_Fixed_frequency.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__EXAMPLES/mpi_main_files/EX_16_impedance_test.py` & `blond-2.1.1/__EXAMPLES/mpi_main_files/EX_16_impedance_test.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__EXAMPLES/mpi_main_files/EX_18_robinson_instability.py` & `blond-2.1.1/__EXAMPLES/mpi_main_files/EX_18_robinson_instability.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__doc/Makefile` & `blond-2.1.1/__doc/Makefile`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__doc/conf.py` & `blond-2.1.1/__doc/conf.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__doc/index.rst` & `blond-2.1.1/__doc/index.rst`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__doc/make.bat` & `blond-2.1.1/__doc/make.bat`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__doc/modules/ACS_cavity_loop.png` & `blond-2.1.1/__doc/modules/ACS_cavity_loop.png`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__doc/modules/ACS_cavity_loop.svg` & `blond-2.1.1/__doc/modules/ACS_cavity_loop.svg`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__doc/modules/RF_noise.gle` & `blond-2.1.1/__doc/modules/RF_noise.gle`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__doc/modules/RF_noise.png` & `blond-2.1.1/__doc/modules/RF_noise.png`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__doc/modules/SPS_OTFB.png` & `blond-2.1.1/__doc/modules/SPS_OTFB.png`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__doc/modules/SPS_OTFB.svg` & `blond-2.1.1/__doc/modules/SPS_OTFB.svg`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__doc/modules/beam.rst` & `blond-2.1.1/__doc/modules/beam.rst`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__doc/modules/csr_impedance_real.png` & `blond-2.1.1/__doc/modules/csr_impedance_real.png`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__doc/modules/equations_of_motion.rst` & `blond-2.1.1/__doc/modules/equations_of_motion.rst`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__doc/modules/impedances.rst` & `blond-2.1.1/__doc/modules/impedances.rst`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__doc/modules/input_parameters.rst` & `blond-2.1.1/__doc/modules/input_parameters.rst`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__doc/modules/lhc_cavity_loop.rst` & `blond-2.1.1/__doc/modules/lhc_cavity_loop.rst`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__doc/modules/llrf.rst` & `blond-2.1.1/__doc/modules/llrf.rst`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__doc/modules/plots.rst` & `blond-2.1.1/__doc/modules/plots.rst`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__doc/modules/ring_and_RFstation.gle` & `blond-2.1.1/__doc/modules/ring_and_RFstation.gle`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__doc/modules/ring_and_RFstation.png` & `blond-2.1.1/__doc/modules/ring_and_RFstation.png`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__doc/modules/sps_cavity_loop.rst` & `blond-2.1.1/__doc/modules/sps_cavity_loop.rst`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__doc/modules/toolbox.rst` & `blond-2.1.1/__doc/modules/toolbox.rst`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__doc/themes/sphinx_rtd_theme/breadcrumbs.html` & `blond-2.1.1/__doc/themes/sphinx_rtd_theme/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__doc/themes/sphinx_rtd_theme/footer.html` & `blond-2.1.1/__doc/themes/sphinx_rtd_theme/footer.html`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__doc/themes/sphinx_rtd_theme/layout.html` & `blond-2.1.1/__doc/themes/sphinx_rtd_theme/layout.html`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__doc/themes/sphinx_rtd_theme/layout_old.html` & `blond-2.1.1/__doc/themes/sphinx_rtd_theme/layout_old.html`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__doc/themes/sphinx_rtd_theme/search.html` & `blond-2.1.1/__doc/themes/sphinx_rtd_theme/search.html`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__doc/themes/sphinx_rtd_theme/static/css/badge_only.css` & `blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__doc/themes/sphinx_rtd_theme/static/css/badge_only.css.map` & `blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/css/badge_only.css.map`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__doc/themes/sphinx_rtd_theme/static/css/theme.css` & `blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/css/theme.css`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__doc/themes/sphinx_rtd_theme/static/css/theme.css.map` & `blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/css/theme.css.map`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__doc/themes/sphinx_rtd_theme/static/fonts/FontAwesome.otf` & `blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__doc/themes/sphinx_rtd_theme/static/fonts/Inconsolata-Bold.ttf` & `blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/fonts/Inconsolata-Bold.ttf`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__doc/themes/sphinx_rtd_theme/static/fonts/Inconsolata-Regular.ttf` & `blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/fonts/Inconsolata-Regular.ttf`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__doc/themes/sphinx_rtd_theme/static/fonts/Lato-Bold.ttf` & `blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/fonts/Lato-Bold.ttf`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__doc/themes/sphinx_rtd_theme/static/fonts/Lato-Regular.ttf` & `blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__doc/themes/sphinx_rtd_theme/static/fonts/RobotoSlab-Bold.ttf` & `blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/fonts/RobotoSlab-Bold.ttf`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__doc/themes/sphinx_rtd_theme/static/fonts/RobotoSlab-Regular.ttf` & `blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/fonts/RobotoSlab-Regular.ttf`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.eot` & `blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.svg` & `blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.ttf` & `blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.woff` & `blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.woff2` & `blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__doc/themes/sphinx_rtd_theme/static/js/copybutton.js` & `blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/js/copybutton.js`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__doc/themes/sphinx_rtd_theme/static/js/modernizr.min.js` & `blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/js/modernizr.min.js`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__doc/themes/sphinx_rtd_theme/static/js/theme.js` & `blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/js/theme.js`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/__doc/themes/sphinx_rtd_theme/versions.html` & `blond-2.1.1/__doc/themes/sphinx_rtd_theme/versions.html`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/appveyor.yml` & `blond-2.1.1/appveyor.yml`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/__init__.py` & `blond-2.1.1/blond/__init__.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/beam/beam.py` & `blond-2.1.1/blond/beam/beam.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/beam/coasting_beam.py` & `blond-2.1.1/blond/beam/coasting_beam.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/beam/distributions.py` & `blond-2.1.1/blond/beam/distributions.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/beam/distributions_multibunch.py` & `blond-2.1.1/blond/beam/distributions_multibunch.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/beam/profile.py` & `blond-2.1.1/blond/beam/profile.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/beam/sparse_histogram.cpp` & `blond-2.1.1/blond/beam/sparse_histogram.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/beam/sparse_slices.py` & `blond-2.1.1/blond/beam/sparse_slices.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/compile.py` & `blond-2.1.1/blond/compile.py`

 * *Files 1% similar despite different names*

```diff
@@ -260,17 +260,17 @@
         elif args.gpu is not None:
             comp_capability = args.gpu
 
         print('Compiling the CUDA library for architecture {}.'.format(comp_capability))
         # Add the -arch required argument
         nvccflags += ['-arch', 'sm_{}'.format(comp_capability)]
         libname_double = os.path.join(basepath,
-                                      f'gpu/cuda_kernels/kernels_double_sm_{comp_capability}.cubin')
+                                      'gpu/cuda_kernels/kernels_double_sm_{}.cubin'.format(comp_capability))
         libname_single = os.path.join(basepath,
-                                      f'gpu/cuda_kernels/kernels_single_sm_{comp_capability}.cubin')
+                                      'gpu/cuda_kernels/kernels_single_sm_{}.cubin'.format(comp_capability))
         # we need to get the header files location
         path = cp.__file__.split('/')[:-1]  # remove __init__.py from path
         path.extend(['_core', 'include'])
 
         cupyloc = os.path.join('/'.join(path))
 
         print('cupy: ', cupyloc)
```

### Comparing `blond-2.1.0/blond/cpp_routines/beam_phase.cpp` & `blond-2.1.1/blond/cpp_routines/beam_phase.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/cpp_routines/blondmath.cpp` & `blond-2.1.1/blond/cpp_routines/blondmath.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/cpp_routines/blondmath.h` & `blond-2.1.1/blond/cpp_routines/blondmath.h`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/cpp_routines/cos.h` & `blond-2.1.1/blond/cpp_routines/cos.h`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/cpp_routines/drift.cpp` & `blond-2.1.1/blond/cpp_routines/drift.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/cpp_routines/exp.h` & `blond-2.1.1/blond/cpp_routines/exp.h`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/cpp_routines/fast_resonator.cpp` & `blond-2.1.1/blond/cpp_routines/fast_resonator.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/cpp_routines/fft.cpp` & `blond-2.1.1/blond/cpp_routines/fft.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/cpp_routines/fft.h` & `blond-2.1.1/blond/cpp_routines/fft.h`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/cpp_routines/histogram.cpp` & `blond-2.1.1/blond/cpp_routines/histogram.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/cpp_routines/kick.cpp` & `blond-2.1.1/blond/cpp_routines/kick.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/cpp_routines/libblond.so` & `blond-2.1.1/blond/cpp_routines/libblond.so`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/cpp_routines/linear_interp_kick.cpp` & `blond-2.1.1/blond/cpp_routines/linear_interp_kick.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/cpp_routines/music_track.cpp` & `blond-2.1.1/blond/cpp_routines/music_track.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/cpp_routines/sin.h` & `blond-2.1.1/blond/cpp_routines/sin.h`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/cpp_routines/sincos.h` & `blond-2.1.1/blond/cpp_routines/sincos.h`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/cpp_routines/vdtcore_common.h` & `blond-2.1.1/blond/cpp_routines/vdtcore_common.h`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/gpu/cuda_kernels/kernels_double.cu` & `blond-2.1.1/blond/gpu/cuda_kernels/kernels_double.cu`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/gpu/cuda_kernels/kernels_single.cu` & `blond-2.1.1/blond/gpu/cuda_kernels/kernels_single.cu`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/gpu/cupy_butils_wrap.py` & `blond-2.1.1/blond/gpu/cupy_butils_wrap.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/impedances/impedance.py` & `blond-2.1.1/blond/impedances/impedance.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/impedances/impedance_sources.py` & `blond-2.1.1/blond/impedances/impedance_sources.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/impedances/induced_voltage_analytical.py` & `blond-2.1.1/blond/impedances/induced_voltage_analytical.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/impedances/music.py` & `blond-2.1.1/blond/impedances/music.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/input_parameters/rf_parameters.py` & `blond-2.1.1/blond/input_parameters/rf_parameters.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/input_parameters/rf_parameters_options.py` & `blond-2.1.1/blond/input_parameters/rf_parameters_options.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/input_parameters/ring.py` & `blond-2.1.1/blond/input_parameters/ring.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/input_parameters/ring_options.py` & `blond-2.1.1/blond/input_parameters/ring_options.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/llrf/beam_feedback.py` & `blond-2.1.1/blond/llrf/beam_feedback.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/llrf/cavity_feedback.py` & `blond-2.1.1/blond/llrf/cavity_feedback.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/llrf/impulse_response.py` & `blond-2.1.1/blond/llrf/impulse_response.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/llrf/notch_filter.py` & `blond-2.1.1/blond/llrf/notch_filter.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/llrf/offset_frequency.py` & `blond-2.1.1/blond/llrf/offset_frequency.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/llrf/rf_modulation.py` & `blond-2.1.1/blond/llrf/rf_modulation.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/llrf/rf_noise.py` & `blond-2.1.1/blond/llrf/rf_noise.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/llrf/signal_processing.py` & `blond-2.1.1/blond/llrf/signal_processing.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/monitors/monitors.py` & `blond-2.1.1/blond/monitors/monitors.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/plots/plot.py` & `blond-2.1.1/blond/plots/plot.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/plots/plot_beams.py` & `blond-2.1.1/blond/plots/plot_beams.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/plots/plot_impedance.py` & `blond-2.1.1/blond/plots/plot_impedance.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/plots/plot_llrf.py` & `blond-2.1.1/blond/plots/plot_llrf.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/plots/plot_parameters.py` & `blond-2.1.1/blond/plots/plot_parameters.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/plots/plot_slices.py` & `blond-2.1.1/blond/plots/plot_slices.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/sanity_check.py` & `blond-2.1.1/blond/sanity_check.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/synchrotron_radiation/synchrotron_radiation.cpp` & `blond-2.1.1/blond/synchrotron_radiation/synchrotron_radiation.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/synchrotron_radiation/synchrotron_radiation.py` & `blond-2.1.1/blond/synchrotron_radiation/synchrotron_radiation.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/toolbox/action.py` & `blond-2.1.1/blond/toolbox/action.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/toolbox/diffusion.py` & `blond-2.1.1/blond/toolbox/diffusion.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/toolbox/filters_and_fitting.py` & `blond-2.1.1/blond/toolbox/filters_and_fitting.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/toolbox/logger.py` & `blond-2.1.1/blond/toolbox/logger.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/toolbox/next_regular.py` & `blond-2.1.1/blond/toolbox/next_regular.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/toolbox/parameter_scaling.py` & `blond-2.1.1/blond/toolbox/parameter_scaling.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/toolbox/tomoscope.cpp` & `blond-2.1.1/blond/toolbox/tomoscope.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/toolbox/tomoscope.py` & `blond-2.1.1/blond/toolbox/tomoscope.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/trackers/tracker.py` & `blond-2.1.1/blond/trackers/tracker.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/trackers/utilities.py` & `blond-2.1.1/blond/trackers/utilities.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/utils/bmath.py` & `blond-2.1.1/blond/utils/bmath.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/utils/butils_wrap.py` & `blond-2.1.1/blond/utils/butils_wrap.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/utils/data_check.py` & `blond-2.1.1/blond/utils/data_check.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/utils/exceptions.py` & `blond-2.1.1/blond/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/utils/input_parser.py` & `blond-2.1.1/blond/utils/input_parser.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/utils/mpi_config.py` & `blond-2.1.1/blond/utils/mpi_config.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/utils/profile_mock.py` & `blond-2.1.1/blond/utils/profile_mock.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond/utils/track_iteration.py` & `blond-2.1.1/blond/utils/track_iteration.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/blond.egg-info/PKG-INFO` & `blond-2.1.1/blond.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: blond
-Version: 2.1.0
+Version: 2.1.1
 Summary: CERN code for simulating longitudinal beam dynamics in synchrotrons.
 Home-page: https://gitlab.cern.ch/blond/BLonD
 Author: Helga Timko et al.
 Author-email: helga.timko@cern.ch
 Maintainer: Konstantinos Iliakis
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: core
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: all
 License-File: LICENSE.txt
```

### Comparing `blond-2.1.0/blond.egg-info/SOURCES.txt` & `blond-2.1.1/blond.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/setup.py` & `blond-2.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import os
 
 HERE = Path(__file__).parent.absolute()
 with (HERE / 'README.md').open('rt', encoding='utf-8') as fh:
     LONG_DESCRIPTION = fh.read().strip()
 
 
-REQUIREMENTS: dict = {
+REQUIREMENTS = {
     'core': ['numpy',
              'scipy',
              'h5py',
              'matplotlib',
              'mpmath'
              ],
     'test': [
@@ -53,15 +53,15 @@
         self.compiler = None
 
     def finalize_options(self):
         """Post-process options."""
         _egg_info.finalize_options(self)
 
     def run(self):
-        cmd = ['python', 'blond/compile.py']
+        cmd = ['python3', 'blond/compile.py']
         if self.parallel:
             cmd.append('-p')
         if self.boost:
             cmd += ['-b', self.boost]
         if self.compiler:
             cmd += ['-c', self.compiler]
 
@@ -87,15 +87,15 @@
 
     def finalize_options(self):
         """Post-process options."""
         pass
 
     def run(self):
         """Run command."""
-        cmd = ['python', 'blond/compile.py']
+        cmd = ['python3', 'blond/compile.py']
         if self.openmp:
             cmd.append('-p')
         if self.boost:
             cmd += ['-b', self.boost]
         if self.compiler:
             cmd += ['-c', self.compiler]
         subprocess.run(cmd, check=True, env=os.environ.copy())
@@ -110,15 +110,15 @@
     maintainer='Konstantinos Iliakis',
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     url='https://gitlab.cern.ch/blond/BLonD',
     # download_url='https://github.com/blond-admin/BLonD/archive/v'+__version__+'.tar.gz',
     packages=find_packages(
         exclude=['__doc', '__BENCHMARKS', '__EXAMPLES', 'unittests']),
-    python_requires='>=3.7',
+    python_requires='>=3.6',
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
         "Intended Audience :: Science/Research",
         "Natural Language :: English",
         "Topic :: Scientific/Engineering :: Physics"
```

### Comparing `blond-2.1.0/unittests/beam_profile/dt_coordinates.npz` & `blond-2.1.1/unittests/beam_profile/dt_coordinates.npz`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/unittests/beam_profile/test_beam_profile_object.py` & `blond-2.1.1/unittests/beam_profile/test_beam_profile_object.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/unittests/beam_profile/test_sparse_profile.py` & `blond-2.1.1/unittests/beam_profile/test_sparse_profile.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/unittests/beams/test_beam_object.py` & `blond-2.1.1/unittests/beams/test_beam_object.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/unittests/beams/test_coasting_beam.py` & `blond-2.1.1/unittests/beams/test_coasting_beam.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/unittests/general/test_separatrix_bigaussian.py` & `blond-2.1.1/unittests/general/test_separatrix_bigaussian.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/unittests/gpu/test_ffts.py` & `blond-2.1.1/unittests/gpu/test_ffts.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/unittests/gpu/test_impedance.py` & `blond-2.1.1/unittests/gpu/test_impedance.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/unittests/gpu/test_physics_kernels.py` & `blond-2.1.1/unittests/gpu/test_physics_kernels.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/unittests/impedances/test_impedance.py` & `blond-2.1.1/unittests/impedances/test_impedance.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/unittests/impedances/test_impedance_sources.py` & `blond-2.1.1/unittests/impedances/test_impedance_sources.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/unittests/input_parameters/test_preprocess.py` & `blond-2.1.1/unittests/input_parameters/test_preprocess.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/unittests/input_parameters/test_rf_params_object.py` & `blond-2.1.1/unittests/input_parameters/test_rf_params_object.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/unittests/input_parameters/test_ring.py` & `blond-2.1.1/unittests/input_parameters/test_ring.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/unittests/integration/test_examples.py` & `blond-2.1.1/unittests/integration/test_examples.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/unittests/integration/test_gpu_examples.py` & `blond-2.1.1/unittests/integration/test_gpu_examples.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/unittests/integration/test_mpi_examples.py` & `blond-2.1.1/unittests/integration/test_mpi_examples.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/unittests/integration/test_validate_gpu.py` & `blond-2.1.1/unittests/integration/test_validate_gpu.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/unittests/integration/test_validate_mpi.py` & `blond-2.1.1/unittests/integration/test_validate_mpi.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/unittests/llrf/ref_DV_MOD_FR.npy` & `blond-2.1.1/unittests/llrf/ref_DV_MOD_FR.npy`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/unittests/llrf/ref_DV_MOD_FRF.npy` & `blond-2.1.1/unittests/llrf/ref_DV_MOD_FRF.npy`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/unittests/llrf/ref_V_IND_COARSE_GEN.npy` & `blond-2.1.1/unittests/llrf/ref_V_IND_COARSE_GEN.npy`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/unittests/llrf/test_beam_feedback.py` & `blond-2.1.1/unittests/llrf/test_beam_feedback.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/unittests/llrf/test_cavity_feedback.py` & `blond-2.1.1/unittests/llrf/test_cavity_feedback.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/unittests/llrf/test_impulse_response.py` & `blond-2.1.1/unittests/llrf/test_impulse_response.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/unittests/llrf/test_offset_frequency.py` & `blond-2.1.1/unittests/llrf/test_offset_frequency.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/unittests/llrf/test_rf_modulation.py` & `blond-2.1.1/unittests/llrf/test_rf_modulation.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/unittests/llrf/test_signal_processing.py` & `blond-2.1.1/unittests/llrf/test_signal_processing.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/unittests/synchrotron_radiation/test_synch_rad.py` & `blond-2.1.1/unittests/synchrotron_radiation/test_synch_rad.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/unittests/trackers/comparison_drift.py` & `blond-2.1.1/unittests/trackers/comparison_drift.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/unittests/trackers/test_drift.py` & `blond-2.1.1/unittests/trackers/test_drift.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/unittests/trackers/test_tracker.py` & `blond-2.1.1/unittests/trackers/test_tracker.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/unittests/utils/test_blondmath.py` & `blond-2.1.1/unittests/utils/test_blondmath.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/unittests/utils/test_data_check.py` & `blond-2.1.1/unittests/utils/test_data_check.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/unittests/utils/test_ffts.py` & `blond-2.1.1/unittests/utils/test_ffts.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.0/unittests/utils/test_iteration.py` & `blond-2.1.1/unittests/utils/test_iteration.py`

 * *Files identical despite different names*

