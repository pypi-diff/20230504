# Comparing `tmp/avio-2.1.3.tar.gz` & `tmp/avio-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avio-2.1.3.tar", last modified: Wed Apr 26 00:48:50 2023, max compression
+gzip compressed data, was "avio-2.1.4.tar", last modified: Wed May  3 23:56:16 2023, max compression
```

## Comparing `avio-2.1.3.tar` & `avio-2.1.4.tar`

### file list

```diff
@@ -1,324 +1,324 @@
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:48:49.997310 avio-2.1.3/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2798 2023-04-25 23:51:01.000000 avio-2.1.3/CMakeLists.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    11357 2023-04-25 23:51:01.000000 avio-2.1.3/LICENSE
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      147 2023-04-25 23:51:01.000000 avio-2.1.3/MANIFEST.in
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1854 2023-04-26 00:48:49.997310 avio-2.1.3/PKG-INFO
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1310 2023-04-25 23:51:01.000000 avio-2.1.3/README.md
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:48:49.973311 avio-2.1.3/cmake/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3496 2023-04-25 23:51:01.000000 avio-2.1.3/cmake/FindFFmpeg.cmake
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:48:49.973311 avio-2.1.3/include/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1251 2023-04-25 23:51:01.000000 avio-2.1.3/include/Clock.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2559 2023-04-25 23:51:01.000000 avio-2.1.3/include/Decoder.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3066 2023-04-25 23:51:01.000000 avio-2.1.3/include/Display.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2290 2023-04-25 23:51:01.000000 avio-2.1.3/include/Encoder.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2402 2023-04-25 23:51:01.000000 avio-2.1.3/include/Exception.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2719 2023-04-25 23:51:01.000000 avio-2.1.3/include/Filter.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1870 2023-04-25 23:51:01.000000 avio-2.1.3/include/Frame.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1249 2023-04-25 23:51:01.000000 avio-2.1.3/include/Packet.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1941 2023-04-25 23:51:01.000000 avio-2.1.3/include/Pipe.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4083 2023-04-25 23:51:01.000000 avio-2.1.3/include/Player.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5327 2023-04-25 23:51:01.000000 avio-2.1.3/include/Queue.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3071 2023-04-25 23:51:01.000000 avio-2.1.3/include/Reader.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1977 2023-04-25 23:51:01.000000 avio-2.1.3/include/Writer.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6747 2023-04-25 23:51:01.000000 avio-2.1.3/include/avio.h
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:48:49.977311 avio-2.1.3/pybind11/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1271 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/.appveyor.yml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      996 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/.clang-format
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2605 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/.clang-tidy
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2196 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/.cmake-format.yaml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1308 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/.codespell-ignore-lines
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       52 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/.git
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       18 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/.gitattributes
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:48:49.977311 avio-2.1.3/pybind11/.github/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      182 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/.github/CODEOWNERS
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    15284 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/.github/CONTRIBUTING.md
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:48:49.977311 avio-2.1.3/pybind11/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2561 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      328 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/.github/ISSUE_TEMPLATE/config.yml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      162 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/.github/dependabot.yml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      116 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/.github/labeler.yml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       50 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/.github/labeler_merged.yml
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:48:49.977311 avio-2.1.3/pybind11/.github/matchers/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      668 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/.github/matchers/pylint.json
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      645 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/.github/pull_request_template.md
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:48:49.977311 avio-2.1.3/pybind11/.github/workflows/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    32023 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/.github/workflows/ci.yml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2127 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/.github/workflows/configure.yml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1460 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/.github/workflows/format.yml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      559 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/.github/workflows/labeler.yml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2558 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/.github/workflows/pip.yml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2865 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/.github/workflows/upstream.yml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      502 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/.gitignore
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4332 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/.pre-commit-config.yaml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       62 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/.readthedocs.yml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    11983 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/CMakeLists.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1684 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/LICENSE
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      223 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/MANIFEST.in
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     7686 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/README.rst
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:48:49.977311 avio-2.1.3/pybind11/docs/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      607 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/docs/Doxyfile
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     7417 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/docs/Makefile
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:48:49.969311 avio-2.1.3/pybind11/docs/_static/
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:48:49.977311 avio-2.1.3/pybind11/docs/_static/css/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       37 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/docs/_static/css/custom.css
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:48:49.981310 avio-2.1.3/pybind11/docs/advanced/
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:48:49.981310 avio-2.1.3/pybind11/docs/advanced/cast/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3937 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/docs/advanced/cast/chrono.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3429 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/docs/advanced/cast/custom.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    14283 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/docs/advanced/cast/eigen.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3889 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/docs/advanced/cast/functional.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1556 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/docs/advanced/cast/index.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    12371 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/docs/advanced/cast/overview.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9586 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/docs/advanced/cast/stl.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8863 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/docs/advanced/cast/strings.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    47796 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/docs/advanced/classes.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8453 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/docs/advanced/embedding.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    17796 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/docs/advanced/exceptions.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    26729 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/docs/advanced/functions.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    15651 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/docs/advanced/misc.rst
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:48:49.981310 avio-2.1.3/pybind11/docs/advanced/pycpp/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      278 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/docs/advanced/pycpp/index.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    17161 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/docs/advanced/pycpp/numpy.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9030 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/docs/advanced/pycpp/object.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5710 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/docs/advanced/pycpp/utilities.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6377 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/docs/advanced/smart_ptrs.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9240 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/docs/basics.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2856 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/docs/benchmark.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3168 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/docs/benchmark.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)   114174 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/docs/changelog.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    16380 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/docs/classes.rst
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:48:49.981310 avio-2.1.3/pybind11/docs/cmake/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      273 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/docs/cmake/index.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    25777 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/docs/compiling.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    11559 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/docs/conf.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    13177 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/docs/faq.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      613 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/docs/index.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3277 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/docs/installing.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3079 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/docs/limitations.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    61034 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/docs/pybind11-logo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    44653 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/docs/pybind11_vs_boost_python1.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    87708 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/docs/pybind11_vs_boost_python1.svg
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    41121 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/docs/pybind11_vs_boost_python2.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    85853 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/docs/pybind11_vs_boost_python2.svg
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2647 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/docs/reference.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4414 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/docs/release.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      149 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/docs/requirements.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    23489 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/docs/upgrade.rst
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:48:49.969311 avio-2.1.3/pybind11/include/
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:48:49.981310 avio-2.1.3/pybind11/include/pybind11/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    23959 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/include/pybind11/attr.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     7069 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/include/pybind11/buffer_info.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    65660 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/include/pybind11/cast.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8458 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/include/pybind11/chrono.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      120 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/include/pybind11/common.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2096 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/include/pybind11/complex.h
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:48:49.985310 avio-2.1.3/pybind11/include/pybind11/detail/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    28251 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/include/pybind11/detail/class.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    52866 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/include/pybind11/detail/common.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5491 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/include/pybind11/detail/descr.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    17869 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/include/pybind11/detail/init.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    26498 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/include/pybind11/detail/internals.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    42613 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/include/pybind11/detail/type_caster_base.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1625 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/include/pybind11/detail/typeid.h
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:48:49.985310 avio-2.1.3/pybind11/include/pybind11/eigen/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    31418 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/include/pybind11/eigen/matrix.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    18108 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/include/pybind11/eigen/tensor.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      316 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/include/pybind11/eigen.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    13471 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/include/pybind11/embed.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4731 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/include/pybind11/eval.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5002 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/include/pybind11/functional.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8262 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/include/pybind11/gil.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8862 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/include/pybind11/iostream.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    79408 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/include/pybind11/numpy.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9103 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/include/pybind11/operators.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2734 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/include/pybind11/options.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)   126420 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/include/pybind11/pybind11.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    94641 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/include/pybind11/pytypes.h
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:48:49.985310 avio-2.1.3/pybind11/include/pybind11/stl/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4185 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/include/pybind11/stl/filesystem.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    15399 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/include/pybind11/stl.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    29824 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/include/pybind11/stl_bind.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2765 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/noxfile.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:48:49.985310 avio-2.1.3/pybind11/pybind11/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      414 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/pybind11/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1360 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/pybind11/__main__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      233 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/pybind11/_version.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1226 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/pybind11/commands.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/pybind11/py.typed
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    17609 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/pybind11/setup_helpers.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1261 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/pyproject.toml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1618 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/setup.cfg
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4877 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/setup.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:48:49.993310 avio-2.1.3/pybind11/tests/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    21675 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/CMakeLists.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5876 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/conftest.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    11736 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/constructor_stats.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3578 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/cross_module_gil_utils.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1776 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/cross_module_interleaved_error_already_set.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      396 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/eigen_tensor_avoid_stl_array.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      940 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/env.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:48:49.993310 avio-2.1.3/pybind11/tests/extra_python_package/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/extra_python_package/pytest.ini
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8296 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/extra_python_package/test_files.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:48:49.993310 avio-2.1.3/pybind11/tests/extra_setuptools/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/extra_setuptools/pytest.ini
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4153 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/extra_setuptools/test_setuphelper.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2847 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/local_bindings.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5743 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/object.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6264 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/pybind11_cross_module_tests.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4517 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/pybind11_tests.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2685 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/pybind11_tests.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      768 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/pytest.ini
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      600 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/requirements.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      855 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_async.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      534 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_async.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8567 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_buffers.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4841 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_buffers.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    16025 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_builtin_casters.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    17245 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_builtin_casters.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4118 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_call_policies.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6549 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_call_policies.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    10858 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_callbacks.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6246 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_callbacks.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3370 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_chrono.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5695 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_chrono.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    24874 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_class.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    14815 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_class.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:48:49.993310 avio-2.1.3/pybind11/tests/test_cmake_build/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2639 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_cmake_build/CMakeLists.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      673 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_cmake_build/embed.cpp
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:48:49.993310 avio-2.1.3/pybind11/tests/test_cmake_build/installed_embed/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1171 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:48:49.993310 avio-2.1.3/pybind11/tests/test_cmake_build/installed_function/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1293 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:48:49.993310 avio-2.1.3/pybind11/tests/test_cmake_build/installed_target/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1685 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      152 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_cmake_build/main.cpp
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:48:49.993310 avio-2.1.3/pybind11/tests/test_cmake_build/subdirectory_embed/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1353 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:48:49.993310 avio-2.1.3/pybind11/tests/test_cmake_build/subdirectory_function/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1163 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:48:49.993310 avio-2.1.3/pybind11/tests/test_cmake_build/subdirectory_target/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1368 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      198 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_cmake_build/test.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3831 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_const_name.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      589 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_const_name.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5615 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_constants_and_functions.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1498 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_constants_and_functions.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    10886 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_copy_move.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4796 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_copy_move.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     7280 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_custom_type_casters.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3980 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_custom_type_casters.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1259 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_custom_type_setup.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1089 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_custom_type_setup.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4557 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_docstring_options.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2423 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_docstring_options.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    19350 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_eigen_matrix.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    28867 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_eigen_matrix.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      473 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_eigen_tensor.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    10590 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_eigen_tensor.inl
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9456 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_eigen_tensor.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:48:49.997310 avio-2.1.3/pybind11/tests/test_embed/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1798 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_embed/CMakeLists.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1315 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_embed/catch.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      543 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_embed/external_module.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    16535 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_embed/test_interpreter.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      237 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_embed/test_interpreter.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      275 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_embed/test_trampoline.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5722 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_enum.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8903 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_enum.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3168 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_eval.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1143 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_eval.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      119 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_eval_call.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    11904 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_exceptions.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      399 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_exceptions.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    12774 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_exceptions.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    18155 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_factory_constructors.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    16519 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_factory_constructors.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5311 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_gil_scoped.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8540 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_gil_scoped.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3960 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_iostream.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     7286 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_iostream.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9444 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_kwargs_and_defaults.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    13757 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_kwargs_and_defaults.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4401 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_local_bindings.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8049 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_local_bindings.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    21388 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_methods_and_attributes.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    18134 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_methods_and_attributes.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4121 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_modules.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4191 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_modules.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    12305 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_multiple_inheritance.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    11874 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_multiple_inheritance.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    19861 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_numpy_array.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    20356 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_numpy_array.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    21114 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_numpy_dtypes.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    14394 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_numpy_dtypes.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4487 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_numpy_vectorize.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9686 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_numpy_vectorize.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2777 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_opaque_types.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1847 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_opaque_types.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9132 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_operator_overloading.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4333 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_operator_overloading.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6719 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_pickling.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2720 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_pickling.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    30750 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_pytypes.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    23630 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_pytypes.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    21153 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_sequences_and_iterators.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8021 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_sequences_and_iterators.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    18898 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_smart_ptr.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9530 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_smart_ptr.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    21587 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_stl.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    12235 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_stl.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4622 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_stl_binders.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9174 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_stl_binders.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4617 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_tagbased_polymorphic.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      741 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_tagbased_polymorphic.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1855 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_thread.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      826 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_thread.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      603 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_union.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      148 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_union.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    22991 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_virtual_functions.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    12919 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/test_virtual_functions.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3226 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/valgrind-numpy-scipy.supp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2657 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tests/valgrind-python.supp
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:48:49.997310 avio-2.1.3/pybind11/tools/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2350 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tools/FindCatch.cmake
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3105 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tools/FindEigen3.cmake
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    11190 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tools/FindPythonLibsNew.cmake
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      817 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tools/JoinPaths.cmake
--rwxrwxr-x   0 stephen   (1000) stephen   (1000)     1423 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tools/check-style.sh
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      952 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tools/cmake_uninstall.cmake.in
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1040 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tools/codespell_ignore_lines_from_errors.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1031 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tools/libsize.py
--rwxrwxr-x   0 stephen   (1000) stephen   (1000)     1311 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tools/make_changelog.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      196 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tools/pybind11.pc.in
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    14033 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tools/pybind11Common.cmake
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6930 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tools/pybind11Config.cmake.in
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8960 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tools/pybind11NewTools.cmake
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8361 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tools/pybind11Tools.cmake
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       94 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tools/pyproject.toml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2104 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tools/setup_global.py.in
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1234 2023-04-25 23:51:08.000000 avio-2.1.3/pybind11/tools/setup_main.py.in
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1351 2023-04-26 00:38:00.000000 avio-2.1.3/pyproject.toml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       38 2023-04-26 00:48:49.997310 avio-2.1.3/setup.cfg
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3072 2023-04-26 00:37:45.000000 avio-2.1.3/setup.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:48:49.997310 avio-2.1.3/src/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2189 2023-04-25 23:51:01.000000 avio-2.1.3/src/Clock.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8368 2023-04-25 23:51:01.000000 avio-2.1.3/src/Decoder.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    19976 2023-04-25 23:51:01.000000 avio-2.1.3/src/Display.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    11378 2023-04-25 23:51:01.000000 avio-2.1.3/src/Encoder.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6430 2023-04-25 23:51:01.000000 avio-2.1.3/src/Exception.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     7061 2023-04-25 23:51:01.000000 avio-2.1.3/src/Filter.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5768 2023-04-25 23:51:01.000000 avio-2.1.3/src/Frame.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2296 2023-04-25 23:51:01.000000 avio-2.1.3/src/Packet.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5126 2023-04-25 23:51:01.000000 avio-2.1.3/src/Pipe.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    11632 2023-04-25 23:51:01.000000 avio-2.1.3/src/Player.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    12986 2023-04-25 23:51:01.000000 avio-2.1.3/src/Reader.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3739 2023-04-25 23:51:01.000000 avio-2.1.3/src/Writer.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9604 2023-04-26 00:38:58.000000 avio-2.1.3/src/avio.cpp
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:48:49.997310 avio-2.1.3/src/avio.egg-info/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1854 2023-04-26 00:48:49.000000 avio-2.1.3/src/avio.egg-info/PKG-INFO
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9620 2023-04-26 00:48:49.000000 avio-2.1.3/src/avio.egg-info/SOURCES.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        1 2023-04-26 00:48:49.000000 avio-2.1.3/src/avio.egg-info/dependency_links.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        1 2023-04-26 00:37:30.000000 avio-2.1.3/src/avio.egg-info/not-zip-safe
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        5 2023-04-26 00:48:49.000000 avio-2.1.3/src/avio.egg-info/top_level.txt
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-03 23:56:16.988070 avio-2.1.4/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2798 2023-04-30 20:27:56.000000 avio-2.1.4/CMakeLists.txt
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    11357 2023-04-30 20:27:56.000000 avio-2.1.4/LICENSE
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      147 2023-04-30 20:27:56.000000 avio-2.1.4/MANIFEST.in
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1854 2023-05-03 23:56:16.988070 avio-2.1.4/PKG-INFO
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1310 2023-04-30 20:27:56.000000 avio-2.1.4/README.md
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-03 23:56:16.948070 avio-2.1.4/cmake/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     3496 2023-04-30 20:27:56.000000 avio-2.1.4/cmake/FindFFmpeg.cmake
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-03 23:56:16.948070 avio-2.1.4/include/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1251 2023-04-30 20:27:56.000000 avio-2.1.4/include/Clock.h
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2559 2023-04-30 20:27:56.000000 avio-2.1.4/include/Decoder.h
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     3142 2023-05-02 23:52:06.000000 avio-2.1.4/include/Display.h
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2290 2023-04-30 20:27:56.000000 avio-2.1.4/include/Encoder.h
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2402 2023-04-30 20:27:56.000000 avio-2.1.4/include/Exception.h
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2719 2023-04-30 20:27:56.000000 avio-2.1.4/include/Filter.h
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1968 2023-05-02 23:52:06.000000 avio-2.1.4/include/Frame.h
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1249 2023-04-30 20:27:56.000000 avio-2.1.4/include/Packet.h
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1941 2023-04-30 20:27:56.000000 avio-2.1.4/include/Pipe.h
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     4147 2023-05-02 23:52:06.000000 avio-2.1.4/include/Player.h
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5327 2023-04-30 20:27:56.000000 avio-2.1.4/include/Queue.h
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     3071 2023-04-30 20:27:56.000000 avio-2.1.4/include/Reader.h
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1977 2023-04-30 20:27:56.000000 avio-2.1.4/include/Writer.h
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     6747 2023-04-30 20:27:56.000000 avio-2.1.4/include/avio.h
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-03 23:56:16.952070 avio-2.1.4/pybind11/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1271 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/.appveyor.yml
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      996 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/.clang-format
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2605 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/.clang-tidy
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2196 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/.cmake-format.yaml
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1308 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/.codespell-ignore-lines
+-rw-r--r--   0 stephen   (1000) stephen   (1000)       52 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/.git
+-rw-r--r--   0 stephen   (1000) stephen   (1000)       18 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/.gitattributes
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-03 23:56:16.952070 avio-2.1.4/pybind11/.github/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      182 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/.github/CODEOWNERS
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    15284 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/.github/CONTRIBUTING.md
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-03 23:56:16.952070 avio-2.1.4/pybind11/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2561 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      328 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      162 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/.github/dependabot.yml
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      116 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/.github/labeler.yml
+-rw-r--r--   0 stephen   (1000) stephen   (1000)       50 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/.github/labeler_merged.yml
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-03 23:56:16.952070 avio-2.1.4/pybind11/.github/matchers/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      668 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/.github/matchers/pylint.json
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      645 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/.github/pull_request_template.md
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-03 23:56:16.952070 avio-2.1.4/pybind11/.github/workflows/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    32023 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/.github/workflows/ci.yml
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2127 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/.github/workflows/configure.yml
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1460 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/.github/workflows/format.yml
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      559 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/.github/workflows/labeler.yml
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2558 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/.github/workflows/pip.yml
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2865 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/.github/workflows/upstream.yml
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      502 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/.gitignore
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     4332 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/.pre-commit-config.yaml
+-rw-r--r--   0 stephen   (1000) stephen   (1000)       62 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/.readthedocs.yml
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    11983 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/CMakeLists.txt
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1684 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/LICENSE
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      223 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/MANIFEST.in
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     7686 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/README.rst
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-03 23:56:16.956070 avio-2.1.4/pybind11/docs/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      607 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/docs/Doxyfile
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     7417 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/docs/Makefile
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-03 23:56:16.944070 avio-2.1.4/pybind11/docs/_static/
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-03 23:56:16.956070 avio-2.1.4/pybind11/docs/_static/css/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)       37 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/docs/_static/css/custom.css
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-03 23:56:16.960070 avio-2.1.4/pybind11/docs/advanced/
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-03 23:56:16.960070 avio-2.1.4/pybind11/docs/advanced/cast/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     3937 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/docs/advanced/cast/chrono.rst
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     3429 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/docs/advanced/cast/custom.rst
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    14283 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/docs/advanced/cast/eigen.rst
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     3889 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/docs/advanced/cast/functional.rst
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1556 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/docs/advanced/cast/index.rst
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    12371 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/docs/advanced/cast/overview.rst
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     9586 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/docs/advanced/cast/stl.rst
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     8863 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/docs/advanced/cast/strings.rst
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    47796 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/docs/advanced/classes.rst
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     8453 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/docs/advanced/embedding.rst
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    17796 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/docs/advanced/exceptions.rst
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    26729 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/docs/advanced/functions.rst
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    15651 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/docs/advanced/misc.rst
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-03 23:56:16.960070 avio-2.1.4/pybind11/docs/advanced/pycpp/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      278 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/docs/advanced/pycpp/index.rst
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    17161 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/docs/advanced/pycpp/numpy.rst
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     9030 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/docs/advanced/pycpp/object.rst
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5710 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/docs/advanced/pycpp/utilities.rst
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     6377 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/docs/advanced/smart_ptrs.rst
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     9240 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/docs/basics.rst
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2856 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/docs/benchmark.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     3168 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/docs/benchmark.rst
+-rw-r--r--   0 stephen   (1000) stephen   (1000)   114174 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/docs/changelog.rst
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    16380 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/docs/classes.rst
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-03 23:56:16.960070 avio-2.1.4/pybind11/docs/cmake/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      273 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/docs/cmake/index.rst
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    25777 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/docs/compiling.rst
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    11559 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/docs/conf.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    13177 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/docs/faq.rst
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      613 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/docs/index.rst
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     3277 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/docs/installing.rst
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     3079 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/docs/limitations.rst
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    61034 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/docs/pybind11-logo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    44653 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/docs/pybind11_vs_boost_python1.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    87708 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/docs/pybind11_vs_boost_python1.svg
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    41121 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/docs/pybind11_vs_boost_python2.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    85853 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/docs/pybind11_vs_boost_python2.svg
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2647 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/docs/reference.rst
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     4414 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/docs/release.rst
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      149 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/docs/requirements.txt
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    23489 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/docs/upgrade.rst
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-03 23:56:16.944070 avio-2.1.4/pybind11/include/
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-03 23:56:16.964070 avio-2.1.4/pybind11/include/pybind11/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    23959 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     7069 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    65660 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     8458 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      120 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/include/pybind11/common.h
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2096 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-03 23:56:16.964070 avio-2.1.4/pybind11/include/pybind11/detail/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    28251 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    52866 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5491 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    17869 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    26498 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    42613 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1625 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/include/pybind11/detail/typeid.h
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-03 23:56:16.964070 avio-2.1.4/pybind11/include/pybind11/eigen/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    31418 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/include/pybind11/eigen/matrix.h
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    18108 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/include/pybind11/eigen/tensor.h
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      316 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    13471 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     4731 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5002 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     8262 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     8862 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    79408 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     9103 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2734 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/include/pybind11/options.h
+-rw-r--r--   0 stephen   (1000) stephen   (1000)   126420 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    94641 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/include/pybind11/pytypes.h
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-03 23:56:16.964070 avio-2.1.4/pybind11/include/pybind11/stl/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     4185 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    15399 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    29824 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/include/pybind11/stl_bind.h
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2765 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/noxfile.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-03 23:56:16.968070 avio-2.1.4/pybind11/pybind11/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      414 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/pybind11/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1360 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/pybind11/__main__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      233 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/pybind11/_version.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1226 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/pybind11/commands.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/pybind11/py.typed
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    17609 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/pybind11/setup_helpers.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1261 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/pyproject.toml
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1618 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/setup.cfg
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     4877 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/setup.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-03 23:56:16.984070 avio-2.1.4/pybind11/tests/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    21675 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/CMakeLists.txt
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5876 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/conftest.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    11736 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/constructor_stats.h
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     3578 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/cross_module_gil_utils.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1776 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/cross_module_interleaved_error_already_set.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      396 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/eigen_tensor_avoid_stl_array.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      940 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/env.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-03 23:56:16.984070 avio-2.1.4/pybind11/tests/extra_python_package/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/extra_python_package/pytest.ini
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     8296 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/extra_python_package/test_files.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-03 23:56:16.984070 avio-2.1.4/pybind11/tests/extra_setuptools/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/extra_setuptools/pytest.ini
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     4153 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/extra_setuptools/test_setuphelper.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2847 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/local_bindings.h
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5743 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/object.h
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     6264 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/pybind11_cross_module_tests.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     4517 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/pybind11_tests.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2685 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/pybind11_tests.h
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      768 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/pytest.ini
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      600 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/requirements.txt
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      855 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_async.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      534 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_async.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     8567 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_buffers.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     4841 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_buffers.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    16025 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_builtin_casters.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    17245 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_builtin_casters.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     4118 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_call_policies.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     6549 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_call_policies.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    10858 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_callbacks.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     6246 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_callbacks.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     3370 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_chrono.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5695 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_chrono.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    24874 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_class.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    14815 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_class.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-03 23:56:16.984070 avio-2.1.4/pybind11/tests/test_cmake_build/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2639 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_cmake_build/CMakeLists.txt
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      673 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_cmake_build/embed.cpp
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-03 23:56:16.984070 avio-2.1.4/pybind11/tests/test_cmake_build/installed_embed/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1171 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-03 23:56:16.984070 avio-2.1.4/pybind11/tests/test_cmake_build/installed_function/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1293 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-03 23:56:16.984070 avio-2.1.4/pybind11/tests/test_cmake_build/installed_target/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1685 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      152 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_cmake_build/main.cpp
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-03 23:56:16.984070 avio-2.1.4/pybind11/tests/test_cmake_build/subdirectory_embed/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1353 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-03 23:56:16.984070 avio-2.1.4/pybind11/tests/test_cmake_build/subdirectory_function/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1163 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-03 23:56:16.984070 avio-2.1.4/pybind11/tests/test_cmake_build/subdirectory_target/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1368 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      198 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_cmake_build/test.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     3831 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_const_name.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      589 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_const_name.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5615 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_constants_and_functions.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1498 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_constants_and_functions.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    10886 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_copy_move.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     4796 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_copy_move.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     7280 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_custom_type_casters.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     3980 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_custom_type_casters.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1259 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_custom_type_setup.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1089 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_custom_type_setup.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     4557 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_docstring_options.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2423 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_docstring_options.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    19350 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_eigen_matrix.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    28867 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_eigen_matrix.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      473 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_eigen_tensor.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    10590 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_eigen_tensor.inl
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     9456 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_eigen_tensor.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-03 23:56:16.984070 avio-2.1.4/pybind11/tests/test_embed/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1798 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_embed/CMakeLists.txt
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1315 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_embed/catch.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      543 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_embed/external_module.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    16535 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_embed/test_interpreter.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      237 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_embed/test_interpreter.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      275 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_embed/test_trampoline.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5722 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_enum.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     8903 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_enum.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     3168 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_eval.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1143 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_eval.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      119 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_eval_call.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    11904 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_exceptions.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      399 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_exceptions.h
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    12774 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_exceptions.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    18155 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_factory_constructors.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    16519 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_factory_constructors.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5311 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_gil_scoped.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     8540 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_gil_scoped.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     3960 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_iostream.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     7286 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_iostream.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     9444 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_kwargs_and_defaults.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    13757 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_kwargs_and_defaults.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     4401 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_local_bindings.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     8049 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_local_bindings.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    21388 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_methods_and_attributes.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    18134 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_methods_and_attributes.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     4121 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_modules.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     4191 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_modules.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    12305 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_multiple_inheritance.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    11874 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_multiple_inheritance.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    19861 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_numpy_array.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    20356 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_numpy_array.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    21114 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_numpy_dtypes.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    14394 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_numpy_dtypes.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     4487 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_numpy_vectorize.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     9686 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_numpy_vectorize.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2777 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_opaque_types.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1847 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_opaque_types.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     9132 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_operator_overloading.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     4333 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_operator_overloading.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     6719 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_pickling.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2720 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_pickling.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    30750 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_pytypes.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    23630 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_pytypes.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    21153 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_sequences_and_iterators.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     8021 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_sequences_and_iterators.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    18898 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_smart_ptr.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     9530 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_smart_ptr.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    21587 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_stl.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    12235 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_stl.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     4622 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_stl_binders.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     9174 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_stl_binders.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     4617 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_tagbased_polymorphic.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      741 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_tagbased_polymorphic.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1855 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_thread.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      826 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_thread.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      603 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_union.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      148 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_union.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    22991 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_virtual_functions.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    12919 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/test_virtual_functions.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     3226 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/valgrind-numpy-scipy.supp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2657 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tests/valgrind-python.supp
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-03 23:56:16.988070 avio-2.1.4/pybind11/tools/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2350 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     3105 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    11190 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tools/FindPythonLibsNew.cmake
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      817 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tools/JoinPaths.cmake
+-rwxr-xr-x   0 stephen   (1000) stephen   (1000)     1423 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tools/check-style.sh
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      952 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tools/cmake_uninstall.cmake.in
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1040 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tools/codespell_ignore_lines_from_errors.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1031 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tools/libsize.py
+-rwxr-xr-x   0 stephen   (1000) stephen   (1000)     1311 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tools/make_changelog.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      196 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tools/pybind11.pc.in
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    14033 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     6930 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tools/pybind11Config.cmake.in
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     8960 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     8361 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tools/pybind11Tools.cmake
+-rw-r--r--   0 stephen   (1000) stephen   (1000)       94 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tools/pyproject.toml
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2104 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tools/setup_global.py.in
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1234 2023-04-30 20:27:59.000000 avio-2.1.4/pybind11/tools/setup_main.py.in
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1351 2023-05-03 23:38:29.000000 avio-2.1.4/pyproject.toml
+-rw-r--r--   0 stephen   (1000) stephen   (1000)       38 2023-05-03 23:56:16.992070 avio-2.1.4/setup.cfg
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     3072 2023-05-03 23:38:19.000000 avio-2.1.4/setup.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-03 23:56:16.988070 avio-2.1.4/src/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2189 2023-04-30 20:27:56.000000 avio-2.1.4/src/Clock.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     8368 2023-04-30 20:27:56.000000 avio-2.1.4/src/Decoder.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    20495 2023-05-02 23:52:06.000000 avio-2.1.4/src/Display.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    11378 2023-04-30 20:27:56.000000 avio-2.1.4/src/Encoder.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     6430 2023-04-30 20:27:56.000000 avio-2.1.4/src/Exception.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     7061 2023-04-30 20:27:56.000000 avio-2.1.4/src/Filter.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     6318 2023-05-02 23:52:06.000000 avio-2.1.4/src/Frame.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2296 2023-04-30 20:27:56.000000 avio-2.1.4/src/Packet.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5126 2023-04-30 20:27:56.000000 avio-2.1.4/src/Pipe.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    11632 2023-04-30 20:27:56.000000 avio-2.1.4/src/Player.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    12986 2023-04-30 20:27:56.000000 avio-2.1.4/src/Reader.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     3739 2023-04-30 20:27:56.000000 avio-2.1.4/src/Writer.cpp
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    10395 2023-05-03 23:41:28.000000 avio-2.1.4/src/avio.cpp
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-03 23:56:16.988070 avio-2.1.4/src/avio.egg-info/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1854 2023-05-03 23:56:16.000000 avio-2.1.4/src/avio.egg-info/PKG-INFO
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     9620 2023-05-03 23:56:16.000000 avio-2.1.4/src/avio.egg-info/SOURCES.txt
+-rw-r--r--   0 stephen   (1000) stephen   (1000)        1 2023-05-03 23:56:16.000000 avio-2.1.4/src/avio.egg-info/dependency_links.txt
+-rw-r--r--   0 stephen   (1000) stephen   (1000)        1 2023-05-02 23:52:39.000000 avio-2.1.4/src/avio.egg-info/not-zip-safe
+-rw-r--r--   0 stephen   (1000) stephen   (1000)        5 2023-05-03 23:56:16.000000 avio-2.1.4/src/avio.egg-info/top_level.txt
```

### Comparing `avio-2.1.3/CMakeLists.txt` & `avio-2.1.4/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/LICENSE` & `avio-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/PKG-INFO` & `avio-2.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avio
-Version: 2.1.3
+Version: 2.1.4
 Summary: A python module for processing media streams
 Author: Stephen Rhodes
 Author-email: Stephen Rhodes <sr99622@gmail.com>
 Project-URL: Homepage, https://github.com/sr99622/libavio
 Project-URL: Bug Tracker, https://github.com/sr99622/libavio/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `avio-2.1.3/README.md` & `avio-2.1.4/README.md`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/cmake/FindFFmpeg.cmake` & `avio-2.1.4/cmake/FindFFmpeg.cmake`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/include/Clock.h` & `avio-2.1.4/include/Clock.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/include/Decoder.h` & `avio-2.1.4/include/Decoder.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/include/Display.h` & `avio-2.1.4/include/Display.h`

 * *Files 3% similar despite different names*

