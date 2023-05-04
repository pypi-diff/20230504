# Comparing `tmp/tl2cgen-0.1.0.tar.gz` & `tmp/tl2cgen-0.2.0.tar.gz`

## Comparing `tl2cgen-0.1.0.tar` & `tl2cgen-0.2.0.tar`

### file list

```diff
@@ -1,104 +1,104 @@
--rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/CMakeLists.txt
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/LICENSE
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/cmake/Doxygen.cmake
--rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/cmake/ExternalLibs.cmake
--rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/cmake/Sanitizer.cmake
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/cmake/TL2cgenConfig.cmake.in
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/cmake/Utils.cmake
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/cmake/Version.cmake
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/cmake/version.h.in
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/cmake/modules/FindASan.cmake
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/cmake/modules/FindLSan.cmake
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/cmake/modules/FindTSan.cmake
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/cmake/modules/FindUBSan.cmake
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/include/tl2cgen/annotator.h
--rw-r--r--   0        0        0    16124 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/include/tl2cgen/c_api.h
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/include/tl2cgen/c_api_error.h
--rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/include/tl2cgen/compiler.h
--rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/include/tl2cgen/compiler_param.h
--rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/include/tl2cgen/data_matrix.h
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/include/tl2cgen/data_matrix_types.h
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/include/tl2cgen/error.h
--rw-r--r--   0        0        0     6090 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/include/tl2cgen/logging.h
--rw-r--r--   0        0        0     7675 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/include/tl2cgen/predictor.h
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/include/tl2cgen/predictor_types.h
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/include/tl2cgen/thread_local.h
--rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/include/tl2cgen/detail/data_matrix_impl.h
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/include/tl2cgen/detail/filesystem.h
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/include/tl2cgen/detail/math_funcs.h
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/include/tl2cgen/detail/compiler/ast_native.h
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/include/tl2cgen/detail/compiler/elf_formatter.h
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/include/tl2cgen/detail/compiler/failsafe.h
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/include/tl2cgen/detail/compiler/pred_transform.h
--rw-r--r--   0        0        0     6209 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/include/tl2cgen/detail/compiler/ast/ast.h
--rw-r--r--   0        0        0     3869 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/include/tl2cgen/detail/compiler/ast/builder.h
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/include/tl2cgen/detail/compiler/templates/code_folder_template.h
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/include/tl2cgen/detail/compiler/templates/header_template.h
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/include/tl2cgen/detail/compiler/templates/main_template.h
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/include/tl2cgen/detail/compiler/templates/pred_transform.h
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/include/tl2cgen/detail/compiler/templates/qnode_template.h
--rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/include/tl2cgen/detail/compiler/templates/typeinfo.h
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/include/tl2cgen/detail/compiler/util/categorical_bitmap.h
--rw-r--r--   0        0        0     6356 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/include/tl2cgen/detail/compiler/util/code_folding_util.h
--rw-r--r--   0        0        0     3918 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/include/tl2cgen/detail/compiler/util/format_util.h
--rw-r--r--   0        0        0     9153 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/include/tl2cgen/detail/predictor/predictor_impl.h
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/include/tl2cgen/detail/predictor/shared_library.h
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/include/tl2cgen/detail/threading_utils/omp_config.h
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/include/tl2cgen/detail/threading_utils/omp_exception.h
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/include/tl2cgen/detail/threading_utils/omp_funcs.h
--rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/include/tl2cgen/detail/threading_utils/parallel_for.h
--rw-r--r--   0        0        0     5721 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/src/CMakeLists.txt
--rw-r--r--   0        0        0     9703 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/src/annotator.cc
--rw-r--r--   0        0        0     2733 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/src/filesystem.cc
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/src/logging.cc
--rw-r--r--   0        0        0    10340 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/src/c_api/c_api.cc
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/src/c_api/c_api_error.cc
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/src/c_api/c_api_treelite_bridge.cc
--rw-r--r--   0        0        0    30107 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/src/compiler/ast_native.cc
--rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/src/compiler/compiler.cc
--rw-r--r--   0        0        0    10328 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/src/compiler/elf_formatter.cc
--rw-r--r--   0        0        0    15023 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/src/compiler/failsafe.cc
--rw-r--r--   0        0        0     6157 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/src/compiler/pred_transform.cc
--rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/src/compiler/ast/builder/build.cc
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/src/compiler/ast/builder/dump.cc
--rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/src/compiler/ast/builder/fold_code.cc
--rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/src/compiler/ast/builder/is_categorical_array.cc
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/src/compiler/ast/builder/load_data_counts.cc
--rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/src/compiler/ast/builder/quantize.cc
--rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/src/compiler/ast/builder/split.cc
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/src/compiler/templates/code_folder_template.cc
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/src/compiler/templates/header_template.cc
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/src/compiler/templates/main_template.cc
--rw-r--r--   0        0        0     7019 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/src/compiler/templates/pred_transform.cc
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/src/compiler/templates/qnode_template.cc
--rw-r--r--   0        0        0     6313 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/src/predictor/predictor.cc
--rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/cpp_src/src/predictor/shared_library.cc
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/packager/__init__.py
--rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/packager/build_config.py
--rw-r--r--   0        0        0     5687 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/packager/nativelib.py
--rw-r--r--   0        0        0     5643 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/packager/pep517.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/packager/sdist.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/packager/util.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/tl2cgen/VERSION
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/tl2cgen/__init__.py
--rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/tl2cgen/core.py
--rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/tl2cgen/create_shared.py
--rw-r--r--   0        0        0     7012 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/tl2cgen/data.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/tl2cgen/dtypes.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/tl2cgen/exception.py
--rw-r--r--   0        0        0     5248 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/tl2cgen/generate_makefile.py
--rw-r--r--   0        0        0     5336 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/tl2cgen/handle_class.py
--rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/tl2cgen/libloader.py
--rw-r--r--   0        0        0     7322 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/tl2cgen/predictor.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/tl2cgen/py.typed
--rw-r--r--   0        0        0     6092 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/tl2cgen/shortcuts.py
--rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/tl2cgen/util.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/tl2cgen/contrib/__init__.py
--rw-r--r--   0        0        0     4353 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/tl2cgen/contrib/create_shared.py
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/tl2cgen/contrib/gcc.py
--rw-r--r--   0        0        0     5168 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/tl2cgen/contrib/msvc.py
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/tl2cgen/contrib/util.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/README.rst
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/hatch_build.py
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 tl2cgen-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/CMakeLists.txt
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/LICENSE
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/cmake/Doxygen.cmake
+-rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/cmake/ExternalLibs.cmake
+-rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/cmake/Sanitizer.cmake
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/cmake/TL2cgenConfig.cmake.in
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/cmake/Utils.cmake
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/cmake/Version.cmake
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/cmake/version.h.in
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/cmake/modules/FindASan.cmake
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/cmake/modules/FindLSan.cmake
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/cmake/modules/FindTSan.cmake
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/cmake/modules/FindUBSan.cmake
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/include/tl2cgen/annotator.h
+-rw-r--r--   0        0        0    16124 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/include/tl2cgen/c_api.h
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/include/tl2cgen/c_api_error.h
+-rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/include/tl2cgen/compiler.h
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/include/tl2cgen/compiler_param.h
+-rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/include/tl2cgen/data_matrix.h
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/include/tl2cgen/data_matrix_types.h
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/include/tl2cgen/error.h
+-rw-r--r--   0        0        0     6090 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/include/tl2cgen/logging.h
+-rw-r--r--   0        0        0     7675 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/include/tl2cgen/predictor.h
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/include/tl2cgen/predictor_types.h
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/include/tl2cgen/thread_local.h
+-rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/include/tl2cgen/detail/data_matrix_impl.h
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/include/tl2cgen/detail/filesystem.h
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/include/tl2cgen/detail/math_funcs.h
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/include/tl2cgen/detail/compiler/ast_native.h
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/include/tl2cgen/detail/compiler/elf_formatter.h
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/include/tl2cgen/detail/compiler/failsafe.h
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/include/tl2cgen/detail/compiler/pred_transform.h
+-rw-r--r--   0        0        0     6209 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/include/tl2cgen/detail/compiler/ast/ast.h
+-rw-r--r--   0        0        0     3869 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/include/tl2cgen/detail/compiler/ast/builder.h
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/include/tl2cgen/detail/compiler/templates/code_folder_template.h
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/include/tl2cgen/detail/compiler/templates/header_template.h
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/include/tl2cgen/detail/compiler/templates/main_template.h
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/include/tl2cgen/detail/compiler/templates/pred_transform.h
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/include/tl2cgen/detail/compiler/templates/qnode_template.h
+-rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/include/tl2cgen/detail/compiler/templates/typeinfo.h
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/include/tl2cgen/detail/compiler/util/categorical_bitmap.h
+-rw-r--r--   0        0        0     6356 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/include/tl2cgen/detail/compiler/util/code_folding_util.h
+-rw-r--r--   0        0        0     3918 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/include/tl2cgen/detail/compiler/util/format_util.h
+-rw-r--r--   0        0        0     9153 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/include/tl2cgen/detail/predictor/predictor_impl.h
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/include/tl2cgen/detail/predictor/shared_library.h
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/include/tl2cgen/detail/threading_utils/omp_config.h
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/include/tl2cgen/detail/threading_utils/omp_exception.h
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/include/tl2cgen/detail/threading_utils/omp_funcs.h
+-rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/include/tl2cgen/detail/threading_utils/parallel_for.h
+-rw-r--r--   0        0        0     5721 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/src/CMakeLists.txt
+-rw-r--r--   0        0        0     9703 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/src/annotator.cc
+-rw-r--r--   0        0        0     2733 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/src/filesystem.cc
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/src/logging.cc
+-rw-r--r--   0        0        0    10340 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/src/c_api/c_api.cc
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/src/c_api/c_api_error.cc
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/src/c_api/c_api_treelite_bridge.cc
+-rw-r--r--   0        0        0    30107 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/src/compiler/ast_native.cc
+-rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/src/compiler/compiler.cc
+-rw-r--r--   0        0        0    10328 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/src/compiler/elf_formatter.cc
+-rw-r--r--   0        0        0    15023 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/src/compiler/failsafe.cc
+-rw-r--r--   0        0        0     6157 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/src/compiler/pred_transform.cc
+-rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/src/compiler/ast/builder/build.cc
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/src/compiler/ast/builder/dump.cc
+-rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/src/compiler/ast/builder/fold_code.cc
+-rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/src/compiler/ast/builder/is_categorical_array.cc
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/src/compiler/ast/builder/load_data_counts.cc
+-rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/src/compiler/ast/builder/quantize.cc
+-rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/src/compiler/ast/builder/split.cc
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/src/compiler/templates/code_folder_template.cc
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/src/compiler/templates/header_template.cc
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/src/compiler/templates/main_template.cc
+-rw-r--r--   0        0        0     7019 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/src/compiler/templates/pred_transform.cc
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/src/compiler/templates/qnode_template.cc
+-rw-r--r--   0        0        0     6313 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/src/predictor/predictor.cc
+-rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/cpp_src/src/predictor/shared_library.cc
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/packager/__init__.py
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/packager/build_config.py
+-rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/packager/nativelib.py
+-rw-r--r--   0        0        0     5643 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/packager/pep517.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/packager/sdist.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/packager/util.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/tl2cgen/VERSION
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/tl2cgen/__init__.py
+-rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/tl2cgen/core.py
+-rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/tl2cgen/create_shared.py
+-rw-r--r--   0        0        0     7012 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/tl2cgen/data.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/tl2cgen/dtypes.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/tl2cgen/exception.py
+-rw-r--r--   0        0        0     5248 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/tl2cgen/generate_makefile.py
+-rw-r--r--   0        0        0     5336 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/tl2cgen/handle_class.py
+-rw-r--r--   0        0        0     4880 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/tl2cgen/libloader.py
+-rw-r--r--   0        0        0     7322 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/tl2cgen/predictor.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/tl2cgen/py.typed
+-rw-r--r--   0        0        0     6092 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/tl2cgen/shortcuts.py
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/tl2cgen/util.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/tl2cgen/contrib/__init__.py
+-rw-r--r--   0        0        0     4353 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/tl2cgen/contrib/create_shared.py
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/tl2cgen/contrib/gcc.py
+-rw-r--r--   0        0        0     5168 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/tl2cgen/contrib/msvc.py
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/tl2cgen/contrib/util.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/README.rst
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/hatch_build.py
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 tl2cgen-0.2.0/PKG-INFO
```

