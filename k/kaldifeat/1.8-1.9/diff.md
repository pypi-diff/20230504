# Comparing `tmp/kaldifeat-1.8.tar.gz` & `tmp/kaldifeat-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kaldifeat-1.8.tar", last modified: Fri Oct 15 11:04:49 2021, max compression
+gzip compressed data, was "dist/kaldifeat-1.9.tar", last modified: Sun Oct 31 02:55:28 2021, max compression
```

## Comparing `kaldifeat-1.8.tar` & `kaldifeat-1.9.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 11:04:49.000000 kaldifeat-1.8/
--rw-r--r--   0 runner    (1001) docker     (121)     2044 2021-10-15 11:04:38.000000 kaldifeat-1.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-15 11:04:49.000000 kaldifeat-1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     8131 2021-10-15 11:04:38.000000 kaldifeat-1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)    11728 2021-10-15 11:04:38.000000 kaldifeat-1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      106 2021-10-15 11:04:38.000000 kaldifeat-1.8/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 11:04:49.000000 kaldifeat-1.8/cmake/
--rw-r--r--   0 runner    (1001) docker     (121)     1244 2021-10-15 11:04:38.000000 kaldifeat-1.8/cmake/torch.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     2993 2021-10-15 11:04:38.000000 kaldifeat-1.8/cmake/cmake_extension.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 11:04:38.000000 kaldifeat-1.8/cmake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      993 2021-10-15 11:04:38.000000 kaldifeat-1.8/cmake/pybind11.cmake
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 11:04:49.000000 kaldifeat-1.8/cmake/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (121)      138 2021-10-15 11:04:49.000000 kaldifeat-1.8/cmake/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 runner    (1001) docker     (121)     2851 2021-10-15 11:04:49.000000 kaldifeat-1.8/cmake/__pycache__/cmake_extension.cpython-36.pyc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 11:04:49.000000 kaldifeat-1.8/cmake/Modules/
--rw-r--r--   0 runner    (1001) docker     (121)      135 2021-10-15 11:04:38.000000 kaldifeat-1.8/cmake/Modules/README.md
--rw-r--r--   0 runner    (1001) docker     (121)    38023 2021-10-15 11:04:38.000000 kaldifeat-1.8/cmake/Modules/FetchContent.cmake
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 11:04:49.000000 kaldifeat-1.8/cmake/Modules/FetchContent/
--rw-r--r--   0 runner    (1001) docker     (121)      831 2021-10-15 11:04:38.000000 kaldifeat-1.8/cmake/Modules/FetchContent/CMakeLists.cmake.in
--rw-r--r--   0 runner    (1001) docker     (121)     2680 2021-10-15 11:04:38.000000 kaldifeat-1.8/cmake/googletest.cmake
--rw-r--r--   0 runner    (1001) docker     (121)    10915 2021-10-15 11:04:49.000000 kaldifeat-1.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 11:04:49.000000 kaldifeat-1.8/kaldifeat/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 11:04:49.000000 kaldifeat-1.8/kaldifeat/csrc/
--rw-r--r--   0 runner    (1001) docker     (121)     2125 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/csrc/feature-common-inl.h
--rw-r--r--   0 runner    (1001) docker     (121)     3011 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/csrc/feature-common.h
--rw-r--r--   0 runner    (1001) docker     (121)     4431 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/csrc/mel-computations.h
--rw-r--r--   0 runner    (1001) docker     (121)     4724 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/csrc/feature-window.h
--rw-r--r--   0 runner    (1001) docker     (121)     6070 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/csrc/feature-plp.cc
--rw-r--r--   0 runner    (1001) docker     (121)      922 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/csrc/feature-functions.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1116 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/csrc/matrix-functions.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2331 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/csrc/log.h
--rw-r--r--   0 runner    (1001) docker     (121)     2316 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/csrc/test_kaldifeat.cc
--rw-r--r--   0 runner    (1001) docker     (121)     7048 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/csrc/pitch-functions.h
--rw-r--r--   0 runner    (1001) docker     (121)     1238 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/csrc/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2510 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/csrc/feature-spectrogram.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2445 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/csrc/feature-window-test.cc
--rw-r--r--   0 runner    (1001) docker     (121)     5377 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/csrc/feature-mfcc.cc
--rw-r--r--   0 runner    (1001) docker     (121)      916 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/csrc/matrix-functions.h
--rw-r--r--   0 runner    (1001) docker     (121)     3981 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/csrc/feature-plp.h
--rw-r--r--   0 runner    (1001) docker     (121)     7159 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/csrc/feature-window.cc
--rw-r--r--   0 runner    (1001) docker     (121)     3125 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/csrc/feature-fbank.h
--rw-r--r--   0 runner    (1001) docker     (121)    12619 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/csrc/mel-computations.cc
--rw-r--r--   0 runner    (1001) docker     (121)     3922 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/csrc/feature-fbank.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2636 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/csrc/feature-spectrogram.h
--rw-r--r--   0 runner    (1001) docker     (121)      453 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/csrc/feature-functions.h
--rw-r--r--   0 runner    (1001) docker     (121)     3428 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/csrc/feature-mfcc.h
--rw-r--r--   0 runner    (1001) docker     (121)       48 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 11:04:49.000000 kaldifeat-1.8/kaldifeat/python/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 11:04:49.000000 kaldifeat-1.8/kaldifeat/python/csrc/
--rw-r--r--   0 runner    (1001) docker     (121)      812 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/python/csrc/kaldifeat.cc
--rw-r--r--   0 runner    (1001) docker     (121)       27 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/python/csrc/CPPLINT.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      410 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/python/csrc/mel-computations.h
--rw-r--r--   0 runner    (1001) docker     (121)      400 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/python/csrc/feature-window.h
--rw-r--r--   0 runner    (1001) docker     (121)     2233 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/python/csrc/feature-plp.cc
--rw-r--r--   0 runner    (1001) docker     (121)      457 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/python/csrc/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      324 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/python/csrc/kaldifeat.h
--rw-r--r--   0 runner    (1001) docker     (121)     1978 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/python/csrc/feature-spectrogram.cc
--rw-r--r--   0 runner    (1001) docker     (121)     5909 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/python/csrc/utils.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1546 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/python/csrc/utils.h
--rw-r--r--   0 runner    (1001) docker     (121)     2060 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/python/csrc/feature-mfcc.cc
--rw-r--r--   0 runner    (1001) docker     (121)      385 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/python/csrc/feature-plp.h
--rw-r--r--   0 runner    (1001) docker     (121)     2500 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/python/csrc/feature-window.cc
--rw-r--r--   0 runner    (1001) docker     (121)      395 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/python/csrc/feature-fbank.h
--rw-r--r--   0 runner    (1001) docker     (121)     1247 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/python/csrc/mel-computations.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2079 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/python/csrc/feature-fbank.cc
--rw-r--r--   0 runner    (1001) docker     (121)      425 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/python/csrc/feature-spectrogram.h
--rw-r--r--   0 runner    (1001) docker     (121)      390 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/python/csrc/feature-mfcc.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 11:04:49.000000 kaldifeat-1.8/kaldifeat/python/kaldifeat/
--rw-r--r--   0 runner    (1001) docker     (121)      293 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/python/kaldifeat/mfcc.py
--rw-r--r--   0 runner    (1001) docker     (121)      314 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/python/kaldifeat/spectrogram.py
--rw-r--r--   0 runner    (1001) docker     (121)      296 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/python/kaldifeat/fbank.py
--rw-r--r--   0 runner    (1001) docker     (121)      291 2021-10-15 11:04:49.000000 kaldifeat-1.8/kaldifeat/python/kaldifeat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5283 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/python/kaldifeat/offline_feature.py
--rw-r--r--   0 runner    (1001) docker     (121)      290 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/python/kaldifeat/plp.py
--rw-r--r--   0 runner    (1001) docker     (121)       47 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/python/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 11:04:49.000000 kaldifeat-1.8/kaldifeat/python/tests/
--rwxr-xr-x   0 runner    (1001) docker     (121)     4889 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/python/tests/test_fbank.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5275 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/python/tests/test_mfcc_options.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2052 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/python/tests/test_plp.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5591 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/python/tests/test_plp_options.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5215 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/python/tests/test_fbank_options.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2585 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/python/tests/test_frame_extraction_options.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/python/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 11:04:49.000000 kaldifeat-1.8/kaldifeat/python/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (121)    14887 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/python/tests/test_data/test-mfcc-no-snip-edges.txt
--rw-r--r--   0 runner    (1001) docker     (121)    16044 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/python/tests/test_data/test2.wav
--rw-r--r--   0 runner    (1001) docker     (121)    24351 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/python/tests/test_data/test.txt
--rw-r--r--   0 runner    (1001) docker     (121)    15398 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/python/tests/test_data/test-plp-no-snip-edges.txt
--rw-r--r--   0 runner    (1001) docker     (121)    15164 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/python/tests/test_data/test-plp.txt
--rw-r--r--   0 runner    (1001) docker     (121)    25404 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/python/tests/test_data/test-with-energy.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/python/tests/test_data/test.scp
--rw-r--r--   0 runner    (1001) docker     (121)    42919 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/python/tests/test_data/test-40-no-snip-edges.txt
--rw-r--r--   0 runner    (1001) docker     (121)    11664 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/python/tests/test_data/test-plp-htk-10-ceps.txt
--rw-r--r--   0 runner    (1001) docker     (121)   274722 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/python/tests/test_data/test-spectrogram-no-snip-edges.txt
--rw-r--r--   0 runner    (1001) docker     (121)    42197 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/python/tests/test_data/test-40.txt
--rw-r--r--   0 runner    (1001) docker     (121)    25404 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/python/tests/test_data/test-htk.txt
--rw-r--r--   0 runner    (1001) docker     (121)    38444 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/python/tests/test_data/test.wav
--rw-r--r--   0 runner    (1001) docker     (121)   270114 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/python/tests/test_data/test-spectrogram.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)     2345 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/python/tests/test_data/run.sh
--rw-r--r--   0 runner    (1001) docker     (121)    14669 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/python/tests/test_data/test-mfcc.txt
--rw-r--r--   0 runner    (1001) docker     (121)      838 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/python/tests/CMakeLists.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)     3667 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/python/tests/test_spectrogram_options.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2021 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/python/tests/test_mel_bank_options.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1446 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/python/tests/test_mfcc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1439 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/python/tests/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1730 2021-10-15 11:04:38.000000 kaldifeat-1.8/kaldifeat/python/tests/test_spectrogram.py
--rw-r--r--   0 runner    (1001) docker     (121)     1330 2021-10-15 11:04:38.000000 kaldifeat-1.8/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 11:04:49.000000 kaldifeat-1.8/kaldifeat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)       21 2021-10-15 11:04:49.000000 kaldifeat-1.8/kaldifeat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3556 2021-10-15 11:04:49.000000 kaldifeat-1.8/kaldifeat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)    10915 2021-10-15 11:04:49.000000 kaldifeat-1.8/kaldifeat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-15 11:04:49.000000 kaldifeat-1.8/kaldifeat.egg-info/dependency_links.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-31 02:55:28.000000 kaldifeat-1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     2044 2021-10-31 02:55:18.000000 kaldifeat-1.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-31 02:55:28.000000 kaldifeat-1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     8131 2021-10-31 02:55:18.000000 kaldifeat-1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)    11728 2021-10-31 02:55:18.000000 kaldifeat-1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      106 2021-10-31 02:55:18.000000 kaldifeat-1.9/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-31 02:55:28.000000 kaldifeat-1.9/cmake/
+-rw-r--r--   0 runner    (1001) docker     (121)     1244 2021-10-31 02:55:18.000000 kaldifeat-1.9/cmake/torch.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     2993 2021-10-31 02:55:18.000000 kaldifeat-1.9/cmake/cmake_extension.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-31 02:55:18.000000 kaldifeat-1.9/cmake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      993 2021-10-31 02:55:18.000000 kaldifeat-1.9/cmake/pybind11.cmake
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-31 02:55:28.000000 kaldifeat-1.9/cmake/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (121)      138 2021-10-31 02:55:27.000000 kaldifeat-1.9/cmake/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 runner    (1001) docker     (121)     2851 2021-10-31 02:55:27.000000 kaldifeat-1.9/cmake/__pycache__/cmake_extension.cpython-36.pyc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-31 02:55:28.000000 kaldifeat-1.9/cmake/Modules/
+-rw-r--r--   0 runner    (1001) docker     (121)      135 2021-10-31 02:55:18.000000 kaldifeat-1.9/cmake/Modules/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)    38023 2021-10-31 02:55:18.000000 kaldifeat-1.9/cmake/Modules/FetchContent.cmake
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-31 02:55:28.000000 kaldifeat-1.9/cmake/Modules/FetchContent/
+-rw-r--r--   0 runner    (1001) docker     (121)      831 2021-10-31 02:55:18.000000 kaldifeat-1.9/cmake/Modules/FetchContent/CMakeLists.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (121)     2680 2021-10-31 02:55:18.000000 kaldifeat-1.9/cmake/googletest.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)    10915 2021-10-31 02:55:28.000000 kaldifeat-1.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-31 02:55:28.000000 kaldifeat-1.9/kaldifeat/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-31 02:55:28.000000 kaldifeat-1.9/kaldifeat/csrc/
+-rw-r--r--   0 runner    (1001) docker     (121)     2125 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/csrc/feature-common-inl.h
+-rw-r--r--   0 runner    (1001) docker     (121)     3011 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/csrc/feature-common.h
+-rw-r--r--   0 runner    (1001) docker     (121)     4431 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/csrc/mel-computations.h
+-rw-r--r--   0 runner    (1001) docker     (121)     4724 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/csrc/feature-window.h
+-rw-r--r--   0 runner    (1001) docker     (121)     6070 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/csrc/feature-plp.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      922 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/csrc/feature-functions.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1116 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/csrc/matrix-functions.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2331 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/csrc/log.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2316 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/csrc/test_kaldifeat.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     7048 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/csrc/pitch-functions.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1238 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/csrc/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2510 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/csrc/feature-spectrogram.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2445 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/csrc/feature-window-test.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     5377 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/csrc/feature-mfcc.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      916 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/csrc/matrix-functions.h
+-rw-r--r--   0 runner    (1001) docker     (121)     3981 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/csrc/feature-plp.h
+-rw-r--r--   0 runner    (1001) docker     (121)     7159 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/csrc/feature-window.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     3125 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/csrc/feature-fbank.h
+-rw-r--r--   0 runner    (1001) docker     (121)    12619 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/csrc/mel-computations.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     3922 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/csrc/feature-fbank.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2636 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/csrc/feature-spectrogram.h
+-rw-r--r--   0 runner    (1001) docker     (121)      453 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/csrc/feature-functions.h
+-rw-r--r--   0 runner    (1001) docker     (121)     3428 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/csrc/feature-mfcc.h
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-31 02:55:28.000000 kaldifeat-1.9/kaldifeat/python/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-31 02:55:28.000000 kaldifeat-1.9/kaldifeat/python/csrc/
+-rw-r--r--   0 runner    (1001) docker     (121)      812 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/python/csrc/kaldifeat.cc
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/python/csrc/CPPLINT.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      410 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/python/csrc/mel-computations.h
+-rw-r--r--   0 runner    (1001) docker     (121)      400 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/python/csrc/feature-window.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2233 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/python/csrc/feature-plp.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      457 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/python/csrc/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      324 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/python/csrc/kaldifeat.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1978 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/python/csrc/feature-spectrogram.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     5909 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/python/csrc/utils.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1546 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/python/csrc/utils.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2060 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/python/csrc/feature-mfcc.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      385 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/python/csrc/feature-plp.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2500 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/python/csrc/feature-window.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      395 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/python/csrc/feature-fbank.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1247 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/python/csrc/mel-computations.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2079 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/python/csrc/feature-fbank.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      425 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/python/csrc/feature-spectrogram.h
+-rw-r--r--   0 runner    (1001) docker     (121)      390 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/python/csrc/feature-mfcc.h
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-31 02:55:28.000000 kaldifeat-1.9/kaldifeat/python/kaldifeat/
+-rw-r--r--   0 runner    (1001) docker     (121)      293 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/python/kaldifeat/mfcc.py
+-rw-r--r--   0 runner    (1001) docker     (121)      314 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/python/kaldifeat/spectrogram.py
+-rw-r--r--   0 runner    (1001) docker     (121)      296 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/python/kaldifeat/fbank.py
+-rw-r--r--   0 runner    (1001) docker     (121)      291 2021-10-31 02:55:27.000000 kaldifeat-1.9/kaldifeat/python/kaldifeat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5283 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/python/kaldifeat/offline_feature.py
+-rw-r--r--   0 runner    (1001) docker     (121)      290 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/python/kaldifeat/plp.py
+-rw-r--r--   0 runner    (1001) docker     (121)       84 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/python/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-31 02:55:28.000000 kaldifeat-1.9/kaldifeat/python/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4889 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/python/tests/test_fbank.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5275 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/python/tests/test_mfcc_options.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2052 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/python/tests/test_plp.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5591 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/python/tests/test_plp_options.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5215 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/python/tests/test_fbank_options.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2585 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/python/tests/test_frame_extraction_options.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/python/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-31 02:55:28.000000 kaldifeat-1.9/kaldifeat/python/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (121)    14887 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/python/tests/test_data/test-mfcc-no-snip-edges.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    16044 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/python/tests/test_data/test2.wav
+-rw-r--r--   0 runner    (1001) docker     (121)    24351 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/python/tests/test_data/test.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    15398 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/python/tests/test_data/test-plp-no-snip-edges.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    15164 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/python/tests/test_data/test-plp.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    25404 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/python/tests/test_data/test-with-energy.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/python/tests/test_data/test.scp
+-rw-r--r--   0 runner    (1001) docker     (121)    42919 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/python/tests/test_data/test-40-no-snip-edges.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    11664 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/python/tests/test_data/test-plp-htk-10-ceps.txt
+-rw-r--r--   0 runner    (1001) docker     (121)   274722 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/python/tests/test_data/test-spectrogram-no-snip-edges.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    42197 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/python/tests/test_data/test-40.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    25404 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/python/tests/test_data/test-htk.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    38444 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/python/tests/test_data/test.wav
+-rw-r--r--   0 runner    (1001) docker     (121)   270114 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/python/tests/test_data/test-spectrogram.txt
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2345 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/python/tests/test_data/run.sh
+-rw-r--r--   0 runner    (1001) docker     (121)    14669 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/python/tests/test_data/test-mfcc.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      838 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/python/tests/CMakeLists.txt
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3667 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/python/tests/test_spectrogram_options.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2021 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/python/tests/test_mel_bank_options.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1446 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/python/tests/test_mfcc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1439 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/python/tests/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1730 2021-10-31 02:55:18.000000 kaldifeat-1.9/kaldifeat/python/tests/test_spectrogram.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1330 2021-10-31 02:55:18.000000 kaldifeat-1.9/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-31 02:55:28.000000 kaldifeat-1.9/kaldifeat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2021-10-31 02:55:27.000000 kaldifeat-1.9/kaldifeat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3556 2021-10-31 02:55:27.000000 kaldifeat-1.9/kaldifeat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    10915 2021-10-31 02:55:27.000000 kaldifeat-1.9/kaldifeat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-31 02:55:27.000000 kaldifeat-1.9/kaldifeat.egg-info/dependency_links.txt
```

### Comparing `kaldifeat-1.8/setup.py` & `kaldifeat-1.9/setup.py`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/README.md` & `kaldifeat-1.9/README.md`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/LICENSE` & `kaldifeat-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/cmake/torch.cmake` & `kaldifeat-1.9/cmake/torch.cmake`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/cmake/cmake_extension.py` & `kaldifeat-1.9/cmake/cmake_extension.py`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/cmake/pybind11.cmake` & `kaldifeat-1.9/cmake/pybind11.cmake`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/cmake/__pycache__/cmake_extension.cpython-36.pyc` & `kaldifeat-1.9/cmake/__pycache__/cmake_extension.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 330d 0d0a 4660 6961 b10b 0000 e300 0000  3...F`ia........
+00000000: 330d 0d0a 9605 7e61 b10b 0000 e300 0000  3.....~a........
 00000010: 0000 0000 0000 0000 000c 0000 0040 0000  .............@..
 00000020: 0073 b600 0000 6400 6401 6c00 5a00 6400  .s....d.d.l.Z.d.
 00000030: 6401 6c01 5a01 6400 6401 6c02 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c03 5a03 6400 6401 6c04 5a04 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6402 6c05 6d06 5a06 0100 6400 6401 6c07  d.l.m.Z...d.d.l.
 00000060: 5a07 6400 6403 6c08 6d09 5a09 0100 6404  Z.d.d.l.m.Z...d.
 00000070: 6405 8400 5a0a 6406 6407 8400 5a0b 7920  d...Z.d.d...Z.y