```diff
@@ -101,14 +101,17 @@
 
     uint8_t* swr_buffer = nullptr;
     int swr_buffer_size = 0;
     int audio_buffer_len = 0;
     bool audio_eof = false;
     float volume = 1.0f;
     bool mute = false;
+    int swr_ptr = 0;
+    bool first_pass = true;
+    int pass_count = 0;
 
     int win_width = 0;
     int win_height = 0;
     int pix_width = 0;
     int pix_height = 0;
     AVPixelFormat pix_fmt = AV_PIX_FMT_NONE;
```

### Comparing `avio-2.1.3/include/Encoder.h` & `avio-2.1.4/include/Encoder.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/include/Exception.h` & `avio-2.1.4/include/Exception.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/include/Filter.h` & `avio-2.1.4/include/Filter.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/include/Frame.h` & `avio-2.1.4/include/Frame.h`

 * *Files 12% similar despite different names*

```diff
@@ -51,14 +51,19 @@
 	void set_rts(AVStream* stream);  // called from Decoder::decode
 	void set_pts(AVStream* stream);  // called from Encoder::encode
 	std::string description() const;
 	uint8_t* data();
 	int width();
 	int height();
 	int stride();
+	int nb_samples();
+	int sample_rate();
+	int64_t channels();
+	int format();
+	bool isPlanar();
 
 	AVFrame* m_frame = nullptr;
 	uint64_t m_rts;
 	bool m_faded = false;  // used by osd to avoid duplicate background fade
 
 };
```