### Comparing `tl2cgen-0.1.0/cpp_src/CMakeLists.txt` & `tl2cgen-0.2.0/cpp_src/CMakeLists.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 cmake_policy(SET CMP0091 NEW)
 set(CMAKE_FIND_NO_INSTALL_PREFIX TRUE FORCE)
 cmake_minimum_required(VERSION 3.16)
-project(tl2cgen LANGUAGES CXX C VERSION 0.1.0)
+project(tl2cgen LANGUAGES CXX C VERSION 0.2.0)
 
 set(CMAKE_MSVC_RUNTIME_LIBRARY "MultiThreaded$<$<CONFIG:Debug>:Debug>")
 
 # check MSVC version
 if (MSVC)
   if (MSVC_VERSION LESS 1920)
     message(FATAL_ERROR "Need Visual Studio 2019 or newer to compile TL2cgen")
```

### Comparing `tl2cgen-0.1.0/cpp_src/LICENSE` & `tl2cgen-0.2.0/cpp_src/LICENSE`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/cmake/ExternalLibs.cmake` & `tl2cgen-0.2.0/cpp_src/cmake/ExternalLibs.cmake`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/cmake/Sanitizer.cmake` & `tl2cgen-0.2.0/cpp_src/cmake/Sanitizer.cmake`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/cmake/Utils.cmake` & `tl2cgen-0.2.0/cpp_src/cmake/Utils.cmake`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/include/tl2cgen/annotator.h` & `tl2cgen-0.2.0/cpp_src/include/tl2cgen/annotator.h`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/include/tl2cgen/c_api.h` & `tl2cgen-0.2.0/cpp_src/include/tl2cgen/c_api.h`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/include/tl2cgen/c_api_error.h` & `tl2cgen-0.2.0/cpp_src/include/tl2cgen/c_api_error.h`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/include/tl2cgen/compiler.h` & `tl2cgen-0.2.0/cpp_src/include/tl2cgen/compiler.h`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/include/tl2cgen/compiler_param.h` & `tl2cgen-0.2.0/cpp_src/include/tl2cgen/compiler_param.h`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
   /*!
    * \defgroup compiler_param Parameters for tree compiler
    * \{
    */
   /*!
    * \brief Name of model annotation file.
    * \verbatim embed:rst:leading-asterisk
-   * Use :py:meth:`~tl2cgen.annotate_branch` to generate this file.
+   * Use :py:func:`tl2cgen.annotate_branch` to generate this file.
    * \endverbatim
    */
   std::string annotate_in;
   /*! \brief Whether to quantize threshold points (0: no, >0: yes) */
   int quantize;
   /*! \brief Option to enable parallel compilation;
              if set to nonzero, the trees will be evely distributed
```