```

### Comparing `kaldifeat-1.8/cmake/Modules/FetchContent.cmake` & `kaldifeat-1.9/cmake/Modules/FetchContent.cmake`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/cmake/Modules/FetchContent/CMakeLists.cmake.in` & `kaldifeat-1.9/cmake/Modules/FetchContent/CMakeLists.cmake.in`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/cmake/googletest.cmake` & `kaldifeat-1.9/cmake/googletest.cmake`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/PKG-INFO` & `kaldifeat-1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaldifeat
-Version: 1.8
+Version: 1.9
 Summary: UNKNOWN
 Home-page: https://github.com/csukuangfj/kaldifeat
 Author: Fangjun Kuang
 Author-email: csukuangfj@gmail.com
 License: Apache licensed, as found in the LICENSE file
 Description: # kaldifeat
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kaldifeat Version: 1.8 Summary: UNKNOWN Home-page:
+Metadata-Version: 2.1 Name: kaldifeat Version: 1.9 Summary: UNKNOWN Home-page:
 https://github.com/csukuangfj/kaldifeat Author: Fangjun Kuang Author-email:
 csukuangfj@gmail.com License: Apache licensed, as found in the LICENSE file
 Description: # kaldifeat
 [/doc/source/images/os.svg] [/doc/source/images/python-3.6_3.7_3.8-blue.svg] [/
 doc/source/images/pytorch-1.6.0_1.7.0_1.7.1_1.8.0_1.8.1_1.9.0-green.svg] [/doc/
               source/images/cuda-10.1_10.2_11.0_11.1-orange.svg]
 Comments    Options                      Feature Computer      Usage
```