### Comparing `avio-2.1.3/include/Packet.h` & `avio-2.1.4/include/Packet.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/include/Pipe.h` & `avio-2.1.4/include/Pipe.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/include/Player.h` & `avio-2.1.4/include/Player.h`

 * *Files 3% similar despite different names*

```diff
@@ -61,18 +61,19 @@
     Queue<Frame>*  afq_display;
 
     std::function<int(void)> width = nullptr;
     std::function<int(void)> height = nullptr;
     std::function<void(float)> progressCallback = nullptr;
     std::function<void(const Frame&)> renderCallback = nullptr;
     std::function<Frame(Frame&)> pythonCallback  = nullptr;
+    std::function<Frame(Frame&)> pyAudioCallback = nullptr;
     std::function<void(int64_t)> cbMediaPlayingStarted = nullptr;
     std::function<void(void)> cbMediaPlayingStopped = nullptr;
-  	std::function<void(const std::string&)> infoCallback = nullptr;
-	std::function<void(const std::string&)> errorCallback = nullptr;
+    std::function<void(const std::string&)> infoCallback = nullptr;
+    std::function<void(const std::string&)> errorCallback = nullptr;
 
     uint64_t hWnd = 0;
     std::string uri;
     std::string video_filter = "null";
     std::string audio_filter = "anull";
     AVHWDeviceType hw_device_type = AV_HWDEVICE_TYPE_NONE;
```

