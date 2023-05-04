# Comparing `tmp/pyllamacpp-2.1.1.tar.gz` & `tmp/pyllamacpp-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyllamacpp-2.1.1.tar", last modified: Tue May  2 03:55:02 2023, max compression
+gzip compressed data, was "pyllamacpp-2.1.2.tar", last modified: Thu May  4 03:40:06 2023, max compression
```

## Comparing `pyllamacpp-2.1.1.tar` & `pyllamacpp-2.1.2.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:55:02.022273 pyllamacpp-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6783 2023-05-02 03:55:02.022273 pyllamacpp-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6363 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:55:02.006273 pyllamacpp-2.1.1/llama.cpp/
--rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-05-02 03:54:51.000000 pyllamacpp-2.1.1/llama.cpp/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:55:02.006273 pyllamacpp-2.1.1/llama.cpp/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-02 03:54:51.000000 pyllamacpp-2.1.1/llama.cpp/examples/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:55:02.006273 pyllamacpp-2.1.1/llama.cpp/examples/embedding/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-02 03:54:51.000000 pyllamacpp-2.1.1/llama.cpp/examples/embedding/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:55:02.006273 pyllamacpp-2.1.1/llama.cpp/examples/main/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-02 03:54:51.000000 pyllamacpp-2.1.1/llama.cpp/examples/main/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:55:02.006273 pyllamacpp-2.1.1/llama.cpp/examples/perplexity/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-02 03:54:51.000000 pyllamacpp-2.1.1/llama.cpp/examples/perplexity/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:55:02.006273 pyllamacpp-2.1.1/llama.cpp/examples/quantize/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-02 03:54:51.000000 pyllamacpp-2.1.1/llama.cpp/examples/quantize/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:55:02.006273 pyllamacpp-2.1.1/llama.cpp/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-02 03:54:51.000000 pyllamacpp-2.1.1/llama.cpp/tests/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:55:02.006273 pyllamacpp-2.1.1/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pybind11/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pybind11/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:55:02.002273 pyllamacpp-2.1.1/pybind11/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:55:02.014273 pyllamacpp-2.1.1/pybind11/include/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)    23920 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pybind11/include/pybind11/attr.h
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 runner    (1001) docker     (123)    64793 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pybind11/include/pybind11/cast.h
--rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pybind11/include/pybind11/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:55:02.018273 pyllamacpp-2.1.1/pybind11/include/pybind11/detail/
--rw-r--r--   0 runner    (1001) docker     (123)    28526 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 runner    (1001) docker     (123)    51655 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 runner    (1001) docker     (123)    17971 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 runner    (1001) docker     (123)    24196 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 runner    (1001) docker     (123)    44414 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pybind11/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pybind11/include/pybind11/detail/typeid.h
--rw-r--r--   0 runner    (1001) docker     (123)    31441 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 runner    (1001) docker     (123)    12175 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pybind11/include/pybind11/embed.h
--rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pybind11/include/pybind11/eval.h
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pybind11/include/pybind11/functional.h
--rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pybind11/include/pybind11/gil.h
--rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 runner    (1001) docker     (123)    78036 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 runner    (1001) docker     (123)     9781 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pybind11/include/pybind11/operators.h
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pybind11/include/pybind11/options.h
--rw-r--r--   0 runner    (1001) docker     (123)   125927 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 runner    (1001) docker     (123)    80901 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pybind11/include/pybind11/pytypes.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:55:02.022273 pyllamacpp-2.1.1/pybind11/include/pybind11/stl/
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pybind11/include/pybind11/stl/filesystem.h
--rw-r--r--   0 runner    (1001) docker     (123)    14438 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pybind11/include/pybind11/stl.h
--rw-r--r--   0 runner    (1001) docker     (123)    26992 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pybind11/include/pybind11/stl_bind.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:55:02.022273 pyllamacpp-2.1.1/pybind11/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    21095 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pybind11/tests/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:55:02.022273 pyllamacpp-2.1.1/pybind11/tests/test_cmake_build/
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pybind11/tests/test_cmake_build/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:55:02.022273 pyllamacpp-2.1.1/pybind11/tests/test_cmake_build/installed_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:55:02.022273 pyllamacpp-2.1.1/pybind11/tests/test_cmake_build/installed_function/
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:55:02.022273 pyllamacpp-2.1.1/pybind11/tests/test_cmake_build/installed_target/
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:55:02.022273 pyllamacpp-2.1.1/pybind11/tests/test_cmake_build/subdirectory_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:55:02.022273 pyllamacpp-2.1.1/pybind11/tests/test_cmake_build/subdirectory_function/
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:55:02.022273 pyllamacpp-2.1.1/pybind11/tests/test_cmake_build/subdirectory_target/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:55:02.022273 pyllamacpp-2.1.1/pybind11/tests/test_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pybind11/tests/test_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:55:02.022273 pyllamacpp-2.1.1/pybind11/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pybind11/tools/FindCatch.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0 runner    (1001) docker     (123)    10378 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pybind11/tools/FindPythonLibsNew.cmake
--rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pybind11/tools/check-style.sh
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pybind11/tools/cmake_uninstall.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pybind11/tools/libsize.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1306 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pybind11/tools/make_changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)    14579 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pybind11/tools/pybind11Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pybind11/tools/pybind11NewTools.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pybind11/tools/pybind11Tools.cmake
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pybind11/tools/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pybind11/tools/setup_global.py.in
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pybind11/tools/setup_main.py.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:55:02.006273 pyllamacpp-2.1.1/pyllamacpp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pyllamacpp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pyllamacpp/_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pyllamacpp/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pyllamacpp/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12153 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pyllamacpp/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pyllamacpp/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10835 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pyllamacpp/webui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:55:02.022273 pyllamacpp-2.1.1/pyllamacpp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6783 2023-05-02 03:55:01.000000 pyllamacpp-2.1.1/pyllamacpp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-05-02 03:55:01.000000 pyllamacpp-2.1.1/pyllamacpp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 03:55:01.000000 pyllamacpp-2.1.1/pyllamacpp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-02 03:55:01.000000 pyllamacpp-2.1.1/pyllamacpp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 03:55:01.000000 pyllamacpp-2.1.1/pyllamacpp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-02 03:55:01.000000 pyllamacpp-2.1.1/pyllamacpp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 03:55:02.022273 pyllamacpp-2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:55:02.022273 pyllamacpp-2.1.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/src/llama.cpp_LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    26926 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/src/main.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-05-02 03:54:50.000000 pyllamacpp-2.1.1/src/main.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:40:06.629970 pyllamacpp-2.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-05-04 03:40:06.629970 pyllamacpp-2.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:40:06.617970 pyllamacpp-2.1.2/llama.cpp/
+-rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-05-04 03:39:57.000000 pyllamacpp-2.1.2/llama.cpp/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:40:06.617970 pyllamacpp-2.1.2/llama.cpp/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-04 03:39:57.000000 pyllamacpp-2.1.2/llama.cpp/examples/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:40:06.617970 pyllamacpp-2.1.2/llama.cpp/examples/embedding/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-04 03:39:57.000000 pyllamacpp-2.1.2/llama.cpp/examples/embedding/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:40:06.617970 pyllamacpp-2.1.2/llama.cpp/examples/main/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-04 03:39:57.000000 pyllamacpp-2.1.2/llama.cpp/examples/main/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:40:06.617970 pyllamacpp-2.1.2/llama.cpp/examples/perplexity/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-04 03:39:57.000000 pyllamacpp-2.1.2/llama.cpp/examples/perplexity/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:40:06.617970 pyllamacpp-2.1.2/llama.cpp/examples/quantize/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-04 03:39:57.000000 pyllamacpp-2.1.2/llama.cpp/examples/quantize/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:40:06.617970 pyllamacpp-2.1.2/llama.cpp/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-04 03:39:57.000000 pyllamacpp-2.1.2/llama.cpp/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:40:06.617970 pyllamacpp-2.1.2/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:40:06.613970 pyllamacpp-2.1.2/pybind11/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:40:06.621970 pyllamacpp-2.1.2/pybind11/include/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)    23920 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 runner    (1001) docker     (123)    64793 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/include/pybind11/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:40:06.625970 pyllamacpp-2.1.2/pybind11/include/pybind11/detail/
+-rw-r--r--   0 runner    (1001) docker     (123)    28526 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 runner    (1001) docker     (123)    51655 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17971 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24196 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 runner    (1001) docker     (123)    44414 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/include/pybind11/detail/typeid.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31441 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12175 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 runner    (1001) docker     (123)    78036 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9781 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/include/pybind11/options.h
+-rw-r--r--   0 runner    (1001) docker     (123)   125927 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 runner    (1001) docker     (123)    80901 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/include/pybind11/pytypes.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:40:06.625970 pyllamacpp-2.1.2/pybind11/include/pybind11/stl/
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14438 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26992 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/include/pybind11/stl_bind.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:40:06.625970 pyllamacpp-2.1.2/pybind11/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    21095 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:40:06.625970 pyllamacpp-2.1.2/pybind11/tests/test_cmake_build/
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/tests/test_cmake_build/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:40:06.625970 pyllamacpp-2.1.2/pybind11/tests/test_cmake_build/installed_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:40:06.625970 pyllamacpp-2.1.2/pybind11/tests/test_cmake_build/installed_function/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:40:06.625970 pyllamacpp-2.1.2/pybind11/tests/test_cmake_build/installed_target/
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:40:06.625970 pyllamacpp-2.1.2/pybind11/tests/test_cmake_build/subdirectory_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:40:06.625970 pyllamacpp-2.1.2/pybind11/tests/test_cmake_build/subdirectory_function/
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:40:06.625970 pyllamacpp-2.1.2/pybind11/tests/test_cmake_build/subdirectory_target/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:40:06.625970 pyllamacpp-2.1.2/pybind11/tests/test_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/tests/test_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:40:06.629970 pyllamacpp-2.1.2/pybind11/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)    10378 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/tools/FindPythonLibsNew.cmake
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/tools/check-style.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/tools/cmake_uninstall.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/tools/libsize.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1306 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/tools/make_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14579 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/tools/pybind11Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/tools/pybind11Tools.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/tools/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/tools/setup_global.py.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/tools/setup_main.py.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:40:06.617970 pyllamacpp-2.1.2/pyllamacpp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pyllamacpp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pyllamacpp/_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pyllamacpp/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pyllamacpp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12464 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pyllamacpp/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pyllamacpp/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10835 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pyllamacpp/webui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:40:06.629970 pyllamacpp-2.1.2/pyllamacpp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-05-04 03:40:06.000000 pyllamacpp-2.1.2/pyllamacpp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-05-04 03:40:06.000000 pyllamacpp-2.1.2/pyllamacpp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 03:40:06.000000 pyllamacpp-2.1.2/pyllamacpp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-04 03:40:06.000000 pyllamacpp-2.1.2/pyllamacpp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 03:40:06.000000 pyllamacpp-2.1.2/pyllamacpp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-04 03:40:06.000000 pyllamacpp-2.1.2/pyllamacpp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 03:40:06.629970 pyllamacpp-2.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:40:06.629970 pyllamacpp-2.1.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/src/llama.cpp_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    27757 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/src/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/src/main.h
```

### Comparing `pyllamacpp-2.1.1/CMakeLists.txt` & `pyllamacpp-2.1.2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/LICENSE` & `pyllamacpp-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/PKG-INFO` & `pyllamacpp-2.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: pyllamacpp
-Version: 2.1.1
-Summary: Python bindings for llama.cpp
-Author: Abdeladim Sadiki
-License: MIT
-Project-URL: Documentation, https://abdeladim-s.github.io/pyllamacpp
-Project-URL: Source, https://github.com/abdeladim-s/pyllamacpp
-Project-URL: Tracker, https://github.com/abdeladim-s/pyllamacpp/issues
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # PyLLaMACpp
 [![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 [![PyPi version](https://badgen.net/pypi/v/pyllamacpp)](https://pypi.org/project/pyllamacpp/)
 
 Python bindings for [llama.cpp](https://github.com/ggerganov/llama.cpp)
 
 
@@ -117,15 +104,15 @@
 
 ### Quick start
 A simple `Pythonic` API is built on top of `llama.cpp` C/C++ functions. You can call it from Python as follows:
 
 ```python
 from pyllamacpp.model import Model
 
-model = Model(ggml_model='./models/gpt4all-model.bin')
+model = Model(model_path='./models/gpt4all-model.bin')
 for token in model.generate("Tell me a joke ?"):
     print(token, end='', flush=True)
 ```
 
 ### Interactive Dialogue
 You can set up an interactive dialogue by simply keeping the `model` variable alive:
 
@@ -176,18 +163,14 @@
     for token in model.generate(prompt, antiprompt='User:'):
       print(f"{token}", end='', flush=True)
       print()
   except KeyboardInterrupt:
     break
 ```
 
-# API reference
-You can check the [API reference documentation](https://abdeladim-s.github.io/pyllamacpp/) for more details.
-
-
 # Supported models
 
 Fully tested with [GPT4All](https://github.com/nomic-ai/gpt4all) model, see [PyGPT4All](https://github.com/nomic-ai/pygpt4all).
 
 But all models supported by `llama.cpp` should be supported as well:
 
 <blockquote>
@@ -199,14 +182,26 @@
 - [X] [Chinese LLaMA / Alpaca](https://github.com/ymcui/Chinese-LLaMA-Alpaca)
 - [X] [Vigogne (French)](https://github.com/bofenghuang/vigogne)
 - [X] [Vicuna](https://github.com/ggerganov/llama.cpp/discussions/643#discussioncomment-5533894)
 - [X] [Koala](https://bair.berkeley.edu/blog/2023/04/03/koala/)
 
 </blockquote>
 
+# Advanced usage
+For advanced users, you can access the [llama.cpp C-API](https://github.com/ggerganov/llama.cpp/blob/master/llama.h) functions directly to make your own logic.
+All functions from `llama.h` are exposed with the binding module [`_pyllamacpp`](https://abdeladim-s.github.io/pyllamacpp/#_pyllamacpp).
+
+# API reference
+You can check the [API reference documentation](https://abdeladim-s.github.io/pyllamacpp/) for more details.
+
+# FAQs
+* [How to build pyllamacpp without AVX2 or FMA.](https://github.com/nomic-ai/pygpt4all/issues/71)
+* [pyllamacpp not support M1 chips MacBook](https://github.com/nomic-ai/pygpt4all/issues/57#issuecomment-1519197837)
+* [ImportError: DLL failed while importing _pyllamacpp](https://github.com/nomic-ai/pygpt4all/issues/53#issuecomment-1529772010)
+
 # Discussions and contributions
 If you find any bug, please open an [issue](https://github.com/abdeladim-s/pyllamacpp/issues).
 
 If you have any feedback, or you want to share how you are using this project, feel free to use the [Discussions](https://github.com/abdeladim-s/pyllamacpp/discussions) and open a new topic.
 
 # License
```

### Comparing `pyllamacpp-2.1.1/README.md` & `pyllamacpp-2.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: pyllamacpp
+Version: 2.1.2
+Summary: Python bindings for llama.cpp
+Author: Abdeladim Sadiki
+License: MIT
+Project-URL: Documentation, https://abdeladim-s.github.io/pyllamacpp
+Project-URL: Source, https://github.com/abdeladim-s/pyllamacpp
+Project-URL: Tracker, https://github.com/abdeladim-s/pyllamacpp/issues
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # PyLLaMACpp
 [![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 [![PyPi version](https://badgen.net/pypi/v/pyllamacpp)](https://pypi.org/project/pyllamacpp/)
 
 Python bindings for [llama.cpp](https://github.com/ggerganov/llama.cpp)
 
 
@@ -104,15 +117,15 @@
 
 ### Quick start
 A simple `Pythonic` API is built on top of `llama.cpp` C/C++ functions. You can call it from Python as follows:
 
 ```python
 from pyllamacpp.model import Model
 
-model = Model(ggml_model='./models/gpt4all-model.bin')
+model = Model(model_path='./models/gpt4all-model.bin')
 for token in model.generate("Tell me a joke ?"):
     print(token, end='', flush=True)
 ```
 
 ### Interactive Dialogue
 You can set up an interactive dialogue by simply keeping the `model` variable alive:
 
@@ -163,18 +176,14 @@
     for token in model.generate(prompt, antiprompt='User:'):
       print(f"{token}", end='', flush=True)
       print()
   except KeyboardInterrupt:
     break
 ```
 
-# API reference
-You can check the [API reference documentation](https://abdeladim-s.github.io/pyllamacpp/) for more details.
-
-
 # Supported models
 
 Fully tested with [GPT4All](https://github.com/nomic-ai/gpt4all) model, see [PyGPT4All](https://github.com/nomic-ai/pygpt4all).
 
 But all models supported by `llama.cpp` should be supported as well:
 
 <blockquote>
@@ -186,14 +195,26 @@
 - [X] [Chinese LLaMA / Alpaca](https://github.com/ymcui/Chinese-LLaMA-Alpaca)
 - [X] [Vigogne (French)](https://github.com/bofenghuang/vigogne)
 - [X] [Vicuna](https://github.com/ggerganov/llama.cpp/discussions/643#discussioncomment-5533894)
 - [X] [Koala](https://bair.berkeley.edu/blog/2023/04/03/koala/)
 
 </blockquote>
 
+# Advanced usage
+For advanced users, you can access the [llama.cpp C-API](https://github.com/ggerganov/llama.cpp/blob/master/llama.h) functions directly to make your own logic.
+All functions from `llama.h` are exposed with the binding module [`_pyllamacpp`](https://abdeladim-s.github.io/pyllamacpp/#_pyllamacpp).
+
+# API reference
+You can check the [API reference documentation](https://abdeladim-s.github.io/pyllamacpp/) for more details.
+
+# FAQs
+* [How to build pyllamacpp without AVX2 or FMA.](https://github.com/nomic-ai/pygpt4all/issues/71)
+* [pyllamacpp not support M1 chips MacBook](https://github.com/nomic-ai/pygpt4all/issues/57#issuecomment-1519197837)
+* [ImportError: DLL failed while importing _pyllamacpp](https://github.com/nomic-ai/pygpt4all/issues/53#issuecomment-1529772010)
+
 # Discussions and contributions
 If you find any bug, please open an [issue](https://github.com/abdeladim-s/pyllamacpp/issues).
 
 If you have any feedback, or you want to share how you are using this project, feel free to use the [Discussions](https://github.com/abdeladim-s/pyllamacpp/discussions) and open a new topic.
 
 # License
```

### Comparing `pyllamacpp-2.1.1/llama.cpp/CMakeLists.txt` & `pyllamacpp-2.1.2/llama.cpp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/llama.cpp/examples/CMakeLists.txt` & `pyllamacpp-2.1.2/llama.cpp/examples/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/pybind11/CMakeLists.txt` & `pyllamacpp-2.1.2/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/pybind11/LICENSE` & `pyllamacpp-2.1.2/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/pybind11/include/pybind11/attr.h` & `pyllamacpp-2.1.2/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/pybind11/include/pybind11/buffer_info.h` & `pyllamacpp-2.1.2/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/pybind11/include/pybind11/cast.h` & `pyllamacpp-2.1.2/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/pybind11/include/pybind11/chrono.h` & `pyllamacpp-2.1.2/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/pybind11/include/pybind11/complex.h` & `pyllamacpp-2.1.2/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/pybind11/include/pybind11/detail/class.h` & `pyllamacpp-2.1.2/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/pybind11/include/pybind11/detail/common.h` & `pyllamacpp-2.1.2/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/pybind11/include/pybind11/detail/descr.h` & `pyllamacpp-2.1.2/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/pybind11/include/pybind11/detail/init.h` & `pyllamacpp-2.1.2/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/pybind11/include/pybind11/detail/internals.h` & `pyllamacpp-2.1.2/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/pybind11/include/pybind11/detail/type_caster_base.h` & `pyllamacpp-2.1.2/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/pybind11/include/pybind11/detail/typeid.h` & `pyllamacpp-2.1.2/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/pybind11/include/pybind11/eigen.h` & `pyllamacpp-2.1.2/pybind11/include/pybind11/eigen.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/pybind11/include/pybind11/embed.h` & `pyllamacpp-2.1.2/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/pybind11/include/pybind11/eval.h` & `pyllamacpp-2.1.2/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/pybind11/include/pybind11/functional.h` & `pyllamacpp-2.1.2/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/pybind11/include/pybind11/gil.h` & `pyllamacpp-2.1.2/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/pybind11/include/pybind11/iostream.h` & `pyllamacpp-2.1.2/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/pybind11/include/pybind11/numpy.h` & `pyllamacpp-2.1.2/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/pybind11/include/pybind11/operators.h` & `pyllamacpp-2.1.2/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/pybind11/include/pybind11/options.h` & `pyllamacpp-2.1.2/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/pybind11/include/pybind11/pybind11.h` & `pyllamacpp-2.1.2/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/pybind11/include/pybind11/pytypes.h` & `pyllamacpp-2.1.2/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/pybind11/include/pybind11/stl/filesystem.h` & `pyllamacpp-2.1.2/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/pybind11/include/pybind11/stl.h` & `pyllamacpp-2.1.2/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/pybind11/include/pybind11/stl_bind.h` & `pyllamacpp-2.1.2/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/pybind11/tests/CMakeLists.txt` & `pyllamacpp-2.1.2/pybind11/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/pybind11/tests/test_cmake_build/CMakeLists.txt` & `pyllamacpp-2.1.2/pybind11/tests/test_cmake_build/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt` & `pyllamacpp-2.1.2/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt` & `pyllamacpp-2.1.2/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt` & `pyllamacpp-2.1.2/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt` & `pyllamacpp-2.1.2/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt` & `pyllamacpp-2.1.2/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt` & `pyllamacpp-2.1.2/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/pybind11/tests/test_embed/CMakeLists.txt` & `pyllamacpp-2.1.2/pybind11/tests/test_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/pybind11/tools/FindCatch.cmake` & `pyllamacpp-2.1.2/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/pybind11/tools/FindEigen3.cmake` & `pyllamacpp-2.1.2/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/pybind11/tools/FindPythonLibsNew.cmake` & `pyllamacpp-2.1.2/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/pybind11/tools/check-style.sh` & `pyllamacpp-2.1.2/pybind11/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/pybind11/tools/cmake_uninstall.cmake.in` & `pyllamacpp-2.1.2/pybind11/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/pybind11/tools/libsize.py` & `pyllamacpp-2.1.2/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/pybind11/tools/make_changelog.py` & `pyllamacpp-2.1.2/pybind11/tools/make_changelog.py`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/pybind11/tools/pybind11Common.cmake` & `pyllamacpp-2.1.2/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/pybind11/tools/pybind11Config.cmake.in` & `pyllamacpp-2.1.2/pybind11/tools/pybind11Config.cmake.in`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/pybind11/tools/pybind11NewTools.cmake` & `pyllamacpp-2.1.2/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/pybind11/tools/pybind11Tools.cmake` & `pyllamacpp-2.1.2/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/pybind11/tools/setup_global.py.in` & `pyllamacpp-2.1.2/pybind11/tools/setup_global.py.in`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/pybind11/tools/setup_main.py.in` & `pyllamacpp-2.1.2/pybind11/tools/setup_main.py.in`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/pyllamacpp/_logger.py` & `pyllamacpp-2.1.2/pyllamacpp/_logger.py`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/pyllamacpp/cli.py` & `pyllamacpp-2.1.2/pyllamacpp/cli.py`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/pyllamacpp/model.py` & `pyllamacpp-2.1.2/pyllamacpp/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,17 +33,17 @@
         print(token, end='', flush=True)
     ```
     """
     _new_text_callback = None
 
     def __init__(self,
                  model_path: str,
-                 prompt_context='',
-                 prompt_prefix='',
-                 prompt_suffix='',
+                 prompt_context: str = '',
+                 prompt_prefix: str = '',
+                 prompt_suffix: str = '',
                  log_level: int = logging.ERROR,
                  n_ctx: int = 512,
                  seed: int = 0,
                  n_parts: int = -1,
                  f16_kv: bool = False,
                  logits_all: bool = False,
                  vocab_only: bool = False,
@@ -99,15 +99,16 @@
 
         self._prompt_context_tokens = []
         self._prompt_prefix_tokens = []
         self._prompt_suffix_tokens = []
 
         self.reset()
 
-    def reset(self):
+    def reset(self) -> None:
+        """Resets the context"""
         self._prompt_context_tokens = pp.llama_tokenize(self._ctx, self.prompt_cntext, True)
         self._prompt_prefix_tokens = pp.llama_tokenize(self._ctx, self.prompt_prefix, True)
         self._prompt_suffix_tokens = pp.llama_tokenize(self._ctx, self.prompt_suffix, True)
         self._last_n_tokens = [0] * self._n_ctx  # n_ctx elements
         self._n_past = 0
 
     def generate(self,
@@ -179,15 +180,18 @@
                                                           repeat_last_n,
                                                           top_k,
                                                           top_p,
                                                           temp,
                                                           repeat_penalty)
 
             predicted_tokens.append(predicted_token)
-            token_str = pp.llama_token_to_str(self._ctx, predicted_token)
+            # tokens come as raw undecoded bytes,
+            # and we decode them, replacing those that can't be decoded.
+            # i decoded here for fear of breaking the stopword logic, 
+            token_str = pp.llama_token_to_str(self._ctx, predicted_token).decode('utf-8', "replace")
             if antiprompt is not None:
                 if token_str == '\n':
                     sequence_queue.append(token_str)
                     continue
                 if len(sequence_queue) != 0:
                     if stop_word.startswith(''.join(sequence_queue).strip()):
                         sequence_queue.append(token_str)
@@ -196,15 +200,14 @@
                         else:
                             continue
                     else:
                         # consume sequence queue tokens
                         while len(sequence_queue) != 0:
                             yield sequence_queue.pop(0)
                         sequence_queue = []
-
             self._last_n_tokens.pop(0)
             self._last_n_tokens.append(predicted_token)
             yield token_str
             if n_predict is not None:
                 if n_remain == n_predict:
                     break
                 else:
@@ -224,19 +227,19 @@
         """
         Internal new_segment_callback, it just calls the user's callback with the `Segment` object
         :return: None
         """
         if Model._new_text_callback is not None:
             Model._new_text_callback(text)
         # save res
-        self.res += text
+        self.res += text.decode('utf-8', 'replace')
 
     def cpp_generate(self, prompt: str,
                      n_predict: int = 128,
-                     new_text_callback: Callable[[str], None] = None,
+                     new_text_callback: Callable[[bytes], None] = None,
                      n_threads: int = 4,
                      repeat_last_n: int = 64,
                      top_k: int = 40,
                      top_p: float = 0.95,
                      temp: float = 0.8,
                      repeat_penalty: float = 1.10,
                      n_batch: int = 8,
```

### Comparing `pyllamacpp-2.1.1/pyllamacpp/utils.py` & `pyllamacpp-2.1.2/pyllamacpp/utils.py`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/pyllamacpp/webui.py` & `pyllamacpp-2.1.2/pyllamacpp/webui.py`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/pyllamacpp.egg-info/PKG-INFO` & `pyllamacpp-2.1.2/pyllamacpp.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyllamacpp
-Version: 2.1.1
+Version: 2.1.2
 Summary: Python bindings for llama.cpp
 Author: Abdeladim Sadiki
 License: MIT
 Project-URL: Documentation, https://abdeladim-s.github.io/pyllamacpp
 Project-URL: Source, https://github.com/abdeladim-s/pyllamacpp
 Project-URL: Tracker, https://github.com/abdeladim-s/pyllamacpp/issues
 Requires-Python: >=3.8
@@ -117,15 +117,15 @@
 
 ### Quick start
 A simple `Pythonic` API is built on top of `llama.cpp` C/C++ functions. You can call it from Python as follows:
 
 ```python
 from pyllamacpp.model import Model
 
-model = Model(ggml_model='./models/gpt4all-model.bin')
+model = Model(model_path='./models/gpt4all-model.bin')
 for token in model.generate("Tell me a joke ?"):
     print(token, end='', flush=True)
 ```
 
 ### Interactive Dialogue
 You can set up an interactive dialogue by simply keeping the `model` variable alive:
 
@@ -176,18 +176,14 @@
     for token in model.generate(prompt, antiprompt='User:'):
       print(f"{token}", end='', flush=True)
       print()
   except KeyboardInterrupt:
     break
 ```
 
-# API reference
-You can check the [API reference documentation](https://abdeladim-s.github.io/pyllamacpp/) for more details.
-
-
 # Supported models
 
 Fully tested with [GPT4All](https://github.com/nomic-ai/gpt4all) model, see [PyGPT4All](https://github.com/nomic-ai/pygpt4all).
 
 But all models supported by `llama.cpp` should be supported as well:
 
 <blockquote>
@@ -199,14 +195,26 @@
 - [X] [Chinese LLaMA / Alpaca](https://github.com/ymcui/Chinese-LLaMA-Alpaca)
 - [X] [Vigogne (French)](https://github.com/bofenghuang/vigogne)
 - [X] [Vicuna](https://github.com/ggerganov/llama.cpp/discussions/643#discussioncomment-5533894)
 - [X] [Koala](https://bair.berkeley.edu/blog/2023/04/03/koala/)
 
 </blockquote>
 
+# Advanced usage
+For advanced users, you can access the [llama.cpp C-API](https://github.com/ggerganov/llama.cpp/blob/master/llama.h) functions directly to make your own logic.
+All functions from `llama.h` are exposed with the binding module [`_pyllamacpp`](https://abdeladim-s.github.io/pyllamacpp/#_pyllamacpp).
+
+# API reference
+You can check the [API reference documentation](https://abdeladim-s.github.io/pyllamacpp/) for more details.
+
+# FAQs
+* [How to build pyllamacpp without AVX2 or FMA.](https://github.com/nomic-ai/pygpt4all/issues/71)
+* [pyllamacpp not support M1 chips MacBook](https://github.com/nomic-ai/pygpt4all/issues/57#issuecomment-1519197837)
+* [ImportError: DLL failed while importing _pyllamacpp](https://github.com/nomic-ai/pygpt4all/issues/53#issuecomment-1529772010)
+
 # Discussions and contributions
 If you find any bug, please open an [issue](https://github.com/abdeladim-s/pyllamacpp/issues).
 
 If you have any feedback, or you want to share how you are using this project, feel free to use the [Discussions](https://github.com/abdeladim-s/pyllamacpp/discussions) and open a new topic.
 
 # License
```

### Comparing `pyllamacpp-2.1.1/pyllamacpp.egg-info/SOURCES.txt` & `pyllamacpp-2.1.2/pyllamacpp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/pyproject.toml` & `pyllamacpp-2.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/setup.py` & `pyllamacpp-2.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 # The information here can also be placed in setup.cfg - better separation of
 # logic and declaration, and simpler if you include description/version in a file.
 setup(
     name="pyllamacpp",
-    version="2.1.1",
+    version="2.1.2",
     author="Abdeladim Sadiki",
     description="Python bindings for llama.cpp",
     long_description=long_description,
     ext_modules=[CMakeExtension("_pyllamacpp")],
     cmdclass={"build_ext": CMakeBuild},
     zip_safe=False,
     # extras_require={"test": ["pytest>=6.0"]},
```

### Comparing `pyllamacpp-2.1.1/src/llama.cpp_LICENSE` & `pyllamacpp-2.1.2/src/llama.cpp_LICENSE`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.1/src/main.cpp` & `pyllamacpp-2.1.2/src/main.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -476,15 +476,20 @@
             }
         }
 
         // display text
         if (!input_noecho) {
             for (auto id : embd) {
 //                printf("%s", llama_token_to_str(ctx, id));
-                new_text_callback(llama_token_to_str(ctx, id));
+                //@NOTE: model.cpp_generate invokes llama_generate() with a python callback function.
+                //@NOTE: we need to make sure that when the python callback function is called, it gets callback with raw bytes
+                //@NOTE: of generated token, else pybind with implicityl try to decode it to Unicode, and cause UnicodeDecodeError
+                std::string tok_str = llama_token_to_str(ctx, id);
+                new_text_callback(py::bytes(tok_str));
+
             }
             fflush(stdout);
         }
         // reset color to default if we there is no pending user input
 //        if (!input_noecho && (int)embd_inp.size() == n_consumed) {
 //            set_console_color(con_st, CONSOLE_COLOR_DEFAULT);
 //        }
@@ -682,15 +687,20 @@
     m.def("llama_eval", &llama_eval_wrapper);
     m.def("llama_tokenize", &llama_tokenize_wrapper);
     m.def("llama_n_vocab", &llama_n_vocab_wrapper);
     m.def("llama_n_ctx", &llama_n_ctx_wrapper);
     m.def("llama_n_embd", &llama_n_embd_wrapper);
     m.def("llama_get_logits", &llama_get_logits_wrapper);
     m.def("llama_get_embeddings", &llama_get_embeddings_wrapper);
-    m.def("llama_token_to_str", &llama_token_to_str_wrapper);
+    m.def("llama_token_to_str", [](struct llama_context_wrapper * ctx_w, llama_token token){
+        //@NOTE: model.generate() calls pp.llama_token_to_str -> llama_token_to_str_wrapper()
+        //@NOTE: we need to make sure that llama_token_to_str_wrapper() returns raw bytes
+        //@NOTE: to prevent implicit conversion of const char* to unicode on python side, leading to UnicodeDecodeError
+        return py::bytes(llama_token_to_str_wrapper(ctx_w, token));
+    });
 
     m.def("llama_token_bos", &llama_token_bos);
     m.def("llama_token_eos", &llama_token_eos);
 
     m.def("llama_sample_top_p_top_k", &llama_sample_top_p_top_k_wrapper);
 
     m.def("llama_print_timings", &llama_print_timings_wrapper);
```

### Comparing `pyllamacpp-2.1.1/src/main.h` & `pyllamacpp-2.1.2/src/main.h`

 * *Files identical despite different names*