### Comparing `tl2cgen-0.1.0/cpp_src/include/tl2cgen/data_matrix.h` & `tl2cgen-0.2.0/cpp_src/include/tl2cgen/data_matrix.h`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/include/tl2cgen/data_matrix_types.h` & `tl2cgen-0.2.0/cpp_src/include/tl2cgen/data_matrix_types.h`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/include/tl2cgen/logging.h` & `tl2cgen-0.2.0/cpp_src/include/tl2cgen/logging.h`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/include/tl2cgen/predictor.h` & `tl2cgen-0.2.0/cpp_src/include/tl2cgen/predictor.h`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/include/tl2cgen/predictor_types.h` & `tl2cgen-0.2.0/cpp_src/include/tl2cgen/predictor_types.h`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/include/tl2cgen/thread_local.h` & `tl2cgen-0.2.0/cpp_src/include/tl2cgen/thread_local.h`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/include/tl2cgen/detail/data_matrix_impl.h` & `tl2cgen-0.2.0/cpp_src/include/tl2cgen/detail/data_matrix_impl.h`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/include/tl2cgen/detail/filesystem.h` & `tl2cgen-0.2.0/cpp_src/include/tl2cgen/detail/filesystem.h`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/include/tl2cgen/detail/math_funcs.h` & `tl2cgen-0.2.0/cpp_src/include/tl2cgen/detail/math_funcs.h`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/include/tl2cgen/detail/compiler/ast_native.h` & `tl2cgen-0.2.0/cpp_src/include/tl2cgen/detail/compiler/ast_native.h`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/include/tl2cgen/detail/compiler/elf_formatter.h` & `tl2cgen-0.2.0/cpp_src/include/tl2cgen/detail/compiler/elf_formatter.h`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/include/tl2cgen/detail/compiler/failsafe.h` & `tl2cgen-0.2.0/cpp_src/include/tl2cgen/detail/compiler/failsafe.h`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/include/tl2cgen/detail/compiler/pred_transform.h` & `tl2cgen-0.2.0/cpp_src/include/tl2cgen/detail/compiler/pred_transform.h`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/include/tl2cgen/detail/compiler/ast/ast.h` & `tl2cgen-0.2.0/cpp_src/include/tl2cgen/detail/compiler/ast/ast.h`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/include/tl2cgen/detail/compiler/ast/builder.h` & `tl2cgen-0.2.0/cpp_src/include/tl2cgen/detail/compiler/ast/builder.h`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/include/tl2cgen/detail/compiler/templates/code_folder_template.h` & `tl2cgen-0.2.0/cpp_src/include/tl2cgen/detail/compiler/templates/code_folder_template.h`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/include/tl2cgen/detail/compiler/templates/header_template.h` & `tl2cgen-0.2.0/cpp_src/include/tl2cgen/detail/compiler/templates/header_template.h`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/include/tl2cgen/detail/compiler/templates/main_template.h` & `tl2cgen-0.2.0/cpp_src/include/tl2cgen/detail/compiler/templates/main_template.h`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/include/tl2cgen/detail/compiler/templates/pred_transform.h` & `tl2cgen-0.2.0/cpp_src/include/tl2cgen/detail/compiler/templates/pred_transform.h`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/include/tl2cgen/detail/compiler/templates/qnode_template.h` & `tl2cgen-0.2.0/cpp_src/include/tl2cgen/detail/compiler/templates/qnode_template.h`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/include/tl2cgen/detail/compiler/templates/typeinfo.h` & `tl2cgen-0.2.0/cpp_src/include/tl2cgen/detail/compiler/templates/typeinfo.h`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/include/tl2cgen/detail/compiler/util/categorical_bitmap.h` & `tl2cgen-0.2.0/cpp_src/include/tl2cgen/detail/compiler/util/categorical_bitmap.h`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/include/tl2cgen/detail/compiler/util/code_folding_util.h` & `tl2cgen-0.2.0/cpp_src/include/tl2cgen/detail/compiler/util/code_folding_util.h`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/include/tl2cgen/detail/compiler/util/format_util.h` & `tl2cgen-0.2.0/cpp_src/include/tl2cgen/detail/compiler/util/format_util.h`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/include/tl2cgen/detail/predictor/predictor_impl.h` & `tl2cgen-0.2.0/cpp_src/include/tl2cgen/detail/predictor/predictor_impl.h`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/include/tl2cgen/detail/predictor/shared_library.h` & `tl2cgen-0.2.0/cpp_src/include/tl2cgen/detail/predictor/shared_library.h`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/include/tl2cgen/detail/threading_utils/omp_config.h` & `tl2cgen-0.2.0/cpp_src/include/tl2cgen/detail/threading_utils/omp_config.h`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/include/tl2cgen/detail/threading_utils/omp_exception.h` & `tl2cgen-0.2.0/cpp_src/include/tl2cgen/detail/threading_utils/omp_exception.h`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/include/tl2cgen/detail/threading_utils/omp_funcs.h` & `tl2cgen-0.2.0/cpp_src/include/tl2cgen/detail/threading_utils/omp_funcs.h`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/include/tl2cgen/detail/threading_utils/parallel_for.h` & `tl2cgen-0.2.0/cpp_src/include/tl2cgen/detail/threading_utils/parallel_for.h`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/src/CMakeLists.txt` & `tl2cgen-0.2.0/cpp_src/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/src/annotator.cc` & `tl2cgen-0.2.0/cpp_src/src/annotator.cc`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/src/filesystem.cc` & `tl2cgen-0.2.0/cpp_src/src/filesystem.cc`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/src/logging.cc` & `tl2cgen-0.2.0/cpp_src/src/logging.cc`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/src/c_api/c_api.cc` & `tl2cgen-0.2.0/cpp_src/src/c_api/c_api.cc`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/src/c_api/c_api_error.cc` & `tl2cgen-0.2.0/cpp_src/src/c_api/c_api_error.cc`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/src/c_api/c_api_treelite_bridge.cc` & `tl2cgen-0.2.0/cpp_src/src/c_api/c_api_treelite_bridge.cc`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/src/compiler/ast_native.cc` & `tl2cgen-0.2.0/cpp_src/src/compiler/ast_native.cc`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/src/compiler/compiler.cc` & `tl2cgen-0.2.0/cpp_src/src/compiler/compiler.cc`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/src/compiler/elf_formatter.cc` & `tl2cgen-0.2.0/cpp_src/src/compiler/elf_formatter.cc`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/src/compiler/failsafe.cc` & `tl2cgen-0.2.0/cpp_src/src/compiler/failsafe.cc`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/src/compiler/pred_transform.cc` & `tl2cgen-0.2.0/cpp_src/src/compiler/pred_transform.cc`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/src/compiler/ast/builder/build.cc` & `tl2cgen-0.2.0/cpp_src/src/compiler/ast/builder/build.cc`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/src/compiler/ast/builder/dump.cc` & `tl2cgen-0.2.0/cpp_src/src/compiler/ast/builder/dump.cc`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/src/compiler/ast/builder/fold_code.cc` & `tl2cgen-0.2.0/cpp_src/src/compiler/ast/builder/fold_code.cc`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/src/compiler/ast/builder/is_categorical_array.cc` & `tl2cgen-0.2.0/cpp_src/src/compiler/ast/builder/is_categorical_array.cc`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/src/compiler/ast/builder/load_data_counts.cc` & `tl2cgen-0.2.0/cpp_src/src/compiler/ast/builder/load_data_counts.cc`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/src/compiler/ast/builder/quantize.cc` & `tl2cgen-0.2.0/cpp_src/src/compiler/ast/builder/quantize.cc`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/src/compiler/ast/builder/split.cc` & `tl2cgen-0.2.0/cpp_src/src/compiler/ast/builder/split.cc`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/src/compiler/templates/code_folder_template.cc` & `tl2cgen-0.2.0/cpp_src/src/compiler/templates/code_folder_template.cc`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/src/compiler/templates/header_template.cc` & `tl2cgen-0.2.0/cpp_src/src/compiler/templates/header_template.cc`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/src/compiler/templates/main_template.cc` & `tl2cgen-0.2.0/cpp_src/src/compiler/templates/main_template.cc`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/src/compiler/templates/pred_transform.cc` & `tl2cgen-0.2.0/cpp_src/src/compiler/templates/pred_transform.cc`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/src/compiler/templates/qnode_template.cc` & `tl2cgen-0.2.0/cpp_src/src/compiler/templates/qnode_template.cc`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/src/predictor/predictor.cc` & `tl2cgen-0.2.0/cpp_src/src/predictor/predictor.cc`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/cpp_src/src/predictor/shared_library.cc` & `tl2cgen-0.2.0/cpp_src/src/predictor/shared_library.cc`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/packager/build_config.py` & `tl2cgen-0.2.0/packager/build_config.py`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/packager/nativelib.py` & `tl2cgen-0.2.0/packager/nativelib.py`

 * *Files 14% similar despite different names*