### Comparing `avio-2.1.3/include/Queue.h` & `avio-2.1.4/include/Queue.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/include/Reader.h` & `avio-2.1.4/include/Reader.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/include/Writer.h` & `avio-2.1.4/include/Writer.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/include/avio.h` & `avio-2.1.4/include/avio.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/.appveyor.yml` & `avio-2.1.4/pybind11/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/.clang-format` & `avio-2.1.4/pybind11/.clang-format`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/.clang-tidy` & `avio-2.1.4/pybind11/.clang-tidy`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/.cmake-format.yaml` & `avio-2.1.4/pybind11/.cmake-format.yaml`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/.codespell-ignore-lines` & `avio-2.1.4/pybind11/.codespell-ignore-lines`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/.github/CONTRIBUTING.md` & `avio-2.1.4/pybind11/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml` & `avio-2.1.4/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/.github/matchers/pylint.json` & `avio-2.1.4/pybind11/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/.github/pull_request_template.md` & `avio-2.1.4/pybind11/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/.github/workflows/ci.yml` & `avio-2.1.4/pybind11/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/.github/workflows/configure.yml` & `avio-2.1.4/pybind11/.github/workflows/configure.yml`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/.github/workflows/format.yml` & `avio-2.1.4/pybind11/.github/workflows/format.yml`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/.github/workflows/labeler.yml` & `avio-2.1.4/pybind11/.github/workflows/labeler.yml`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/.github/workflows/pip.yml` & `avio-2.1.4/pybind11/.github/workflows/pip.yml`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/.github/workflows/upstream.yml` & `avio-2.1.4/pybind11/.github/workflows/upstream.yml`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/.pre-commit-config.yaml` & `avio-2.1.4/pybind11/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/CMakeLists.txt` & `avio-2.1.4/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/LICENSE` & `avio-2.1.4/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/README.rst` & `avio-2.1.4/pybind11/README.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/docs/Doxyfile` & `avio-2.1.4/pybind11/docs/Doxyfile`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/docs/Makefile` & `avio-2.1.4/pybind11/docs/Makefile`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/docs/advanced/cast/chrono.rst` & `avio-2.1.4/pybind11/docs/advanced/cast/chrono.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/docs/advanced/cast/custom.rst` & `avio-2.1.4/pybind11/docs/advanced/cast/custom.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/docs/advanced/cast/eigen.rst` & `avio-2.1.4/pybind11/docs/advanced/cast/eigen.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/docs/advanced/cast/functional.rst` & `avio-2.1.4/pybind11/docs/advanced/cast/functional.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/docs/advanced/cast/index.rst` & `avio-2.1.4/pybind11/docs/advanced/cast/index.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/docs/advanced/cast/overview.rst` & `avio-2.1.4/pybind11/docs/advanced/cast/overview.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/docs/advanced/cast/stl.rst` & `avio-2.1.4/pybind11/docs/advanced/cast/stl.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/docs/advanced/cast/strings.rst` & `avio-2.1.4/pybind11/docs/advanced/cast/strings.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/docs/advanced/classes.rst` & `avio-2.1.4/pybind11/docs/advanced/classes.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/docs/advanced/embedding.rst` & `avio-2.1.4/pybind11/docs/advanced/embedding.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/docs/advanced/exceptions.rst` & `avio-2.1.4/pybind11/docs/advanced/exceptions.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/docs/advanced/functions.rst` & `avio-2.1.4/pybind11/docs/advanced/functions.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/docs/advanced/misc.rst` & `avio-2.1.4/pybind11/docs/advanced/misc.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/docs/advanced/pycpp/numpy.rst` & `avio-2.1.4/pybind11/docs/advanced/pycpp/numpy.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/docs/advanced/pycpp/object.rst` & `avio-2.1.4/pybind11/docs/advanced/pycpp/object.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/docs/advanced/pycpp/utilities.rst` & `avio-2.1.4/pybind11/docs/advanced/pycpp/utilities.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/docs/advanced/smart_ptrs.rst` & `avio-2.1.4/pybind11/docs/advanced/smart_ptrs.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/docs/basics.rst` & `avio-2.1.4/pybind11/docs/basics.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/docs/benchmark.py` & `avio-2.1.4/pybind11/docs/benchmark.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/docs/benchmark.rst` & `avio-2.1.4/pybind11/docs/benchmark.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/docs/changelog.rst` & `avio-2.1.4/pybind11/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/docs/classes.rst` & `avio-2.1.4/pybind11/docs/classes.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/docs/compiling.rst` & `avio-2.1.4/pybind11/docs/compiling.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/docs/conf.py` & `avio-2.1.4/pybind11/docs/conf.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/docs/faq.rst` & `avio-2.1.4/pybind11/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/docs/index.rst` & `avio-2.1.4/pybind11/docs/index.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/docs/installing.rst` & `avio-2.1.4/pybind11/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/docs/limitations.rst` & `avio-2.1.4/pybind11/docs/limitations.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/docs/pybind11-logo.png` & `avio-2.1.4/pybind11/docs/pybind11-logo.png`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/docs/pybind11_vs_boost_python1.png` & `avio-2.1.4/pybind11/docs/pybind11_vs_boost_python1.png`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/docs/pybind11_vs_boost_python1.svg` & `avio-2.1.4/pybind11/docs/pybind11_vs_boost_python1.svg`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/docs/pybind11_vs_boost_python2.png` & `avio-2.1.4/pybind11/docs/pybind11_vs_boost_python2.png`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/docs/pybind11_vs_boost_python2.svg` & `avio-2.1.4/pybind11/docs/pybind11_vs_boost_python2.svg`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/docs/reference.rst` & `avio-2.1.4/pybind11/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/docs/release.rst` & `avio-2.1.4/pybind11/docs/release.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/docs/upgrade.rst` & `avio-2.1.4/pybind11/docs/upgrade.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/include/pybind11/attr.h` & `avio-2.1.4/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/include/pybind11/buffer_info.h` & `avio-2.1.4/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/include/pybind11/cast.h` & `avio-2.1.4/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/include/pybind11/chrono.h` & `avio-2.1.4/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/include/pybind11/complex.h` & `avio-2.1.4/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/include/pybind11/detail/class.h` & `avio-2.1.4/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/include/pybind11/detail/common.h` & `avio-2.1.4/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/include/pybind11/detail/descr.h` & `avio-2.1.4/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/include/pybind11/detail/init.h` & `avio-2.1.4/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/include/pybind11/detail/internals.h` & `avio-2.1.4/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/include/pybind11/detail/type_caster_base.h` & `avio-2.1.4/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/include/pybind11/detail/typeid.h` & `avio-2.1.4/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/include/pybind11/eigen/matrix.h` & `avio-2.1.4/pybind11/include/pybind11/eigen/matrix.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/include/pybind11/eigen/tensor.h` & `avio-2.1.4/pybind11/include/pybind11/eigen/tensor.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/include/pybind11/embed.h` & `avio-2.1.4/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/include/pybind11/eval.h` & `avio-2.1.4/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/include/pybind11/functional.h` & `avio-2.1.4/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/include/pybind11/gil.h` & `avio-2.1.4/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/include/pybind11/iostream.h` & `avio-2.1.4/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/include/pybind11/numpy.h` & `avio-2.1.4/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/include/pybind11/operators.h` & `avio-2.1.4/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/include/pybind11/options.h` & `avio-2.1.4/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/include/pybind11/pybind11.h` & `avio-2.1.4/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/include/pybind11/pytypes.h` & `avio-2.1.4/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/include/pybind11/stl/filesystem.h` & `avio-2.1.4/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/include/pybind11/stl.h` & `avio-2.1.4/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/include/pybind11/stl_bind.h` & `avio-2.1.4/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/noxfile.py` & `avio-2.1.4/pybind11/noxfile.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/pybind11/__main__.py` & `avio-2.1.4/pybind11/pybind11/__main__.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/pybind11/commands.py` & `avio-2.1.4/pybind11/pybind11/commands.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/pybind11/setup_helpers.py` & `avio-2.1.4/pybind11/pybind11/setup_helpers.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/pyproject.toml` & `avio-2.1.4/pybind11/pyproject.toml`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/setup.cfg` & `avio-2.1.4/pybind11/setup.cfg`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/setup.py` & `avio-2.1.4/pybind11/setup.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/CMakeLists.txt` & `avio-2.1.4/pybind11/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/conftest.py` & `avio-2.1.4/pybind11/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/constructor_stats.h` & `avio-2.1.4/pybind11/tests/constructor_stats.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/cross_module_gil_utils.cpp` & `avio-2.1.4/pybind11/tests/cross_module_gil_utils.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/cross_module_interleaved_error_already_set.cpp` & `avio-2.1.4/pybind11/tests/cross_module_interleaved_error_already_set.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/env.py` & `avio-2.1.4/pybind11/tests/env.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/extra_python_package/test_files.py` & `avio-2.1.4/pybind11/tests/extra_python_package/test_files.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/extra_setuptools/test_setuphelper.py` & `avio-2.1.4/pybind11/tests/extra_setuptools/test_setuphelper.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/local_bindings.h` & `avio-2.1.4/pybind11/tests/local_bindings.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/object.h` & `avio-2.1.4/pybind11/tests/object.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/pybind11_cross_module_tests.cpp` & `avio-2.1.4/pybind11/tests/pybind11_cross_module_tests.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/pybind11_tests.cpp` & `avio-2.1.4/pybind11/tests/pybind11_tests.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/pybind11_tests.h` & `avio-2.1.4/pybind11/tests/pybind11_tests.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/pytest.ini` & `avio-2.1.4/pybind11/tests/pytest.ini`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/requirements.txt` & `avio-2.1.4/pybind11/tests/requirements.txt`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_async.cpp` & `avio-2.1.4/pybind11/tests/test_async.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_async.py` & `avio-2.1.4/pybind11/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_buffers.cpp` & `avio-2.1.4/pybind11/tests/test_buffers.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_buffers.py` & `avio-2.1.4/pybind11/tests/test_buffers.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_builtin_casters.cpp` & `avio-2.1.4/pybind11/tests/test_builtin_casters.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_builtin_casters.py` & `avio-2.1.4/pybind11/tests/test_builtin_casters.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_call_policies.cpp` & `avio-2.1.4/pybind11/tests/test_call_policies.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_call_policies.py` & `avio-2.1.4/pybind11/tests/test_call_policies.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_callbacks.cpp` & `avio-2.1.4/pybind11/tests/test_callbacks.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_callbacks.py` & `avio-2.1.4/pybind11/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_chrono.cpp` & `avio-2.1.4/pybind11/tests/test_chrono.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_chrono.py` & `avio-2.1.4/pybind11/tests/test_chrono.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_class.cpp` & `avio-2.1.4/pybind11/tests/test_class.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_class.py` & `avio-2.1.4/pybind11/tests/test_class.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_cmake_build/CMakeLists.txt` & `avio-2.1.4/pybind11/tests/test_cmake_build/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_cmake_build/embed.cpp` & `avio-2.1.4/pybind11/tests/test_cmake_build/embed.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt` & `avio-2.1.4/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt` & `avio-2.1.4/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt` & `avio-2.1.4/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt` & `avio-2.1.4/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt` & `avio-2.1.4/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt` & `avio-2.1.4/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_const_name.cpp` & `avio-2.1.4/pybind11/tests/test_const_name.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_const_name.py` & `avio-2.1.4/pybind11/tests/test_const_name.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_constants_and_functions.cpp` & `avio-2.1.4/pybind11/tests/test_constants_and_functions.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_constants_and_functions.py` & `avio-2.1.4/pybind11/tests/test_constants_and_functions.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_copy_move.cpp` & `avio-2.1.4/pybind11/tests/test_copy_move.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_copy_move.py` & `avio-2.1.4/pybind11/tests/test_copy_move.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_custom_type_casters.cpp` & `avio-2.1.4/pybind11/tests/test_custom_type_casters.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_custom_type_casters.py` & `avio-2.1.4/pybind11/tests/test_custom_type_casters.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_custom_type_setup.cpp` & `avio-2.1.4/pybind11/tests/test_custom_type_setup.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_custom_type_setup.py` & `avio-2.1.4/pybind11/tests/test_custom_type_setup.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_docstring_options.cpp` & `avio-2.1.4/pybind11/tests/test_docstring_options.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_docstring_options.py` & `avio-2.1.4/pybind11/tests/test_docstring_options.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_eigen_matrix.cpp` & `avio-2.1.4/pybind11/tests/test_eigen_matrix.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_eigen_matrix.py` & `avio-2.1.4/pybind11/tests/test_eigen_matrix.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_eigen_tensor.inl` & `avio-2.1.4/pybind11/tests/test_eigen_tensor.inl`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_eigen_tensor.py` & `avio-2.1.4/pybind11/tests/test_eigen_tensor.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_embed/CMakeLists.txt` & `avio-2.1.4/pybind11/tests/test_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_embed/catch.cpp` & `avio-2.1.4/pybind11/tests/test_embed/catch.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_embed/external_module.cpp` & `avio-2.1.4/pybind11/tests/test_embed/external_module.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_embed/test_interpreter.cpp` & `avio-2.1.4/pybind11/tests/test_embed/test_interpreter.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_enum.cpp` & `avio-2.1.4/pybind11/tests/test_enum.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_enum.py` & `avio-2.1.4/pybind11/tests/test_enum.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_eval.cpp` & `avio-2.1.4/pybind11/tests/test_eval.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_eval.py` & `avio-2.1.4/pybind11/tests/test_eval.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_exceptions.cpp` & `avio-2.1.4/pybind11/tests/test_exceptions.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_exceptions.py` & `avio-2.1.4/pybind11/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_factory_constructors.cpp` & `avio-2.1.4/pybind11/tests/test_factory_constructors.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_factory_constructors.py` & `avio-2.1.4/pybind11/tests/test_factory_constructors.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_gil_scoped.cpp` & `avio-2.1.4/pybind11/tests/test_gil_scoped.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_gil_scoped.py` & `avio-2.1.4/pybind11/tests/test_gil_scoped.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_iostream.cpp` & `avio-2.1.4/pybind11/tests/test_iostream.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_iostream.py` & `avio-2.1.4/pybind11/tests/test_iostream.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_kwargs_and_defaults.cpp` & `avio-2.1.4/pybind11/tests/test_kwargs_and_defaults.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_kwargs_and_defaults.py` & `avio-2.1.4/pybind11/tests/test_kwargs_and_defaults.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_local_bindings.cpp` & `avio-2.1.4/pybind11/tests/test_local_bindings.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_local_bindings.py` & `avio-2.1.4/pybind11/tests/test_local_bindings.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_methods_and_attributes.cpp` & `avio-2.1.4/pybind11/tests/test_methods_and_attributes.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_methods_and_attributes.py` & `avio-2.1.4/pybind11/tests/test_methods_and_attributes.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_modules.cpp` & `avio-2.1.4/pybind11/tests/test_modules.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_modules.py` & `avio-2.1.4/pybind11/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_multiple_inheritance.cpp` & `avio-2.1.4/pybind11/tests/test_multiple_inheritance.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_multiple_inheritance.py` & `avio-2.1.4/pybind11/tests/test_multiple_inheritance.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_numpy_array.cpp` & `avio-2.1.4/pybind11/tests/test_numpy_array.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_numpy_array.py` & `avio-2.1.4/pybind11/tests/test_numpy_array.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_numpy_dtypes.cpp` & `avio-2.1.4/pybind11/tests/test_numpy_dtypes.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_numpy_dtypes.py` & `avio-2.1.4/pybind11/tests/test_numpy_dtypes.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_numpy_vectorize.cpp` & `avio-2.1.4/pybind11/tests/test_numpy_vectorize.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_numpy_vectorize.py` & `avio-2.1.4/pybind11/tests/test_numpy_vectorize.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_opaque_types.cpp` & `avio-2.1.4/pybind11/tests/test_opaque_types.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_opaque_types.py` & `avio-2.1.4/pybind11/tests/test_opaque_types.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_operator_overloading.cpp` & `avio-2.1.4/pybind11/tests/test_operator_overloading.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_operator_overloading.py` & `avio-2.1.4/pybind11/tests/test_operator_overloading.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_pickling.cpp` & `avio-2.1.4/pybind11/tests/test_pickling.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_pickling.py` & `avio-2.1.4/pybind11/tests/test_pickling.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_pytypes.cpp` & `avio-2.1.4/pybind11/tests/test_pytypes.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_pytypes.py` & `avio-2.1.4/pybind11/tests/test_pytypes.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_sequences_and_iterators.cpp` & `avio-2.1.4/pybind11/tests/test_sequences_and_iterators.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_sequences_and_iterators.py` & `avio-2.1.4/pybind11/tests/test_sequences_and_iterators.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_smart_ptr.cpp` & `avio-2.1.4/pybind11/tests/test_smart_ptr.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_smart_ptr.py` & `avio-2.1.4/pybind11/tests/test_smart_ptr.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_stl.cpp` & `avio-2.1.4/pybind11/tests/test_stl.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_stl.py` & `avio-2.1.4/pybind11/tests/test_stl.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_stl_binders.cpp` & `avio-2.1.4/pybind11/tests/test_stl_binders.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_stl_binders.py` & `avio-2.1.4/pybind11/tests/test_stl_binders.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_tagbased_polymorphic.cpp` & `avio-2.1.4/pybind11/tests/test_tagbased_polymorphic.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_tagbased_polymorphic.py` & `avio-2.1.4/pybind11/tests/test_tagbased_polymorphic.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_thread.cpp` & `avio-2.1.4/pybind11/tests/test_thread.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_thread.py` & `avio-2.1.4/pybind11/tests/test_thread.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_union.cpp` & `avio-2.1.4/pybind11/tests/test_union.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_virtual_functions.cpp` & `avio-2.1.4/pybind11/tests/test_virtual_functions.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/test_virtual_functions.py` & `avio-2.1.4/pybind11/tests/test_virtual_functions.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/valgrind-numpy-scipy.supp` & `avio-2.1.4/pybind11/tests/valgrind-numpy-scipy.supp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tests/valgrind-python.supp` & `avio-2.1.4/pybind11/tests/valgrind-python.supp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tools/FindCatch.cmake` & `avio-2.1.4/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tools/FindEigen3.cmake` & `avio-2.1.4/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tools/FindPythonLibsNew.cmake` & `avio-2.1.4/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tools/JoinPaths.cmake` & `avio-2.1.4/pybind11/tools/JoinPaths.cmake`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tools/check-style.sh` & `avio-2.1.4/pybind11/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tools/cmake_uninstall.cmake.in` & `avio-2.1.4/pybind11/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tools/codespell_ignore_lines_from_errors.py` & `avio-2.1.4/pybind11/tools/codespell_ignore_lines_from_errors.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tools/libsize.py` & `avio-2.1.4/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tools/make_changelog.py` & `avio-2.1.4/pybind11/tools/make_changelog.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tools/pybind11Common.cmake` & `avio-2.1.4/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tools/pybind11Config.cmake.in` & `avio-2.1.4/pybind11/tools/pybind11Config.cmake.in`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tools/pybind11NewTools.cmake` & `avio-2.1.4/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tools/pybind11Tools.cmake` & `avio-2.1.4/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tools/setup_global.py.in` & `avio-2.1.4/pybind11/tools/setup_global.py.in`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pybind11/tools/setup_main.py.in` & `avio-2.1.4/pybind11/tools/setup_main.py.in`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/pyproject.toml` & `avio-2.1.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "avio"
-version = "2.1.3"
+version = "2.1.4"
 authors = [
     { name="Stephen Rhodes", email="sr99622@gmail.com" },
 ]
 description = "A python module for processing media streams"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `avio-2.1.3/setup.py` & `avio-2.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
             os.makedirs(build_temp)
 
         subprocess.run(["cmake", ext.sourcedir] + cmake_args, cwd=build_temp)
         subprocess.run(["cmake", "--build", "."] + build_args, cwd=build_temp)
 
 setup(
     name="avio",
-    version="2.1.3",
+    version="2.1.4",
     author="Stephen Rhodes",
     author_email="sr99622@gmail.com",
     description="A python media processing module",
     long_description="",
     ext_modules=[CMakeExtension("avio")],
     cmdclass={"build_ext": CMakeBuild},
     zip_safe=False,
```