### Comparing `kaldifeat-1.8/kaldifeat/csrc/feature-common-inl.h` & `kaldifeat-1.9/kaldifeat/csrc/feature-common-inl.h`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/csrc/feature-common.h` & `kaldifeat-1.9/kaldifeat/csrc/feature-common.h`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/csrc/mel-computations.h` & `kaldifeat-1.9/kaldifeat/csrc/mel-computations.h`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/csrc/feature-window.h` & `kaldifeat-1.9/kaldifeat/csrc/feature-window.h`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/csrc/feature-plp.cc` & `kaldifeat-1.9/kaldifeat/csrc/feature-plp.cc`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/csrc/feature-functions.cc` & `kaldifeat-1.9/kaldifeat/csrc/feature-functions.cc`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/csrc/matrix-functions.cc` & `kaldifeat-1.9/kaldifeat/csrc/matrix-functions.cc`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/csrc/log.h` & `kaldifeat-1.9/kaldifeat/csrc/log.h`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/csrc/test_kaldifeat.cc` & `kaldifeat-1.9/kaldifeat/csrc/test_kaldifeat.cc`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/csrc/pitch-functions.h` & `kaldifeat-1.9/kaldifeat/csrc/pitch-functions.h`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/csrc/CMakeLists.txt` & `kaldifeat-1.9/kaldifeat/csrc/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/csrc/feature-spectrogram.cc` & `kaldifeat-1.9/kaldifeat/csrc/feature-spectrogram.cc`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/csrc/feature-window-test.cc` & `kaldifeat-1.9/kaldifeat/csrc/feature-window-test.cc`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/csrc/feature-mfcc.cc` & `kaldifeat-1.9/kaldifeat/csrc/feature-mfcc.cc`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/csrc/matrix-functions.h` & `kaldifeat-1.9/kaldifeat/csrc/matrix-functions.h`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/csrc/feature-plp.h` & `kaldifeat-1.9/kaldifeat/csrc/feature-plp.h`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/csrc/feature-window.cc` & `kaldifeat-1.9/kaldifeat/csrc/feature-window.cc`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/csrc/feature-fbank.h` & `kaldifeat-1.9/kaldifeat/csrc/feature-fbank.h`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/csrc/mel-computations.cc` & `kaldifeat-1.9/kaldifeat/csrc/mel-computations.cc`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/csrc/feature-fbank.cc` & `kaldifeat-1.9/kaldifeat/csrc/feature-fbank.cc`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/csrc/feature-spectrogram.h` & `kaldifeat-1.9/kaldifeat/csrc/feature-spectrogram.h`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/csrc/feature-mfcc.h` & `kaldifeat-1.9/kaldifeat/csrc/feature-mfcc.h`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/python/csrc/kaldifeat.cc` & `kaldifeat-1.9/kaldifeat/python/csrc/kaldifeat.cc`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/python/csrc/feature-plp.cc` & `kaldifeat-1.9/kaldifeat/python/csrc/feature-plp.cc`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/python/csrc/feature-spectrogram.cc` & `kaldifeat-1.9/kaldifeat/python/csrc/feature-spectrogram.cc`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/python/csrc/utils.cc` & `kaldifeat-1.9/kaldifeat/python/csrc/utils.cc`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/python/csrc/utils.h` & `kaldifeat-1.9/kaldifeat/python/csrc/utils.h`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/python/csrc/feature-mfcc.cc` & `kaldifeat-1.9/kaldifeat/python/csrc/feature-mfcc.cc`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/python/csrc/feature-window.cc` & `kaldifeat-1.9/kaldifeat/python/csrc/feature-window.cc`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/python/csrc/mel-computations.cc` & `kaldifeat-1.9/kaldifeat/python/csrc/mel-computations.cc`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/python/csrc/feature-fbank.cc` & `kaldifeat-1.9/kaldifeat/python/csrc/feature-fbank.cc`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/python/kaldifeat/offline_feature.py` & `kaldifeat-1.9/kaldifeat/python/kaldifeat/offline_feature.py`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/python/tests/test_fbank.py` & `kaldifeat-1.9/kaldifeat/python/tests/test_fbank.py`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/python/tests/test_mfcc_options.py` & `kaldifeat-1.9/kaldifeat/python/tests/test_mfcc_options.py`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/python/tests/test_plp.py` & `kaldifeat-1.9/kaldifeat/python/tests/test_plp.py`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/python/tests/test_plp_options.py` & `kaldifeat-1.9/kaldifeat/python/tests/test_plp_options.py`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/python/tests/test_fbank_options.py` & `kaldifeat-1.9/kaldifeat/python/tests/test_fbank_options.py`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/python/tests/test_frame_extraction_options.py` & `kaldifeat-1.9/kaldifeat/python/tests/test_frame_extraction_options.py`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/python/tests/test_data/test-mfcc-no-snip-edges.txt` & `kaldifeat-1.9/kaldifeat/python/tests/test_data/test-mfcc-no-snip-edges.txt`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/python/tests/test_data/test2.wav` & `kaldifeat-1.9/kaldifeat/python/tests/test_data/test2.wav`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/python/tests/test_data/test.txt` & `kaldifeat-1.9/kaldifeat/python/tests/test_data/test.txt`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/python/tests/test_data/test-plp-no-snip-edges.txt` & `kaldifeat-1.9/kaldifeat/python/tests/test_data/test-plp-no-snip-edges.txt`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/python/tests/test_data/test-plp.txt` & `kaldifeat-1.9/kaldifeat/python/tests/test_data/test-plp.txt`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/python/tests/test_data/test-with-energy.txt` & `kaldifeat-1.9/kaldifeat/python/tests/test_data/test-with-energy.txt`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/python/tests/test_data/test-40-no-snip-edges.txt` & `kaldifeat-1.9/kaldifeat/python/tests/test_data/test-40-no-snip-edges.txt`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/python/tests/test_data/test-plp-htk-10-ceps.txt` & `kaldifeat-1.9/kaldifeat/python/tests/test_data/test-plp-htk-10-ceps.txt`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/python/tests/test_data/test-spectrogram-no-snip-edges.txt` & `kaldifeat-1.9/kaldifeat/python/tests/test_data/test-spectrogram-no-snip-edges.txt`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/python/tests/test_data/test-40.txt` & `kaldifeat-1.9/kaldifeat/python/tests/test_data/test-40.txt`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/python/tests/test_data/test-htk.txt` & `kaldifeat-1.9/kaldifeat/python/tests/test_data/test-htk.txt`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/python/tests/test_data/test.wav` & `kaldifeat-1.9/kaldifeat/python/tests/test_data/test.wav`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/python/tests/test_data/test-spectrogram.txt` & `kaldifeat-1.9/kaldifeat/python/tests/test_data/test-spectrogram.txt`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/python/tests/test_data/run.sh` & `kaldifeat-1.9/kaldifeat/python/tests/test_data/run.sh`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/python/tests/test_data/test-mfcc.txt` & `kaldifeat-1.9/kaldifeat/python/tests/test_data/test-mfcc.txt`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/python/tests/CMakeLists.txt` & `kaldifeat-1.9/kaldifeat/python/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/python/tests/test_spectrogram_options.py` & `kaldifeat-1.9/kaldifeat/python/tests/test_spectrogram_options.py`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/python/tests/test_mel_bank_options.py` & `kaldifeat-1.9/kaldifeat/python/tests/test_mel_bank_options.py`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/python/tests/test_mfcc.py` & `kaldifeat-1.9/kaldifeat/python/tests/test_mfcc.py`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/python/tests/utils.py` & `kaldifeat-1.9/kaldifeat/python/tests/utils.py`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat/python/tests/test_spectrogram.py` & `kaldifeat-1.9/kaldifeat/python/tests/test_spectrogram.py`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/CMakeLists.txt` & `kaldifeat-1.9/CMakeLists.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 cmake_minimum_required(VERSION 3.8 FATAL_ERROR)
 
 project(kaldifeat)
 
 # remember to change the version in
 # scripts/conda/kaldifeat/meta.yaml