```diff
@@ -130,24 +130,36 @@
     build_config: BuildConfiguration,
 ) -> pathlib.Path:
     """Locate libtl2cgen; if not exist, build it"""
     logger = logging.getLogger("tl2cgen.packager.locate_or_build_libtl2cgen")
 
     if build_config.use_system_libtl2cgen:
         # Find libtl2cgen from system prefix
-        sys_prefix = pathlib.Path(sys.prefix).absolute().resolve()
-        libtl2cgen_sys = sys_prefix / "lib" / _lib_name()
-        if not libtl2cgen_sys.exists():
-            raise RuntimeError(
-                f"use_system_libtl2cgen was specified but {_lib_name()} is "
-                f"not found in {libtl2cgen_sys.parent}"
-            )
-
-        logger.info("Using system tl2cgen: %s", str(libtl2cgen_sys))
-        return libtl2cgen_sys
+        sys_prefix = pathlib.Path(sys.prefix)
+        sys_prefix_candidates = [
+            sys_prefix / "lib",
+            # Paths possibly used on Windows
+            sys_prefix / "bin",
+            sys_prefix / "Library",
+            sys_prefix / "Library" / "bin",
+            sys_prefix / "Library" / "lib",
+        ]
+        sys_prefix_candidates = [
+            p.expanduser().resolve() for p in sys_prefix_candidates
+        ]
+        for candidate_dir in sys_prefix_candidates:
+            libtl2cgen_sys = candidate_dir / _lib_name()
+            if libtl2cgen_sys.exists():
+                logger.info("Using system tl2cgen: %s", str(libtl2cgen_sys))
+                return libtl2cgen_sys
+        raise RuntimeError(
+            f"use_system_libtl2cgen was specified but {_lib_name()} is "
+            f"not found. Paths searched (in order): \n"
+            + "\n".join([f"* {str(p)}" for p in sys_prefix_candidates])
+        )
 
     libtl2cgen = locate_local_libtl2cgen(toplevel_dir, logger=logger)
     if libtl2cgen is not None:
         return libtl2cgen
 
     if toplevel_dir.joinpath("cpp_src").exists():
         # Source distribution; all C++ source files to be found in cpp_src/
```