### Comparing `avio-2.1.3/src/Clock.cpp` & `avio-2.1.4/src/Clock.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/src/Decoder.cpp` & `avio-2.1.4/src/Decoder.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/src/Display.cpp` & `avio-2.1.4/src/Display.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -369,42 +369,62 @@
 void Display::AudioCallback(void* userdata, uint8_t* audio_buffer, int len)
 {
     Display* d = (Display*)userdata;
     memset(audio_buffer, 0, len);
     uint8_t* temp = (uint8_t*)malloc(len);
     memset(temp, 0, len);
     Frame f;
-    int ptr = 0;
     Player* player = (Player*)d->player;
 
     if (d->paused)
         return;
 
     try {
         while (len > 0) {
-            if (ptr < d->audio_buffer_len) {
+            if (!d->swr_ptr) {
+
                 d->afq_in->pop_move(f);
 
+                if (player->pyAudioCallback) f = player->pyAudioCallback(f);
+
                 if (f.isValid()) {
                     uint64_t channels = f.m_frame->channels;
                     int nb_samples = f.m_frame->nb_samples;
+                    int format = f.m_frame->format;
                     const uint8_t** data = (const uint8_t**)&f.m_frame->data[0];
                     int frame_buffer_size = av_samples_get_buffer_size(NULL, channels, nb_samples, d->sdl_sample_format, 0);
-                        
+
                     if (frame_buffer_size != d->swr_buffer_size) {
                         if (d->swr_buffer) delete[] d->swr_buffer;
                         d->swr_buffer = new uint8_t[frame_buffer_size];
                         d->swr_buffer_size = frame_buffer_size;
                     }
 
                     swr_convert(d->swr_ctx, &d->swr_buffer, nb_samples, data, nb_samples);
-                    int mark = std::min(len, d->swr_buffer_size);
-                    if (player->running) memcpy(temp + ptr, d->swr_buffer, mark);
-                    ptr += mark;
-                    len -= mark;
+
+                    d->rtClock.sync(f.m_rts); 
+                    d->reader->seek_found_pts = AV_NOPTS_VALUE;
+
+                    if (player->progressCallback) {
+                        if (!d->reader->has_video()) {
+                            if (d->reader->duration()) {
+                                float pct = (float)f.m_rts / (float)d->reader->duration();
+                                int progress = (int)(1000 * pct);
+                                if (progress != player->last_progress) {
+                                    player->progressCallback(pct);
+                                    player->last_progress = progress;
+                                }
+                            }
+                        }
+                    }
+
+                    if (d->afq_out)
+                        d->afq_out->push_move(f);
+                    else
+                        f.invalidate();
                 }
                 else {
                     if (d->afq_out) d->afq_out->push_move(f);
                     SDL_PauseAudioDevice(d->audioDeviceID, true);
                     if (!d->vfq_in) {
                         len = -1;
                         d->audio_eof = true;
@@ -412,36 +432,28 @@
                         event.type = SDL_QUIT;
                         SDL_PushEvent(&event);
                     }
                     return;
                 }
             }
 
-            if (!d->mute)
-                SDL_MixAudioFormat(audio_buffer, temp, d->sdl.format, d->audio_buffer_len, SDL_MIX_MAXVOLUME * d->volume);
-
-            d->rtClock.sync(f.m_rts); 
-            d->reader->seek_found_pts = AV_NOPTS_VALUE;
+            int swr_residual = d->swr_buffer_size - d->swr_ptr;
+            int tmp_residual = d->audio_buffer_len - len;
+            int mark = std::min(len, swr_residual);
+
+            if (player->running) memcpy(temp + tmp_residual, d->swr_buffer + d->swr_ptr, mark);
+            len -= mark;
+            d->swr_ptr += mark;
+            if (d->swr_ptr >= d->swr_buffer_size)
+                d->swr_ptr = 0;
+        }
 
-            if (player->progressCallback) {
-                if (d->reader->duration()) {
-                    float pct = (float)f.m_rts / (float)d->reader->duration();
-                    int progress = (int)(1000 * pct);
-                    if (progress != player->last_progress) {
-                        player->progressCallback(pct);
-                        player->last_progress = progress;
-                    }
-                }
-            }
+        if (!d->mute)
+            SDL_MixAudioFormat(audio_buffer, temp, d->sdl.format, d->audio_buffer_len, SDL_MIX_MAXVOLUME * d->volume);
 
-            if (d->afq_out)
-                d->afq_out->push_move(f);
-            else
-                f.invalidate();
-        }
     }
     catch (const Exception& e) { 
         std::stringstream str;
         str << "Audio callback exception: " << e.what();
         if (d->infoCallback) d->infoCallback(str.str());
         else std::cout << str.str() << std::endl;
     }
```

### Comparing `avio-2.1.3/src/Encoder.cpp` & `avio-2.1.4/src/Encoder.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/src/Exception.cpp` & `avio-2.1.4/src/Exception.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/src/Filter.cpp` & `avio-2.1.4/src/Filter.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/src/Frame.cpp` & `avio-2.1.4/src/Frame.cpp`

 * *Files 21% similar despite different names*

```diff
@@ -228,8 +228,41 @@
 int Frame::stride()
 {
 	int result = 0;
 	if (m_frame) result = m_frame->linesize[0];
 	return result;
 }
 
+int Frame::nb_samples()
+{
+	int result = 0;
+	if (m_frame) result = m_frame->nb_samples;
+	return result;
+}
+
+int Frame::sample_rate()
+{
+	int result = 0;
+	if (m_frame) result = m_frame->sample_rate;
+	return result;
+}
+
+int64_t Frame::channels()
+{
+	int64_t result = 0;
+	if (m_frame) result = m_frame->channels;
+	return result;
+}
+
+int Frame::format()
+{
+	int result = -1;
+	if (m_frame) result = m_frame->format;
+	return result;
+}
+
+bool Frame::isPlanar()
+{
+	return av_sample_fmt_is_planar((AVSampleFormat)m_frame->format);
+}
+
 }
