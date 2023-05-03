# Comparing `tmp/pywhispercpp-1.0.7.tar.gz` & `tmp/pywhispercpp-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywhispercpp-1.0.7.tar", last modified: Sat Mar 25 04:02:10 2023, max compression
+gzip compressed data, was "pywhispercpp-1.0.8.tar", last modified: Wed May  3 23:10:05 2023, max compression
```

## Comparing `pywhispercpp-1.0.7.tar` & `pywhispercpp-1.0.8.tar`

### file list

```diff
@@ -1,138 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 04:02:10.815817 pywhispercpp-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14387 2023-03-25 04:02:10.811817 pywhispercpp-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 04:02:10.799816 pywhispercpp-1.0.7/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pybind11/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pybind11/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 04:02:10.795816 pywhispercpp-1.0.7/pybind11/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 04:02:10.803817 pywhispercpp-1.0.7/pybind11/include/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)    23920 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pybind11/include/pybind11/attr.h
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 runner    (1001) docker     (123)    64793 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pybind11/include/pybind11/cast.h
--rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pybind11/include/pybind11/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 04:02:10.803817 pywhispercpp-1.0.7/pybind11/include/pybind11/detail/
--rw-r--r--   0 runner    (1001) docker     (123)    28526 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 runner    (1001) docker     (123)    51655 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 runner    (1001) docker     (123)    17971 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 runner    (1001) docker     (123)    24196 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 runner    (1001) docker     (123)    44414 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pybind11/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pybind11/include/pybind11/detail/typeid.h
--rw-r--r--   0 runner    (1001) docker     (123)    31441 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 runner    (1001) docker     (123)    12175 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pybind11/include/pybind11/embed.h
--rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pybind11/include/pybind11/eval.h
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pybind11/include/pybind11/functional.h
--rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pybind11/include/pybind11/gil.h
--rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 runner    (1001) docker     (123)    78036 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 runner    (1001) docker     (123)     9781 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pybind11/include/pybind11/operators.h
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pybind11/include/pybind11/options.h
--rw-r--r--   0 runner    (1001) docker     (123)   125927 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 runner    (1001) docker     (123)    80901 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pybind11/include/pybind11/pytypes.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 04:02:10.803817 pywhispercpp-1.0.7/pybind11/include/pybind11/stl/
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pybind11/include/pybind11/stl/filesystem.h
--rw-r--r--   0 runner    (1001) docker     (123)    14438 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pybind11/include/pybind11/stl.h
--rw-r--r--   0 runner    (1001) docker     (123)    26992 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pybind11/include/pybind11/stl_bind.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 04:02:10.807817 pywhispercpp-1.0.7/pybind11/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    21095 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pybind11/tests/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 04:02:10.807817 pywhispercpp-1.0.7/pybind11/tests/test_cmake_build/
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pybind11/tests/test_cmake_build/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 04:02:10.807817 pywhispercpp-1.0.7/pybind11/tests/test_cmake_build/installed_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 04:02:10.807817 pywhispercpp-1.0.7/pybind11/tests/test_cmake_build/installed_function/
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 04:02:10.807817 pywhispercpp-1.0.7/pybind11/tests/test_cmake_build/installed_target/
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 04:02:10.807817 pywhispercpp-1.0.7/pybind11/tests/test_cmake_build/subdirectory_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 04:02:10.807817 pywhispercpp-1.0.7/pybind11/tests/test_cmake_build/subdirectory_function/
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 04:02:10.807817 pywhispercpp-1.0.7/pybind11/tests/test_cmake_build/subdirectory_target/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 04:02:10.807817 pywhispercpp-1.0.7/pybind11/tests/test_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pybind11/tests/test_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 04:02:10.807817 pywhispercpp-1.0.7/pybind11/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pybind11/tools/FindCatch.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0 runner    (1001) docker     (123)    10378 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pybind11/tools/FindPythonLibsNew.cmake
--rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pybind11/tools/check-style.sh
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pybind11/tools/cmake_uninstall.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pybind11/tools/libsize.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1306 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pybind11/tools/make_changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)    14579 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pybind11/tools/pybind11Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pybind11/tools/pybind11NewTools.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pybind11/tools/pybind11Tools.cmake
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pybind11/tools/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pybind11/tools/setup_global.py.in
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pybind11/tools/setup_main.py.in
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 04:02:10.799816 pywhispercpp-1.0.7/pywhispercpp/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pywhispercpp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pywhispercpp/_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pywhispercpp/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 04:02:10.799816 pywhispercpp-1.0.7/pywhispercpp/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pywhispercpp/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pywhispercpp/examples/assistant.py
--rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pywhispercpp/examples/livestream.py
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pywhispercpp/examples/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pywhispercpp/examples/recording.py
--rw-r--r--   0 runner    (1001) docker     (123)     9965 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pywhispercpp/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/pywhispercpp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 04:02:10.811817 pywhispercpp-1.0.7/pywhispercpp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14387 2023-03-25 04:02:10.000000 pywhispercpp-1.0.7/pywhispercpp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-03-25 04:02:10.000000 pywhispercpp-1.0.7/pywhispercpp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 04:02:10.000000 pywhispercpp-1.0.7/pywhispercpp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-03-25 04:02:10.000000 pywhispercpp-1.0.7/pywhispercpp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 04:02:10.000000 pywhispercpp-1.0.7/pywhispercpp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-03-25 04:02:10.000000 pywhispercpp-1.0.7/pywhispercpp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-25 04:02:10.000000 pywhispercpp-1.0.7/pywhispercpp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 04:02:10.815817 pywhispercpp-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 04:02:10.811817 pywhispercpp-1.0.7/src/
--rw-r--r--   0 runner    (1001) docker     (123)    26781 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/src/main.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 04:02:10.811817 pywhispercpp-1.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/tests/test_c_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-03-25 04:01:57.000000 pywhispercpp-1.0.7/tests/test_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 04:02:10.811817 pywhispercpp-1.0.7/whisper.cpp/
--rw-r--r--   0 runner    (1001) docker     (123)     7745 2023-03-25 04:01:59.000000 pywhispercpp-1.0.7/whisper.cpp/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 04:02:10.811817 pywhispercpp-1.0.7/whisper.cpp/bindings/
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-03-25 04:01:59.000000 pywhispercpp-1.0.7/whisper.cpp/bindings/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 04:02:10.811817 pywhispercpp-1.0.7/whisper.cpp/bindings/javascript/
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-03-25 04:01:59.000000 pywhispercpp-1.0.7/whisper.cpp/bindings/javascript/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 04:02:10.811817 pywhispercpp-1.0.7/whisper.cpp/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-03-25 04:01:59.000000 pywhispercpp-1.0.7/whisper.cpp/cmake/BuildTypes.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-03-25 04:01:59.000000 pywhispercpp-1.0.7/whisper.cpp/cmake/DefaultTargetOptions.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-03-25 04:01:59.000000 pywhispercpp-1.0.7/whisper.cpp/cmake/GitVars.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 04:02:10.811817 pywhispercpp-1.0.7/whisper.cpp/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-03-25 04:01:59.000000 pywhispercpp-1.0.7/whisper.cpp/examples/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 04:02:10.811817 pywhispercpp-1.0.7/whisper.cpp/examples/addon.node/
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-03-25 04:01:59.000000 pywhispercpp-1.0.7/whisper.cpp/examples/addon.node/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 04:02:10.811817 pywhispercpp-1.0.7/whisper.cpp/examples/bench/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-03-25 04:01:59.000000 pywhispercpp-1.0.7/whisper.cpp/examples/bench/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 04:02:10.811817 pywhispercpp-1.0.7/whisper.cpp/examples/bench.wasm/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-03-25 04:01:59.000000 pywhispercpp-1.0.7/whisper.cpp/examples/bench.wasm/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 04:02:10.811817 pywhispercpp-1.0.7/whisper.cpp/examples/command/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-03-25 04:01:59.000000 pywhispercpp-1.0.7/whisper.cpp/examples/command/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 04:02:10.811817 pywhispercpp-1.0.7/whisper.cpp/examples/command.wasm/
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-03-25 04:01:59.000000 pywhispercpp-1.0.7/whisper.cpp/examples/command.wasm/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 04:02:10.811817 pywhispercpp-1.0.7/whisper.cpp/examples/main/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-03-25 04:01:59.000000 pywhispercpp-1.0.7/whisper.cpp/examples/main/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 04:02:10.811817 pywhispercpp-1.0.7/whisper.cpp/examples/stream/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-03-25 04:01:59.000000 pywhispercpp-1.0.7/whisper.cpp/examples/stream/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 04:02:10.811817 pywhispercpp-1.0.7/whisper.cpp/examples/stream.wasm/
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-03-25 04:01:59.000000 pywhispercpp-1.0.7/whisper.cpp/examples/stream.wasm/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 04:02:10.811817 pywhispercpp-1.0.7/whisper.cpp/examples/talk/
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-03-25 04:01:59.000000 pywhispercpp-1.0.7/whisper.cpp/examples/talk/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 04:02:10.811817 pywhispercpp-1.0.7/whisper.cpp/examples/talk.wasm/
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-03-25 04:01:59.000000 pywhispercpp-1.0.7/whisper.cpp/examples/talk.wasm/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 04:02:10.811817 pywhispercpp-1.0.7/whisper.cpp/examples/whisper.wasm/
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-03-25 04:01:59.000000 pywhispercpp-1.0.7/whisper.cpp/examples/whisper.wasm/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 04:02:10.811817 pywhispercpp-1.0.7/whisper.cpp/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-03-25 04:01:59.000000 pywhispercpp-1.0.7/whisper.cpp/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.458759 pywhispercpp-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14525 2023-05-03 23:10:05.458759 pywhispercpp-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14074 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.434759 pywhispercpp-1.0.8/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.426759 pywhispercpp-1.0.8/pybind11/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.442759 pywhispercpp-1.0.8/pybind11/include/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)    23920 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 runner    (1001) docker     (123)    64793 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/include/pybind11/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.442759 pywhispercpp-1.0.8/pybind11/include/pybind11/detail/
+-rw-r--r--   0 runner    (1001) docker     (123)    28526 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 runner    (1001) docker     (123)    51655 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17971 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24196 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 runner    (1001) docker     (123)    44414 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/include/pybind11/detail/typeid.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31441 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12175 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 runner    (1001) docker     (123)    78036 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9781 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/include/pybind11/options.h
+-rw-r--r--   0 runner    (1001) docker     (123)   125927 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 runner    (1001) docker     (123)    80901 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/include/pybind11/pytypes.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.442759 pywhispercpp-1.0.8/pybind11/include/pybind11/stl/
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14438 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26992 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/include/pybind11/stl_bind.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.442759 pywhispercpp-1.0.8/pybind11/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    21095 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.446759 pywhispercpp-1.0.8/pybind11/tests/test_cmake_build/
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/tests/test_cmake_build/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.446759 pywhispercpp-1.0.8/pybind11/tests/test_cmake_build/installed_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.446759 pywhispercpp-1.0.8/pybind11/tests/test_cmake_build/installed_function/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.446759 pywhispercpp-1.0.8/pybind11/tests/test_cmake_build/installed_target/
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.446759 pywhispercpp-1.0.8/pybind11/tests/test_cmake_build/subdirectory_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.446759 pywhispercpp-1.0.8/pybind11/tests/test_cmake_build/subdirectory_function/
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.446759 pywhispercpp-1.0.8/pybind11/tests/test_cmake_build/subdirectory_target/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.446759 pywhispercpp-1.0.8/pybind11/tests/test_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/tests/test_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.450759 pywhispercpp-1.0.8/pybind11/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)    10378 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/tools/FindPythonLibsNew.cmake
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/tools/check-style.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/tools/cmake_uninstall.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/tools/libsize.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1306 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/tools/make_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14579 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/tools/pybind11Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/tools/pybind11Tools.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/tools/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/tools/setup_global.py.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/tools/setup_main.py.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.434759 pywhispercpp-1.0.8/pywhispercpp/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pywhispercpp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pywhispercpp/_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pywhispercpp/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.434759 pywhispercpp-1.0.8/pywhispercpp/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pywhispercpp/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pywhispercpp/examples/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pywhispercpp/examples/livestream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pywhispercpp/examples/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pywhispercpp/examples/recording.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9965 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pywhispercpp/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pywhispercpp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.450759 pywhispercpp-1.0.8/pywhispercpp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14525 2023-05-03 23:10:05.000000 pywhispercpp-1.0.8/pywhispercpp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-03 23:10:05.000000 pywhispercpp-1.0.8/pywhispercpp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 23:10:05.000000 pywhispercpp-1.0.8/pywhispercpp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-03 23:10:05.000000 pywhispercpp-1.0.8/pywhispercpp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 23:10:05.000000 pywhispercpp-1.0.8/pywhispercpp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-03 23:10:05.000000 pywhispercpp-1.0.8/pywhispercpp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-03 23:10:05.000000 pywhispercpp-1.0.8/pywhispercpp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 23:10:05.458759 pywhispercpp-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.450759 pywhispercpp-1.0.8/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    26781 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/src/main.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.454759 pywhispercpp-1.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/tests/test_c_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/tests/test_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.454759 pywhispercpp-1.0.8/whisper.cpp/
+-rw-r--r--   0 runner    (1001) docker     (123)     7745 2023-05-03 23:09:51.000000 pywhispercpp-1.0.8/whisper.cpp/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.454759 pywhispercpp-1.0.8/whisper.cpp/bindings/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-03 23:09:51.000000 pywhispercpp-1.0.8/whisper.cpp/bindings/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.454759 pywhispercpp-1.0.8/whisper.cpp/bindings/javascript/
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-03 23:09:51.000000 pywhispercpp-1.0.8/whisper.cpp/bindings/javascript/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.454759 pywhispercpp-1.0.8/whisper.cpp/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-03 23:09:51.000000 pywhispercpp-1.0.8/whisper.cpp/cmake/BuildTypes.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-03 23:09:51.000000 pywhispercpp-1.0.8/whisper.cpp/cmake/DefaultTargetOptions.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-03 23:09:51.000000 pywhispercpp-1.0.8/whisper.cpp/cmake/GitVars.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.454759 pywhispercpp-1.0.8/whisper.cpp/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-03 23:09:51.000000 pywhispercpp-1.0.8/whisper.cpp/examples/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.454759 pywhispercpp-1.0.8/whisper.cpp/examples/addon.node/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-03 23:09:51.000000 pywhispercpp-1.0.8/whisper.cpp/examples/addon.node/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.454759 pywhispercpp-1.0.8/whisper.cpp/examples/bench/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-03 23:09:51.000000 pywhispercpp-1.0.8/whisper.cpp/examples/bench/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.454759 pywhispercpp-1.0.8/whisper.cpp/examples/bench.wasm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-03 23:09:51.000000 pywhispercpp-1.0.8/whisper.cpp/examples/bench.wasm/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.454759 pywhispercpp-1.0.8/whisper.cpp/examples/command/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-03 23:09:51.000000 pywhispercpp-1.0.8/whisper.cpp/examples/command/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.454759 pywhispercpp-1.0.8/whisper.cpp/examples/command.wasm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-03 23:09:51.000000 pywhispercpp-1.0.8/whisper.cpp/examples/command.wasm/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.454759 pywhispercpp-1.0.8/whisper.cpp/examples/main/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-03 23:09:51.000000 pywhispercpp-1.0.8/whisper.cpp/examples/main/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.454759 pywhispercpp-1.0.8/whisper.cpp/examples/stream/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-03 23:09:51.000000 pywhispercpp-1.0.8/whisper.cpp/examples/stream/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.458759 pywhispercpp-1.0.8/whisper.cpp/examples/stream.wasm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-03 23:09:51.000000 pywhispercpp-1.0.8/whisper.cpp/examples/stream.wasm/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.458759 pywhispercpp-1.0.8/whisper.cpp/examples/talk/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-03 23:09:51.000000 pywhispercpp-1.0.8/whisper.cpp/examples/talk/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.458759 pywhispercpp-1.0.8/whisper.cpp/examples/talk.wasm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-03 23:09:51.000000 pywhispercpp-1.0.8/whisper.cpp/examples/talk.wasm/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.458759 pywhispercpp-1.0.8/whisper.cpp/examples/whisper.wasm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-03 23:09:51.000000 pywhispercpp-1.0.8/whisper.cpp/examples/whisper.wasm/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.458759 pywhispercpp-1.0.8/whisper.cpp/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-03 23:09:51.000000 pywhispercpp-1.0.8/whisper.cpp/tests/CMakeLists.txt
```

### Comparing `pywhispercpp-1.0.7/CMakeLists.txt` & `pywhispercpp-1.0.8/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/LICENSE` & `pywhispercpp-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/PKG-INFO` & `pywhispercpp-1.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: pywhispercpp
-Version: 1.0.7
+Version: 1.0.8
 Summary: Python bindings for whisper.cpp
 Author: abdeladim-s
 License: MIT
 Project-URL: Documentation, https://abdeladim-s.github.io/pywhispercpp/
 Project-URL: Source, https://github.com/abdeladim-s/pywhispercpp
 Project-URL: Tracker, https://github.com/abdeladim-s/pywhispercpp/issues
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: examples
 License-File: LICENSE
 
 # pywhispercpp
 Python bindings for [whisper.cpp](https://github.com/ggerganov/whisper.cpp) with a simple Pythonic API on top of it.
 
 [![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 [![Wheels](https://github.com/abdeladim-s/pywhispercpp/actions/workflows/wheels.yml/badge.svg?branch=main&event=push)](https://github.com/abdeladim-s/pywhispercpp/actions/workflows/wheels.yml)
@@ -80,14 +81,19 @@
 
 2. Once ffmpeg is installed, install `pywhispercpp`
 
 ```shell
 pip install pywhispercpp
 ```
 
+If you want to use the examples, you will need to install extra dependencies
+
+```shell
+pip install pywhispercpp[examples]
+```
 
 Or install the latest dev version from GitHub
 
 ```shell
 pip install git+https://github.com/abdeladim-s/pywhispercpp
 ```
 
@@ -328,15 +334,15 @@
   -ss SAMPLE_SIZE, --sample_size SAMPLE_SIZE
                         Sample size, default to 4
 ```
 
 # Advanced usage
 * First check the [API documentation](https://abdeladim-s.github.io/pywhispercpp/) for more advanced usage.
 * If you are a more experienced user, you can access the [C-Style API](https://github.com/ggerganov/whisper.cpp/blob/master/whisper.h) directly, almost all functions from `whisper.h`
-are exposed with the binding module `_pywhispercpp`, for example:
+are exposed with the binding module `_pywhispercpp`.
 
 ```python
 import _pywhispercpp as pwcpp
 
 ctx = pwcpp.whisper_init_from_file('path/to/ggml/model')
 ```
```

### Comparing `pywhispercpp-1.0.7/README.md` & `pywhispercpp-1.0.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,19 @@
 
 2. Once ffmpeg is installed, install `pywhispercpp`
 
 ```shell
 pip install pywhispercpp
 ```
 
+If you want to use the examples, you will need to install extra dependencies
+
+```shell
+pip install pywhispercpp[examples]
+```
 
 Or install the latest dev version from GitHub
 
 ```shell
 pip install git+https://github.com/abdeladim-s/pywhispercpp
 ```
 
@@ -315,15 +320,15 @@
   -ss SAMPLE_SIZE, --sample_size SAMPLE_SIZE
                         Sample size, default to 4
 ```
 
 # Advanced usage
 * First check the [API documentation](https://abdeladim-s.github.io/pywhispercpp/) for more advanced usage.
 * If you are a more experienced user, you can access the [C-Style API](https://github.com/ggerganov/whisper.cpp/blob/master/whisper.h) directly, almost all functions from `whisper.h`
-are exposed with the binding module `_pywhispercpp`, for example:
+are exposed with the binding module `_pywhispercpp`.
 
 ```python
 import _pywhispercpp as pwcpp
 
 ctx = pwcpp.whisper_init_from_file('path/to/ggml/model')
 ```
```

### Comparing `pywhispercpp-1.0.7/pybind11/CMakeLists.txt` & `pywhispercpp-1.0.8/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pybind11/LICENSE` & `pywhispercpp-1.0.8/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pybind11/include/pybind11/attr.h` & `pywhispercpp-1.0.8/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pybind11/include/pybind11/buffer_info.h` & `pywhispercpp-1.0.8/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pybind11/include/pybind11/cast.h` & `pywhispercpp-1.0.8/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pybind11/include/pybind11/chrono.h` & `pywhispercpp-1.0.8/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pybind11/include/pybind11/complex.h` & `pywhispercpp-1.0.8/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pybind11/include/pybind11/detail/class.h` & `pywhispercpp-1.0.8/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pybind11/include/pybind11/detail/common.h` & `pywhispercpp-1.0.8/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pybind11/include/pybind11/detail/descr.h` & `pywhispercpp-1.0.8/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pybind11/include/pybind11/detail/init.h` & `pywhispercpp-1.0.8/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pybind11/include/pybind11/detail/internals.h` & `pywhispercpp-1.0.8/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pybind11/include/pybind11/detail/type_caster_base.h` & `pywhispercpp-1.0.8/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pybind11/include/pybind11/detail/typeid.h` & `pywhispercpp-1.0.8/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pybind11/include/pybind11/eigen.h` & `pywhispercpp-1.0.8/pybind11/include/pybind11/eigen.h`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pybind11/include/pybind11/embed.h` & `pywhispercpp-1.0.8/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pybind11/include/pybind11/eval.h` & `pywhispercpp-1.0.8/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pybind11/include/pybind11/functional.h` & `pywhispercpp-1.0.8/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pybind11/include/pybind11/gil.h` & `pywhispercpp-1.0.8/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pybind11/include/pybind11/iostream.h` & `pywhispercpp-1.0.8/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pybind11/include/pybind11/numpy.h` & `pywhispercpp-1.0.8/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pybind11/include/pybind11/operators.h` & `pywhispercpp-1.0.8/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pybind11/include/pybind11/options.h` & `pywhispercpp-1.0.8/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pybind11/include/pybind11/pybind11.h` & `pywhispercpp-1.0.8/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pybind11/include/pybind11/pytypes.h` & `pywhispercpp-1.0.8/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pybind11/include/pybind11/stl/filesystem.h` & `pywhispercpp-1.0.8/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pybind11/include/pybind11/stl.h` & `pywhispercpp-1.0.8/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pybind11/include/pybind11/stl_bind.h` & `pywhispercpp-1.0.8/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pybind11/tests/CMakeLists.txt` & `pywhispercpp-1.0.8/pybind11/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pybind11/tests/test_cmake_build/CMakeLists.txt` & `pywhispercpp-1.0.8/pybind11/tests/test_cmake_build/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt` & `pywhispercpp-1.0.8/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt` & `pywhispercpp-1.0.8/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt` & `pywhispercpp-1.0.8/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt` & `pywhispercpp-1.0.8/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt` & `pywhispercpp-1.0.8/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt` & `pywhispercpp-1.0.8/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pybind11/tests/test_embed/CMakeLists.txt` & `pywhispercpp-1.0.8/pybind11/tests/test_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pybind11/tools/FindCatch.cmake` & `pywhispercpp-1.0.8/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pybind11/tools/FindEigen3.cmake` & `pywhispercpp-1.0.8/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pybind11/tools/FindPythonLibsNew.cmake` & `pywhispercpp-1.0.8/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pybind11/tools/check-style.sh` & `pywhispercpp-1.0.8/pybind11/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pybind11/tools/cmake_uninstall.cmake.in` & `pywhispercpp-1.0.8/pybind11/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pybind11/tools/libsize.py` & `pywhispercpp-1.0.8/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pybind11/tools/make_changelog.py` & `pywhispercpp-1.0.8/pybind11/tools/make_changelog.py`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pybind11/tools/pybind11Common.cmake` & `pywhispercpp-1.0.8/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pybind11/tools/pybind11Config.cmake.in` & `pywhispercpp-1.0.8/pybind11/tools/pybind11Config.cmake.in`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pybind11/tools/pybind11NewTools.cmake` & `pywhispercpp-1.0.8/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pybind11/tools/pybind11Tools.cmake` & `pywhispercpp-1.0.8/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pybind11/tools/setup_global.py.in` & `pywhispercpp-1.0.8/pybind11/tools/setup_global.py.in`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pybind11/tools/setup_main.py.in` & `pywhispercpp-1.0.8/pybind11/tools/setup_main.py.in`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pyproject.toml` & `pywhispercpp-1.0.8/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -42,16 +42,8 @@
   "PGH",  # pygrep-hooks
   "RUF",  # Ruff-specific
   "UP",   # pyupgrade
 ]
 extend-ignore = [
   "E501",   # Line too long
 ]
-target-version = "py39"
-
-# dependencies
-[project]
-name = "pywhispercpp"
-dynamic = ["dependencies", "version", "readme"]
-
-[tool.setuptools.dynamic]
-dependencies = {file = ["requirements.txt"]}
+target-version = "py39"
```

### Comparing `pywhispercpp-1.0.7/pywhispercpp/_logger.py` & `pywhispercpp-1.0.8/pywhispercpp/_logger.py`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pywhispercpp/constants.py` & `pywhispercpp-1.0.8/pywhispercpp/constants.py`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pywhispercpp/examples/assistant.py` & `pywhispercpp-1.0.8/pywhispercpp/examples/assistant.py`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pywhispercpp/examples/livestream.py` & `pywhispercpp-1.0.8/pywhispercpp/examples/livestream.py`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pywhispercpp/examples/main.py` & `pywhispercpp-1.0.8/pywhispercpp/examples/main.py`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pywhispercpp/examples/recording.py` & `pywhispercpp-1.0.8/pywhispercpp/examples/recording.py`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pywhispercpp/model.py` & `pywhispercpp-1.0.8/pywhispercpp/model.py`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pywhispercpp/utils.py` & `pywhispercpp-1.0.8/pywhispercpp/utils.py`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/pywhispercpp.egg-info/PKG-INFO` & `pywhispercpp-1.0.8/pywhispercpp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: pywhispercpp
-Version: 1.0.7
+Version: 1.0.8
 Summary: Python bindings for whisper.cpp
 Author: abdeladim-s
 License: MIT
 Project-URL: Documentation, https://abdeladim-s.github.io/pywhispercpp/
 Project-URL: Source, https://github.com/abdeladim-s/pywhispercpp
 Project-URL: Tracker, https://github.com/abdeladim-s/pywhispercpp/issues
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: examples
 License-File: LICENSE
 
 # pywhispercpp
 Python bindings for [whisper.cpp](https://github.com/ggerganov/whisper.cpp) with a simple Pythonic API on top of it.
 
 [![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 [![Wheels](https://github.com/abdeladim-s/pywhispercpp/actions/workflows/wheels.yml/badge.svg?branch=main&event=push)](https://github.com/abdeladim-s/pywhispercpp/actions/workflows/wheels.yml)
@@ -80,14 +81,19 @@
 
 2. Once ffmpeg is installed, install `pywhispercpp`
 
 ```shell
 pip install pywhispercpp
 ```
 
+If you want to use the examples, you will need to install extra dependencies
+
+```shell
+pip install pywhispercpp[examples]
+```
 
 Or install the latest dev version from GitHub
 
 ```shell
 pip install git+https://github.com/abdeladim-s/pywhispercpp
 ```
 
@@ -328,15 +334,15 @@
   -ss SAMPLE_SIZE, --sample_size SAMPLE_SIZE
                         Sample size, default to 4
 ```
 
 # Advanced usage
 * First check the [API documentation](https://abdeladim-s.github.io/pywhispercpp/) for more advanced usage.
 * If you are a more experienced user, you can access the [C-Style API](https://github.com/ggerganov/whisper.cpp/blob/master/whisper.h) directly, almost all functions from `whisper.h`
-are exposed with the binding module `_pywhispercpp`, for example:
+are exposed with the binding module `_pywhispercpp`.
 
 ```python
 import _pywhispercpp as pwcpp
 
 ctx = pwcpp.whisper_init_from_file('path/to/ggml/model')
 ```
```

### Comparing `pywhispercpp-1.0.7/pywhispercpp.egg-info/SOURCES.txt` & `pywhispercpp-1.0.8/pywhispercpp.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 CMakeLists.txt
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
-requirements.txt
 setup.py
 ./pywhispercpp/__init__.py
 ./pywhispercpp/_logger.py
 ./pywhispercpp/constants.py
 ./pywhispercpp/model.py
 ./pywhispercpp/utils.py
 ./pywhispercpp/examples/__init__.py
```

### Comparing `pywhispercpp-1.0.7/setup.py` & `pywhispercpp-1.0.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 # The information here can also be placed in setup.cfg - better separation of
 # logic and declaration, and simpler if you include description/version in a file.
 setup(
     name="pywhispercpp",
-    version="1.0.7",
+    version="1.0.8",
     author="abdeladim-s",
     description="Python bindings for whisper.cpp",
     long_description=long_description,
     ext_modules=[CMakeExtension("_pywhispercpp")],
     cmdclass={"build_ext": CMakeBuild},
     zip_safe=False,
     # extras_require={"test": ["pytest>=6.0"]},
@@ -151,8 +151,10 @@
                             'pwcpp-recording=pywhispercpp.examples.recording:_main']
     },
     project_urls={
         'Documentation': 'https://abdeladim-s.github.io/pywhispercpp/',
         'Source': 'https://github.com/abdeladim-s/pywhispercpp',
         'Tracker': 'https://github.com/abdeladim-s/pywhispercpp/issues',
     },
+    install_requires=['numpy', "pydub", "requests", "tqdm", "platformdirs"],
+    extras_require={"examples": ["sounddevice", "webrtcvad"]},
 )
```

### Comparing `pywhispercpp-1.0.7/src/main.cpp` & `pywhispercpp-1.0.8/src/main.cpp`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/tests/test_c_api.py` & `pywhispercpp-1.0.8/tests/test_c_api.py`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/tests/test_model.py` & `pywhispercpp-1.0.8/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/whisper.cpp/CMakeLists.txt` & `pywhispercpp-1.0.8/whisper.cpp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/whisper.cpp/bindings/CMakeLists.txt` & `pywhispercpp-1.0.8/whisper.cpp/bindings/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/whisper.cpp/bindings/javascript/CMakeLists.txt` & `pywhispercpp-1.0.8/whisper.cpp/bindings/javascript/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/whisper.cpp/cmake/BuildTypes.cmake` & `pywhispercpp-1.0.8/whisper.cpp/cmake/BuildTypes.cmake`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/whisper.cpp/cmake/GitVars.cmake` & `pywhispercpp-1.0.8/whisper.cpp/cmake/GitVars.cmake`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/whisper.cpp/examples/CMakeLists.txt` & `pywhispercpp-1.0.8/whisper.cpp/examples/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/whisper.cpp/examples/addon.node/CMakeLists.txt` & `pywhispercpp-1.0.8/whisper.cpp/examples/addon.node/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/whisper.cpp/examples/bench.wasm/CMakeLists.txt` & `pywhispercpp-1.0.8/whisper.cpp/examples/bench.wasm/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/whisper.cpp/examples/command.wasm/CMakeLists.txt` & `pywhispercpp-1.0.8/whisper.cpp/examples/command.wasm/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/whisper.cpp/examples/stream.wasm/CMakeLists.txt` & `pywhispercpp-1.0.8/whisper.cpp/examples/stream.wasm/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/whisper.cpp/examples/talk/CMakeLists.txt` & `pywhispercpp-1.0.8/whisper.cpp/examples/talk/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/whisper.cpp/examples/talk.wasm/CMakeLists.txt` & `pywhispercpp-1.0.8/whisper.cpp/examples/talk.wasm/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/whisper.cpp/examples/whisper.wasm/CMakeLists.txt` & `pywhispercpp-1.0.8/whisper.cpp/examples/whisper.wasm/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.7/whisper.cpp/tests/CMakeLists.txt` & `pywhispercpp-1.0.8/whisper.cpp/tests/CMakeLists.txt`

 * *Files identical despite different names*