-set(kaldifeat_VERSION "1.8")
+set(kaldifeat_VERSION "1.9")
 
 set(CMAKE_ARCHIVE_OUTPUT_DIRECTORY "${CMAKE_BINARY_DIR}/lib")
 set(CMAKE_LIBRARY_OUTPUT_DIRECTORY "${CMAKE_BINARY_DIR}/lib")
 set(CMAKE_RUNTIME_OUTPUT_DIRECTORY "${CMAKE_BINARY_DIR}/bin")
 
 set(CMAKE_SKIP_BUILD_RPATH FALSE)
 set(BUILD_RPATH_USE_ORIGIN TRUE)
```

### Comparing `kaldifeat-1.8/kaldifeat.egg-info/SOURCES.txt` & `kaldifeat-1.9/kaldifeat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kaldifeat-1.8/kaldifeat.egg-info/PKG-INFO` & `kaldifeat-1.9/kaldifeat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaldifeat
-Version: 1.8
+Version: 1.9
 Summary: UNKNOWN
 Home-page: https://github.com/csukuangfj/kaldifeat
 Author: Fangjun Kuang
 Author-email: csukuangfj@gmail.com
 License: Apache licensed, as found in the LICENSE file
 Description: # kaldifeat
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kaldifeat Version: 1.8 Summary: UNKNOWN Home-page:
+Metadata-Version: 2.1 Name: kaldifeat Version: 1.9 Summary: UNKNOWN Home-page:
 https://github.com/csukuangfj/kaldifeat Author: Fangjun Kuang Author-email:
 csukuangfj@gmail.com License: Apache licensed, as found in the LICENSE file
 Description: # kaldifeat
 [/doc/source/images/os.svg] [/doc/source/images/python-3.6_3.7_3.8-blue.svg] [/
 doc/source/images/pytorch-1.6.0_1.7.0_1.7.1_1.8.0_1.8.1_1.9.0-green.svg] [/doc/
               source/images/cuda-10.1_10.2_11.0_11.1-orange.svg]
 Comments    Options                      Feature Computer      Usage
```