```

### Comparing `avio-2.1.3/src/Packet.cpp` & `avio-2.1.4/src/Packet.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/src/Pipe.cpp` & `avio-2.1.4/src/Pipe.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/src/Player.cpp` & `avio-2.1.4/src/Player.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/src/Reader.cpp` & `avio-2.1.4/src/Reader.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/src/Writer.cpp` & `avio-2.1.4/src/Writer.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.3/src/avio.cpp` & `avio-2.1.4/src/avio.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -56,14 +56,15 @@
         .def_readwrite("width", &Player::width)
         .def_readwrite("height", &Player::height)
         .def_readwrite("disable_video", &Player::disable_video)
         .def_readwrite("disable_audio", &Player::disable_audio)
         .def_readwrite("progressCallback", &Player::progressCallback)
         .def_readwrite("renderCallback", &Player::renderCallback)
         .def_readwrite("pythonCallback", &Player::pythonCallback)
+        .def_readwrite("pyAudioCallback", &Player::pyAudioCallback)
         .def_readwrite("infoCallback", &Player::infoCallback)
         .def_readwrite("errorCallback", &Player::errorCallback)
         .def_readwrite("cbMediaPlayingStarted", &Player::cbMediaPlayingStarted)
         .def_readwrite("cbMediaPlayingStopped", &Player::cbMediaPlayingStopped)
         .def_readwrite("uri", &Player::uri)
         .def_readwrite("hWnd", &Player::hWnd)
         .def_readwrite("vpq_size", &Player::vpq_size)