### Comparing `tl2cgen-0.1.0/packager/pep517.py` & `tl2cgen-0.2.0/packager/pep517.py`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/packager/sdist.py` & `tl2cgen-0.2.0/packager/sdist.py`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/packager/util.py` & `tl2cgen-0.2.0/packager/util.py`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/tl2cgen/__init__.py` & `tl2cgen-0.2.0/tl2cgen/__init__.py`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/tl2cgen/core.py` & `tl2cgen-0.2.0/tl2cgen/core.py`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/tl2cgen/create_shared.py` & `tl2cgen-0.2.0/tl2cgen/create_shared.py`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/tl2cgen/data.py` & `tl2cgen-0.2.0/tl2cgen/data.py`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/tl2cgen/dtypes.py` & `tl2cgen-0.2.0/tl2cgen/dtypes.py`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/tl2cgen/generate_makefile.py` & `tl2cgen-0.2.0/tl2cgen/generate_makefile.py`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/tl2cgen/handle_class.py` & `tl2cgen-0.2.0/tl2cgen/handle_class.py`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/tl2cgen/libloader.py` & `tl2cgen-0.2.0/tl2cgen/libloader.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # coding: utf-8
 """Find the path to TL2cgen dynamic library files."""
 
 import ctypes
 import os
 import pathlib