@@ -113,24 +114,37 @@
         .def(py::init<>())
         .def(py::init<const Frame&>())
         .def("isValid", &Frame::isValid)
         .def("invalidate", &Frame::invalidate)
         .def("width", &Frame::width)
         .def("height", &Frame::height)
         .def("stride", &Frame::stride)
+        .def("nb_samples", &Frame::nb_samples)
+        .def("sample_rate", &Frame::sample_rate)
+        .def("channels", &Frame::channels)
         .def_readwrite("m_rts", &Frame::m_rts)
         .def_buffer([](Frame &m) -> py::buffer_info {
-            return py::buffer_info(
-                m.data(),
-                sizeof(uint8_t),
-                py::format_descriptor<uint8_t>::format(),
-                3,
-                { m.height(), m.width(), 3},
-                { sizeof(uint8_t) * m.stride(), sizeof(uint8_t) * 3, sizeof(uint8_t) }
-            );
+            if (m.height() == 0 && m.width() == 0) {
+                return py::buffer_info(
+                    m.data(),
+                    sizeof(float),
+                    py::format_descriptor<float>::format(),
+                    1,
+                    { m.nb_samples() * m.channels() },
+                    { sizeof(float) }
+                );
+            }
+            else {
+                py::ssize_t element_size = sizeof(uint8_t);
+                std::string fmt_desc =  py::format_descriptor<uint8_t>::format();
+                std::vector<py::ssize_t> dims = { m.height(), m.width(), 3};
+                py::ssize_t ndim = dims.size();
+                std::vector<py::ssize_t> strides = { sizeof(uint8_t) * m.stride(), (py::ssize_t)(sizeof(uint8_t) * ndim), sizeof(uint8_t) };
+                return py::buffer_info(m.data(), element_size, fmt_desc, ndim, dims, strides);
+            }
         });
     py::class_<AVRational>(m, "AVRational")
         .def(py::init<>())
         .def_readwrite("num", &AVRational::num)
         .def_readwrite("den", &AVRational::den);
     py::enum_<AVMediaType>(m, "AVMediaType")
         .value("AVMEDIA_TYPE_UNKNOWN", AVMediaType::AVMEDIA_TYPE_UNKNOWN)
```

### Comparing `avio-2.1.3/src/avio.egg-info/PKG-INFO` & `avio-2.1.4/src/avio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avio
-Version: 2.1.3
+Version: 2.1.4
 Summary: A python module for processing media streams
 Author: Stephen Rhodes
 Author-email: Stephen Rhodes <sr99622@gmail.com>
 Project-URL: Homepage, https://github.com/sr99622/libavio
 Project-URL: Bug Tracker, https://github.com/sr99622/libavio/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `avio-2.1.3/src/avio.egg-info/SOURCES.txt` & `avio-2.1.4/src/avio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