-import platform
 import sys
 import warnings
 from typing import List
 
 from .exception import TL2cgenError, TL2cgenLibraryNotFound
 from .util import py_str
 
@@ -19,29 +18,33 @@
     Returns
     -------
     lib_path
        List of all found library path to TL2cgen
     """
     curr_path = pathlib.Path(__file__).expanduser().absolute().parent
     dll_path = [
-        # When installed, libtreelite will be installed in <site-package-dir>/lib
+        # When installed, libtl2cgen will be installed in <site-package-dir>/lib
         curr_path / "lib",
         # Editable installation
         curr_path.parent.parent / "build",
-        # Use libtreelite from a system prefix, if available. This should be the last option.
-        pathlib.Path(sys.prefix).absolute().resolve() / "lib",
+        # Use libtl2cgen from a system prefix, if available. This should be the last option.
+        pathlib.Path(sys.prefix).expanduser().resolve() / "lib",
     ]
 
     if sys.platform == "win32":
-        if platform.architecture()[0] == "64bit":
-            dll_path.append(curr_path.joinpath("../../windows/x64/Release/"))
-            dll_path.append(curr_path.joinpath("./windows/x64/Release/"))
-        else:
-            dll_path.append(curr_path.joinpath("../../windows/Release/"))
-            dll_path.append(curr_path.joinpath("./windows/Release/"))
+        # On Windows, Conda may install libs in different paths
+        sys_prefix = pathlib.Path(sys.prefix)
+        dll_path.extend(
+            [
+                sys_prefix / "bin",
+                sys_prefix / "Library",
+                sys_prefix / "Library" / "bin",
+                sys_prefix / "Library" / "lib",
+            ]
+        )
         dll_path = [p.joinpath("tl2cgen.dll") for p in dll_path]
     elif sys.platform.startswith(("linux", "freebsd", "emscripten", "OS400")):
         dll_path = [p.joinpath("libtl2cgen.so") for p in dll_path]
     elif sys.platform == "darwin":
         dll_path = [p.joinpath("libtl2cgen.dylib") for p in dll_path]
     elif sys.platform == "cygwin":
         dll_path = [p.joinpath("cygtl2cgen.dll") for p in dll_path]
```

### Comparing `tl2cgen-0.1.0/tl2cgen/predictor.py` & `tl2cgen-0.2.0/tl2cgen/predictor.py`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/tl2cgen/shortcuts.py` & `tl2cgen-0.2.0/tl2cgen/shortcuts.py`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/tl2cgen/util.py` & `tl2cgen-0.2.0/tl2cgen/util.py`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/tl2cgen/contrib/create_shared.py` & `tl2cgen-0.2.0/tl2cgen/contrib/create_shared.py`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/tl2cgen/contrib/gcc.py` & `tl2cgen-0.2.0/tl2cgen/contrib/gcc.py`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/tl2cgen/contrib/msvc.py` & `tl2cgen-0.2.0/tl2cgen/contrib/msvc.py`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/tl2cgen/contrib/util.py` & `tl2cgen-0.2.0/tl2cgen/contrib/util.py`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/hatch_build.py` & `tl2cgen-0.2.0/hatch_build.py`

 * *Files identical despite different names*

### Comparing `tl2cgen-0.1.0/pyproject.toml` & `tl2cgen-0.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "hatchling>=1.12.1"
 ]
 backend-path = ["."]
 build-backend = "packager.pep517"
 
 [project]
 name = "tl2cgen"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
     {name = "Hyunsu Cho", email = "chohyu01@cs.washington.edu"}
 ]
 description = "TL2cgen: Compiler for decision tree models"
 readme = {file = "README.rst", content-type = "text/x-rst"}
 requires-python = ">=3.8"
 license = {text = "Apache-2.0"}
```

### Comparing `tl2cgen-0.1.0/PKG-INFO` & `tl2cgen-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tl2cgen
-Version: 0.1.0
+Version: 0.2.0
 Summary: TL2cgen: Compiler for decision tree models
 Project-URL: documentation, https://tl2cgen.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/dmlc/tl2cgen
 Author-email: Hyunsu Cho <chohyu01@cs.washington.edu>
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

